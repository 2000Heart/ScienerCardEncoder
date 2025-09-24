//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)/[clearCard](clear-card.md)

# clearCard

[androidJvm]\
abstract fun [clearCard](clear-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[CardClearResult](../-card-clear-result/index.md)&gt;)

清空卡片中的酒店信息

清除卡片中已写入的酒店信息，使卡片恢复到空白状态。 这是一个两步操作，需要等待设备响应。

#### Parameters

androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，用于验证权限 |
| callback | 两步操作回调，包含接收和清空结果 |

#### See also

| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md) | 两步操作回调接口 |
| [CardClearResult](../-card-clear-result/index.md) | 清空结果数据类 |

#### Samples
