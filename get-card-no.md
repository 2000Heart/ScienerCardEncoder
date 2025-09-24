---
title: getCardNo
---
//[ScienerCardEncoder](index.html)/[getCardNo](get-card-no.html)



# getCardNo



[androidJvm]\
abstract fun [getCardNo](get-card-no.html)(callback: CardEncoderTwoStepCallback&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)



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
| CardEncoderTwoStepCallback | 两步操作回调接口 |


#### Samples

```kotlin
import com.ttlock.cardencoder.ScienerCardEncoder
import com.ttlock.cardencoder.api.CardEncoderDevice
import com.ttlock.cardencoder.api.CardEncoderCallback
import com.ttlock.cardencoder.api.CardEncoderTwoStepCallback
import com.ttlock.cardencoder.api.CardEncoderException
import com.ttlock.cardencoder.api.CardWriteResult
import com.ttlock.cardencoder.api.CardReadResult
import com.ttlock.cardencoder.api.CardClearResult

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



