---
title: disconnect
---
//[ScienerCardEncoder](index.html)/[disconnect](disconnect.html)



# disconnect



[androidJvm]\
abstract fun [disconnect](disconnect.html)(callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)



断开当前连接的设备



释放与当前设备的USB连接，释放相关资源。 在应用退出或不再需要操作设备时调用此方法。



#### Parameters


androidJvm

| | |
|---|---|
| callback | 断开连接结果回调，成功时表示连接已断开，失败时返回错误信息 |



#### See also


| | |
|---|---|
| [ScienerCardEncoder.connect](connect.html) | 连接设备方法 |


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

sdk.disconnect(object : CardEncoderCallback<Unit> {
    override fun onSuccess(result: Unit) {
        // 断开连接成功
        println("设备断开成功")
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 断开连接失败，处理错误
        println("设备断开失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



