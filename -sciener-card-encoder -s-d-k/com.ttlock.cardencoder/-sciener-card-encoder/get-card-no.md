---
title: getCardNo
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[getCardNo](get-card-no.html)



# getCardNo



[androidJvm]\
abstract fun [getCardNo](get-card-no.html)(callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)



读取卡片号码



从已插入的卡片中读取卡号信息。这是一个两步操作：



1. 
   首先调用onReceive()表示开始读取
2. 
   然后调用onSuccess()或onFailure()返回结果




#### Parameters


androidJvm

| | |
|---|---|
| callback | 两步操作回调，包含接收和结果回调 |



#### See also


| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html) | 两步操作回调接口 |


#### Samples

```kotlin
import com.ttlock.cardencoder.ScienerCardEncoder
import com.ttlock.cardencoder.CardEncoderDevice
import com.ttlock.cardencoder.CardEncoderCallback
import com.ttlock.cardencoder.CardEncoderTwoStepCallback
import com.ttlock.cardencoder.CardEncoderException
import com.ttlock.cardencoder.CardWriteResult
import com.ttlock.cardencoder.CardReadResult
import com.ttlock.cardencoder.CardClearResult

fun main() { 
   //sampleStart 
   val sdk = ScienerCardEncoder.getInstance()

sdk.getCardNo(object : CardEncoderTwoStepCallback<String> {
    override fun onReceive() {
        // 开始读取卡片，可以显示加载状态
        println("开始读取卡片...")
    }
    
    override fun onSuccess(result: String) {
        // 读取成功，result为卡号
        println("卡号: $result")
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 读取失败，处理错误
        println("读取卡号失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



