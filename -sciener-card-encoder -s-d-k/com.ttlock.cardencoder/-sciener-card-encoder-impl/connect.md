---
title: connect
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoderImpl](index.html)/[connect](connect.html)



# connect



[androidJvm]\
open override fun [connect](connect.html)(device: [CardEncoderDevice](../-card-encoder-device/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)



连接指定的卡片编码器设备



建立与指定设备的USB连接，连接成功后可以进行后续的卡片操作。 在调用其他操作前必须先连接设备。



#### Parameters


androidJvm

| | |
|---|---|
| device | 要连接的设备对象，通过scanDevices()方法获取 |
| callback | 连接结果回调，成功时表示连接建立，失败时返回错误信息 |



#### See also


| | |
|---|---|
| [ScienerCardEncoderImpl.scanDevices](scan-devices.html) | 扫描设备方法 |
| [CardEncoderDevice](../-card-encoder-device/index.html) | 设备信息实体类 |
| [ScienerCardEncoderImpl.disconnect](disconnect.html) | 断开连接方法 |


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
val selectedDevice = CardEncoderDevice(
    deviceId = "VID_1234_PID_5678",
    deviceName = "Sciener Card Encoder",
    vendorId = 1234,
    productId = 5678,
    deviceProductName = "Card Encoder Pro"
)

sdk.connect(selectedDevice, object : CardEncoderCallback<Unit> {
    override fun onSuccess(result: Unit) {
        // 连接成功，可以进行后续操作
        println("设备连接成功")
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 连接失败，处理错误
        println("设备连接失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



