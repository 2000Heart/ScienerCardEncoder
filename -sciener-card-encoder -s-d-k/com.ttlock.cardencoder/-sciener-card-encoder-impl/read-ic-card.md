//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[readIcCard](read-ic-card.md)

# readIcCard

[androidJvm]\
open override fun [readIcCard](read-ic-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[CardReadResult](../-card-read-result/index.md)&gt;)

读取IC卡数据

从已插入的IC卡中读取完整的卡片数据，包括酒店信息、楼栋、楼层等。 这是一个两步操作，需要等待设备响应。

#### Parameters

androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，用于验证权限 |
| callback | 两步操作回调，包含接收和读取结果 |

#### See also

| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md) | 两步操作回调接口 |
| [CardReadResult](../-card-read-result/index.md) | 读取结果数据类 |

#### Samples
