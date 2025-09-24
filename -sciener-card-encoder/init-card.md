---
title: initCard
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[initCard](init-card.html)



# initCard



[androidJvm]\
abstract fun [initCard](init-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)



下发空白卡



向发卡器下发空白卡片，准备进行后续的卡片写入操作。 此方法需要在initCardEncoder()成功后调用。



#### Parameters


androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，必须与initCardEncoder()中使用的信息一致 |
| callback | 下发结果回调，成功时表示空白卡已下发，失败时返回错误信息 |



#### See also


| | |
|---|---|
| [ScienerCardEncoder.initCardEncoder](init-card-encoder.html) | 初始化卡片编码器方法 |
| [ScienerCardEncoder.writeCard](write-card.html) | 写入卡片信息方法 |


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

sdk.initCard("HOTEL_001", object : CardEncoderCallback<Unit> {
    override fun onSuccess(result: Unit) {
        // 空白卡下发成功，可以写入卡片信息
        println("空白卡下发成功")
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 下发失败，处理错误
        println("空白卡下发失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



