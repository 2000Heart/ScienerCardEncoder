---
title: ScienerCardEncoder
---
//[ScienerCardEncoder](index.html)



# ScienerCardEncoder



[androidJvm]\
abstract class [ScienerCardEncoder](index.html)

Sciener发卡器抽象基类



提供统一的回调接口，简化错误处理



## Constructors


| | |
|---|---|
| [ScienerCardEncoder](-sciener-card-encoder.html) | [androidJvm]<br>constructor() |


## Types


| Name | Summary |
|---|---|
| [Companion](-companion/index.html) | [androidJvm]<br>object [Companion](-companion/index.html) |


## Functions


| Name | Summary |
|---|---|
| [beep](beep.html) | [androidJvm]<br>abstract fun [beep](beep.html)(voiceLen: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), interval: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), voiceCount: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>控制蜂鸣器发声 |
| [clearCard](clear-card.html) | [androidJvm]<br>abstract fun [clearCard](clear-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderTwoStepCallback&lt;CardClearResult&gt;)<br>清空卡片中的酒店信息 |
| [connect](connect.html) | [androidJvm]<br>abstract fun [connect](connect.html)(device: CardEncoderDevice, callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>连接指定的卡片编码器设备 |
| [disconnect](disconnect.html) | [androidJvm]<br>abstract fun [disconnect](disconnect.html)(callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>断开当前连接的设备 |
| [getCardNo](get-card-no.html) | [androidJvm]<br>abstract fun [getCardNo](get-card-no.html)(callback: CardEncoderTwoStepCallback&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)<br>读取卡片号码 |
| [getNetworkTimeout](get-network-timeout.html) | [androidJvm]<br>abstract fun [getNetworkTimeout](get-network-timeout.html)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html)<br>获取当前网络超时时间 |
| [getSectorConfig](get-sector-config.html) | [androidJvm]<br>abstract fun [getSectorConfig](get-sector-config.html)(callback: CardEncoderCallback&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)<br>获取当前扇区配置 |
| [getServerBaseUrl](get-server-base-url.html) | [androidJvm]<br>abstract fun [getServerBaseUrl](get-server-base-url.html)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)<br>获取当前服务器基础URL |
| [initCard](init-card.html) | [androidJvm]<br>abstract fun [initCard](init-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>下发空白卡 |
| [initCardEncoder](init-card-encoder.html) | [androidJvm]<br>abstract fun [initCardEncoder](init-card-encoder.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)<br>初始化卡片编码器 |
| [isInitialized](is-initialized.html) | [androidJvm]<br>abstract fun [isInitialized](is-initialized.html)(): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)<br>检查发卡器是否已初始化 |
| [isLoggingEnabled](is-logging-enabled.html) | [androidJvm]<br>abstract fun [isLoggingEnabled](is-logging-enabled.html)(): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)<br>获取当前日志启用状态 |
| [readCard](read-card.html) | [androidJvm]<br>abstract fun [readCard](read-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderTwoStepCallback&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;CardData&gt;&gt;)<br>读取IC卡数据 |
| [scanDevices](scan-devices.html) | [androidJvm]<br>abstract fun [scanDevices](scan-devices.html)(callback: CardEncoderCallback&lt;[List](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin.collections/-list/index.html)&lt;CardEncoderDevice&gt;&gt;)<br>扫描设备 |
| [setLoggingEnabled](set-logging-enabled.html) | [androidJvm]<br>abstract fun [setLoggingEnabled](set-logging-enabled.html)(enabled: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html))<br>设置日志启用状态 |
| [setNetworkTimeout](set-network-timeout.html) | [androidJvm]<br>abstract fun [setNetworkTimeout](set-network-timeout.html)(timeout: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html))<br>设置网络超时时间 |
| [setSectorConfig](set-sector-config.html) | [androidJvm]<br>abstract fun [setSectorConfig](set-sector-config.html)(sectorSelect: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderCallback&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)<br>设置扇区配置 |
| [setServerBaseUrl](set-server-base-url.html) | [androidJvm]<br>abstract fun [setServerBaseUrl](set-server-base-url.html)(baseUrl: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html))<br>设置服务器基础URL |
| [writeCard](write-card.html) | [androidJvm]<br>abstract fun [writeCard](write-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), buildNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), floorNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), mac: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-long/index.html), allowLockOut: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), callback: CardEncoderTwoStepCallback&lt;CardWriteResult&gt;)<br>写入卡片酒店信息 |

