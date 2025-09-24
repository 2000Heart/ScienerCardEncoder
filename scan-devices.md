---
title: scanDevices
---
//[ScienerCardEncoder](index.html)/[scanDevices](scan-devices.html)



# scanDevices



[androidJvm]\
abstract fun [scanDevices](scan-devices.html)(callback: CardEncoderCallback&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;CardEncoderDevice&gt;&gt;)



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
| CardEncoderDevice | 设备信息实体类 |
| CardEncoderCallback | 回调接口 |


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



