//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)/[initCardEncoder](init-card-encoder.md)

# initCardEncoder

[androidJvm]\
abstract fun [initCardEncoder](init-card-encoder.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)

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
| [ScienerCardEncoder.connect](connect.md) | 连接设备方法 |
| [ScienerCardEncoder.initCard](init-card.md) | 下发空白卡方法 |

#### Samples
