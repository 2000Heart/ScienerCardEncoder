---
title: readIcCard
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[readIcCard](read-ic-card.html)



# readIcCard



[androidJvm]\
abstract fun [readIcCard](read-ic-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[CardReadResult](../-card-read-result/index.html)&gt;)



读取IC卡数据



从已插入的IC卡中读取完整的卡片数据，包括酒店信息、楼栋、楼层等。 这是一个两步操作，需要等待设备响应。



#### Parameters


androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，用于验证权限 |
| callback | 两步操作回调，包含接收和读取结果 |



#### See also


| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html) | 两步操作回调接口 |
| [CardReadResult](../-card-read-result/index.html) | 读取结果数据类 |


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

sdk.readIcCard("HOTEL_001", object : CardEncoderTwoStepCallback<CardReadResult> {
    override fun onReceive() {
        // 开始读取IC卡数据
        println("开始读取IC卡数据...")
    }
    
    override fun onSuccess(result: CardReadResult) {
        if (result.isRead) {
            // 读取成功，result.cardData包含卡片数据
            println("IC卡数据读取成功: ${result.cardData}")
        } else {
            println("IC卡数据读取失败: ${result.message}")
        }
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 读取失败
        println("读取IC卡数据失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



