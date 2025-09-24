//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)/[disconnect](disconnect.md)

# disconnect

[androidJvm]\
abstract fun [disconnect](disconnect.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)

断开当前连接的设备

释放与当前设备的USB连接，释放相关资源。 在应用退出或不再需要操作设备时调用此方法。

#### Parameters

androidJvm

| | |
|---|---|
| callback | 断开连接结果回调，成功时表示连接已断开，失败时返回错误信息 |

#### See also

| | |
|---|---|
| [ScienerCardEncoder.connect](connect.md) | 连接设备方法 |

#### Samples
