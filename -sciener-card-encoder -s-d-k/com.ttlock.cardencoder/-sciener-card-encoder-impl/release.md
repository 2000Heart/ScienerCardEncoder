//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[release](release.md)

# release

[androidJvm]\
open override fun [release](release.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)

释放SDK资源

释放SDK占用的所有资源，包括设备连接、网络连接等。 在应用退出或不再使用SDK时调用此方法。

#### Parameters

androidJvm

| | |
|---|---|
| callback | 释放结果回调，成功时返回true，失败时返回false |

#### See also

| | |
|---|---|
| [ScienerCardEncoderImpl.disconnect](disconnect.md) | 断开设备连接方法 |

#### Samples
