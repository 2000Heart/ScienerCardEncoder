//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[CardEncoderDevice](index.md)

# CardEncoderDevice

[androidJvm]\
data class [CardEncoderDevice](index.md)(val deviceId: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), val deviceName: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), val vendorId: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), val productId: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), val deviceProductName: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)?, val serialNumber: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? = null, val devicePath: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? = null)

卡片读取器设备实体

用于表示业务层的设备信息，与底层USB设备解耦

## Constructors

| | |
|---|---|
| [CardEncoderDevice](-card-encoder-device.md) | [androidJvm]<br>constructor(deviceId: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), deviceName: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), vendorId: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), productId: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), deviceProductName: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)?, serialNumber: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? = null, devicePath: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? = null) |

## Properties

| Name | Summary |
|---|---|
| [deviceId](device-id.md) | [androidJvm]<br>val [deviceId](device-id.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |
| [deviceName](device-name.md) | [androidJvm]<br>val [deviceName](device-name.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |
| [devicePath](device-path.md) | [androidJvm]<br>val [devicePath](device-path.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? = null |
| [deviceProductName](device-product-name.md) | [androidJvm]<br>val [deviceProductName](device-product-name.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? |
| [productId](product-id.md) | [androidJvm]<br>val [productId](product-id.md): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html) |
| [serialNumber](serial-number.md) | [androidJvm]<br>val [serialNumber](serial-number.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)? = null |
| [vendorId](vendor-id.md) | [androidJvm]<br>val [vendorId](vendor-id.md): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html) |

## Functions

| Name | Summary |
|---|---|
| [equals](equals.md) | [androidJvm]<br>open operator override fun [equals](equals.md)(other: [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-any/index.html)?): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html) |
| [getDescription](get-description.md) | [androidJvm]<br>fun [getDescription](get-description.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)<br>获取设备描述信息 |
| [getDisplayName](get-display-name.md) | [androidJvm]<br>fun [getDisplayName](get-display-name.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)<br>获取设备显示名称 |
| [getProductName](get-product-name.md) | [androidJvm]<br>fun [getProductName](get-product-name.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)<br>获取产品显示名称 |
| [hashCode](hash-code.md) | [androidJvm]<br>open override fun [hashCode](hash-code.md)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html) |
| [isAvailable](is-available.md) | [androidJvm]<br>fun [isAvailable](is-available.md)(): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)<br>检查设备是否可用 |
| [toString](to-string.md) | [androidJvm]<br>open override fun [toString](to-string.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |
