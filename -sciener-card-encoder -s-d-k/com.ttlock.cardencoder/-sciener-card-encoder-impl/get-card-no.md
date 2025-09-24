//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[getCardNo](get-card-no.md)

# getCardNo

[androidJvm]\
open override fun [getCardNo](get-card-no.md)(callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)

读取卡片号码

从已插入的卡片中读取卡号信息。这是一个两步操作：

1. 
   首先调用onReceive()表示开始读取
2. 
   然后调用onSuccess()或onFailure()返回结果

#### Parameters

androidJvm

| | |
|---|---|
| callback | 两步操作回调，包含接收和结果回调 |

#### See also

| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md) | 两步操作回调接口 |

#### Samples
