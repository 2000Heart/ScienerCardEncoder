//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[scanDevices](scan-devices.md)

# scanDevices

[androidJvm]\
open override fun [scanDevices](scan-devices.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;[CardEncoderDevice](../-card-encoder-device/index.md)&gt;&gt;)

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
| [CardEncoderDevice](../-card-encoder-device/index.md) | 设备信息实体类 |
| [CardEncoderCallback](../-card-encoder-callback/index.md) | 回调接口 |

#### Samples
