---
title: clearCard
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[clearCard](clear-card.html)



# clearCard



[androidJvm]\
abstract fun [clearCard](clear-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[CardClearResult](../-card-clear-result/index.html)&gt;)



清空卡片中的酒店信息



清除卡片中已写入的酒店信息，使卡片恢复到空白状态。 这是一个两步操作，需要等待设备响应。



#### Parameters


androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，用于验证权限 |
| callback | 两步操作回调，包含接收和清空结果 |



#### See also


| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html) | 两步操作回调接口 |
| [CardClearResult](../-card-clear-result/index.html) | 清空结果数据类 |


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

sdk.clearCard("HOTEL_001", object : CardEncoderTwoStepCallback<CardClearResult> {
    override fun onReceive() {
        // 开始清空操作
        println("开始清空卡片...")
    }
    
    override fun onSuccess(result: CardClearResult) {
        if (result.isCleared) {
            // 清空成功
            println("卡片清空成功")
        } else {
            println("卡片清空失败: ${result.message}")
        }
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 清空失败
        println("清空卡片失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



