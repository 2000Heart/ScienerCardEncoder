//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)/[setSectorConfig](set-sector-config.md)

# setSectorConfig

[androidJvm]\
abstract fun [setSectorConfig](set-sector-config.md)(sectorSelect: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)

设置扇区配置

配置IC卡的扇区选择参数，用于指定读写操作的目标扇区。 扇区配置影响后续的卡片读写操作。

#### Parameters

androidJvm

| | |
|---|---|
| sectorSelect | 扇区选择配置字符串，格式为十六进制字符串 |
| callback | 设置结果回调，成功时返回true，失败时返回false |

#### See also

| | |
|---|---|
| [ScienerCardEncoder.getSectorConfig](get-sector-config.md) | 获取扇区配置方法 |

#### Samples
