//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoder](index.md)

# ScienerCardEncoder

abstract class [ScienerCardEncoder](index.md)

Sciener发卡器抽象基类

提供统一的回调接口，简化错误处理

#### Inheritors

| |
|---|
| [ScienerCardEncoderImpl](../-sciener-card-encoder-impl/index.md) |

## Constructors

| | |
|---|---|
| [ScienerCardEncoder](-sciener-card-encoder.md) | [androidJvm]<br>constructor() |

## Types

| Name | Summary |
|---|---|
| [Companion](-companion/index.md) | [androidJvm]<br>object [Companion](-companion/index.md) |

## Functions

| Name | Summary |
|---|---|
| [beep](beep.md) | [androidJvm]<br>abstract fun [beep](beep.md)(voiceLen: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), interval: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), voiceCount: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>控制蜂鸣器发声 |
| [clearCard](clear-card.md) | [androidJvm]<br>abstract fun [clearCard](clear-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[CardClearResult](../-card-clear-result/index.md)&gt;)<br>清空卡片中的酒店信息 |
| [connect](connect.md) | [androidJvm]<br>abstract fun [connect](connect.md)(device: [CardEncoderDevice](../-card-encoder-device/index.md), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>连接指定的卡片编码器设备 |
| [disconnect](disconnect.md) | [androidJvm]<br>abstract fun [disconnect](disconnect.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>断开当前连接的设备 |
| [getCardNo](get-card-no.md) | [androidJvm]<br>abstract fun [getCardNo](get-card-no.md)(callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)<br>读取卡片号码 |
| [getNetworkTimeout](get-network-timeout.md) | [androidJvm]<br>abstract fun [getNetworkTimeout](get-network-timeout.md)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html)<br>获取当前网络超时时间 |
| [getSectorConfig](get-sector-config.md) | [androidJvm]<br>abstract fun [getSectorConfig](get-sector-config.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)<br>获取当前扇区配置 |
| [getServerBaseUrl](get-server-base-url.md) | [androidJvm]<br>abstract fun [getServerBaseUrl](get-server-base-url.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)<br>获取当前服务器基础URL |
| [initCard](init-card.md) | [androidJvm]<br>abstract fun [initCard](init-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>下发空白卡 |
| [initCardEncoder](init-card-encoder.md) | [androidJvm]<br>abstract fun [initCardEncoder](init-card-encoder.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>初始化卡片编码器 |
| [isInitialized](is-initialized.md) | [androidJvm]<br>abstract fun [isInitialized](is-initialized.md)(): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)<br>检查发卡器是否已初始化 |
| [readIcCard](read-ic-card.md) | [androidJvm]<br>abstract fun [readIcCard](read-ic-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[CardReadResult](../-card-read-result/index.md)&gt;)<br>读取IC卡数据 |
| [release](release.md) | [androidJvm]<br>abstract fun [release](release.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)<br>释放SDK资源 |
| [scanDevices](scan-devices.md) | [androidJvm]<br>abstract fun [scanDevices](scan-devices.md)(callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;[CardEncoderDevice](../-card-encoder-device/index.md)&gt;&gt;)<br>扫描设备 |
| [setNetworkTimeout](set-network-timeout.md) | [androidJvm]<br>abstract fun [setNetworkTimeout](set-network-timeout.md)(timeout: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html))<br>设置网络超时时间 |
| [setSectorConfig](set-sector-config.md) | [androidJvm]<br>abstract fun [setSectorConfig](set-sector-config.md)(sectorSelect: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)<br>设置扇区配置 |
| [setServerBaseUrl](set-server-base-url.md) | [androidJvm]<br>abstract fun [setServerBaseUrl](set-server-base-url.md)(baseUrl: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html))<br>设置服务器基础URL |
| [writeCard](write-card.md) | [androidJvm]<br>abstract fun [writeCard](write-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), buildNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), floorNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), mac: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-long/index.html), allowLockOut: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[CardWriteResult](../-card-write-result/index.md)&gt;)<br>写入卡片酒店信息 |
