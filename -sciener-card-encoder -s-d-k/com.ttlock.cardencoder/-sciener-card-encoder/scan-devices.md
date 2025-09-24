---
title: scanDevices
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[scanDevices](scan-devices.html)



# scanDevices



[androidJvm]\
abstract fun [scanDevices](scan-devices.html)(callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;[CardEncoderDevice](../-card-encoder-device/index.html)&gt;&gt;)



扫描设备



扫描系统中所有可用的USB设备。 通常在应用启动时调用此方法来获取可用设备列表。



#### Parameters


androidJvm

| | |
|---|---|
| callback | 扫描结果回调，成功时返回设备列表，失败时返回错误信息 |



#### See also


| | |
|---|---|
| [CardEncoderDevice](../-card-encoder-device/index.html) | 设备信息实体类 |
| [CardEncoderCallback](../-card-encoder-callback/index.html) | 回调接口 |


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

sdk.scanDevices(object : CardEncoderCallback<List<CardEncoderDevice>> {
    override fun onSuccess(result: List<CardEncoderDevice>) {
        // 处理设备列表
        result.forEach { device ->
            println("设备: ${device.getDisplayName()}")
        }
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 处理错误
        println("扫描设备失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



