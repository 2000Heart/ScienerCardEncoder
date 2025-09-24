---
title: ScienerCardEncoderImpl
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoderImpl](index.html)



# ScienerCardEncoderImpl



[androidJvm]\
class [ScienerCardEncoderImpl](index.html)(context: [Application](https://developer.android.com/reference/kotlin/android/app/Application.html), enableLogging: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), enableErrorHandling: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)) : [ScienerCardEncoder](../-sciener-card-encoder/index.html)

ScienerCardEncoder的具体实现



## Constructors


| | |
|---|---|
| [ScienerCardEncoderImpl](-sciener-card-encoder-impl.html) | [androidJvm]<br>constructor(context: [Application](https://developer.android.com/reference/kotlin/android/app/Application.html), enableLogging: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), enableErrorHandling: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)) |


## Functions


| Name | Summary |
|---|---|
| [beep](beep.html) | [androidJvm]<br>open override fun [beep](beep.html)(voiceLen: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), interval: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), voiceCount: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>控制蜂鸣器发声 |
| [clearCard](clear-card.html) | [androidJvm]<br>open override fun [clearCard](clear-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[CardClearResult](../-card-clear-result/index.html)&gt;)<br>清空卡片中的酒店信息 |
| [connect](connect.html) | [androidJvm]<br>open override fun [connect](connect.html)(device: [CardEncoderDevice](../-card-encoder-device/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>连接指定的卡片编码器设备 |
| [disconnect](disconnect.html) | [androidJvm]<br>open override fun [disconnect](disconnect.html)(callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>断开当前连接的设备 |
| [getCardNo](get-card-no.html) | [androidJvm]<br>open override fun [getCardNo](get-card-no.html)(callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)<br>读取卡片号码 |
| [getNetworkTimeout](get-network-timeout.html) | [androidJvm]<br>open override fun [getNetworkTimeout](get-network-timeout.html)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html)<br>获取当前网络超时时间 |
| [getSectorConfig](get-sector-config.html) | [androidJvm]<br>open override fun [getSectorConfig](get-sector-config.html)(callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)<br>获取当前扇区配置 |
| [getServerBaseUrl](get-server-base-url.html) | [androidJvm]<br>open override fun [getServerBaseUrl](get-server-base-url.html)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)<br>获取当前服务器基础URL |
| [initCard](init-card.html) | [androidJvm]<br>open override fun [initCard](init-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>下发空白卡 |
| [initCardEncoder](init-card-encoder.html) | [androidJvm]<br>open override fun [initCardEncoder](init-card-encoder.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>初始化卡片编码器 |
| [isInitialized](is-initialized.html) | [androidJvm]<br>open override fun [isInitialized](is-initialized.html)(): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)<br>检查发卡器是否已初始化 |
| [parseError](parse-error.html) | [androidJvm]<br>fun [parseError](parse-error.html)(result: AtCommandResult): [CardEncoderException](../-card-encoder-exception/index.html) |
| [readIcCard](read-ic-card.html) | [androidJvm]<br>open override fun [readIcCard](read-ic-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[CardReadResult](../-card-read-result/index.html)&gt;)<br>读取IC卡数据 |
| [release](release.html) | [androidJvm]<br>open override fun [release](release.html)(callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)<br>释放SDK资源 |
| [scanDevices](scan-devices.html) | [androidJvm]<br>open override fun [scanDevices](scan-devices.html)(callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;[CardEncoderDevice](../-card-encoder-device/index.html)&gt;&gt;)<br>扫描设备 |
| [setNetworkTimeout](set-network-timeout.html) | [androidJvm]<br>open override fun [setNetworkTimeout](set-network-timeout.html)(timeout: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html))<br>设置网络超时时间 |
| [setSectorConfig](set-sector-config.html) | [androidJvm]<br>open override fun [setSectorConfig](set-sector-config.html)(sectorSelect: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)<br>设置扇区配置 |
| [setServerBaseUrl](set-server-base-url.html) | [androidJvm]<br>open override fun [setServerBaseUrl](set-server-base-url.html)(baseUrl: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html))<br>设置服务器基础URL |
| [writeCard](write-card.html) | [androidJvm]<br>open override fun [writeCard](write-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), buildNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), floorNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), mac: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-long/index.html), allowLockOut: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.html)&lt;[CardWriteResult](../-card-write-result/index.html)&gt;)<br>写入卡片酒店信息 |

