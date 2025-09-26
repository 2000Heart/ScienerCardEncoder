---
title: initCardEncoder
---
//[ScienerCardEncoder](index.html)/[initCardEncoder](init-card-encoder.html)



# initCardEncoder



[androidJvm]\
abstract fun [initCardEncoder](init-card-encoder.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)



初始化卡片编码器



配置发卡器的基本参数，包括酒店信息等。此方法必须在连接设备后、 进行任何卡片操作前调用。



#### Parameters


androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，用于标识和配置发卡器 |
| callback | 初始化结果回调，成功时表示配置完成，失败时返回错误信息 |



#### See also


| | |
|---|---|
| [ScienerCardEncoder.connect](connect.html) | 连接设备方法 |
| [ScienerCardEncoder.initCard](init-card.html) | 下发空白卡方法 |


#### Samples

```kotlin
import com.ttlock.cardencoder.ScienerCardEncoder
import com.ttlock.cardencoder.api.CardClearResult
import com.ttlock.cardencoder.api.CardEncoderCallback
import com.ttlock.cardencoder.api.CardEncoderDevice
import com.ttlock.cardencoder.api.CardEncoderException
import com.ttlock.cardencoder.api.CardEncoderTwoStepCallback
import com.ttlock.cardencoder.api.CardWriteResult
import com.ttlock.cardencoder.domain.entity.CardData

fun main() { 
   //sampleStart 
   val sdk = ScienerCardEncoder.getInstance()

sdk.initCardEncoder("HOTEL_001", object : CardEncoderCallback<Unit> {
    override fun onSuccess(result: Unit) {
        // 初始化成功，可以进行卡片操作
        println("卡片编码器初始化成功")
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 初始化失败，处理错误
        println("初始化失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



