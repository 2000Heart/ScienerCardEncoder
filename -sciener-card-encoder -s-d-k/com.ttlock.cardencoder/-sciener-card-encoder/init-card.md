//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)/[initCard](init-card.md)

# initCard

[androidJvm]\
abstract fun [initCard](init-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)

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
| [ScienerCardEncoder.initCardEncoder](init-card-encoder.md) | 初始化卡片编码器方法 |
| [ScienerCardEncoder.writeCard](write-card.md) | 写入卡片信息方法 |

#### Samples
