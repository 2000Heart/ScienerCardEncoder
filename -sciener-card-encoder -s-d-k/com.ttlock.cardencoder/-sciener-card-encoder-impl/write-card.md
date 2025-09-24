//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[writeCard](write-card.md)

# writeCard

[androidJvm]\
open override fun [writeCard](write-card.md)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), buildNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), floorNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), mac: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-long/index.html), allowLockOut: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), callback: [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md)&lt;[CardWriteResult](../-card-write-result/index.md)&gt;)

写入卡片酒店信息

将酒店门锁的详细信息写入到卡片中，包括楼栋、楼层、MAC地址等。 这是一个两步操作，需要等待设备响应。

#### Parameters

androidJvm

| | |
|---|---|
| hotelInfo | 酒店信息字符串，用于标识酒店 |
| buildNo | 楼栋号，用于指定具体的楼栋 |
| floorNo | 楼层号，用于指定具体的楼层 |
| mac | 门锁MAC地址，用于指定具体的门锁设备 |
| timestamp | 时间戳，用于设置卡片的有效时间 |
| allowLockOut | 是否允许开反锁，true表示可以开反锁，false表示只能开正锁 |
| callback | 两步操作回调，包含接收和写入结果 |

#### See also

| | |
|---|---|
| [CardEncoderTwoStepCallback](../-card-encoder-two-step-callback/index.md) | 两步操作回调接口 |
| [CardWriteResult](../-card-write-result/index.md) | 写入结果数据类 |

#### Samples
