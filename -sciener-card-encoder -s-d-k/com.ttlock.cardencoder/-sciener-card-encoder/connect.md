//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)/[connect](connect.md)

# connect

[androidJvm]\
abstract fun [connect](connect.md)(device: [CardEncoderDevice](../-card-encoder-device/index.md), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)

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
| [ScienerCardEncoder.scanDevices](scan-devices.md) | 扫描设备方法 |
| [CardEncoderDevice](../-card-encoder-device/index.md) | 设备信息实体类 |
| [ScienerCardEncoder.disconnect](disconnect.md) | 断开连接方法 |

#### Samples
