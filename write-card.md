---
title: writeCard
---
//[ScienerCardEncoder](index.html)/[writeCard](write-card.html)



# writeCard



[androidJvm]\
abstract fun [writeCard](write-card.html)(hotelInfo: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), buildNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), floorNo: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), mac: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), timestamp: [Long](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-long/index.html), allowLockOut: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html), callback: CardEncoderTwoStepCallback&lt;CardWriteResult&gt;)



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
| CardEncoderTwoStepCallback | 两步操作回调接口 |
| CardWriteResult | 写入结果数据类 |


#### Samples

```kotlin
import com.ttlock.cardencoder.ScienerCardEncoder
import com.ttlock.cardencoder.api.CardClearResult
import com.ttlock.cardencoder.api.CardEncoderCallback
import com.ttlock.cardencoder.api.CardEncoderDevice
import com.ttlock.cardencoder.api.CardEncoderException
import com.ttlock.cardencoder.api.CardEncoderTwoStepCallback
import com.ttlock.cardencoder.api.CardWriteResult
import com.ttlock.cardencoder.domain.entity.CardData

fun main() { 
   //sampleStart 
   val sdk = ScienerCardEncoder.getInstance()

sdk.writeCard(
    hotelInfo = "HOTEL_001",
    buildNo = 1,
    floorNo = 5,
    mac = "AA:BB:CC:DD:EE:FF",
    timestamp = System.currentTimeMillis(),
    allowLockOut = true,
    callback = object : CardEncoderTwoStepCallback<CardWriteResult> {
        override fun onReceive() {
            // 开始写入操作
            println("开始写入卡片信息...")
        }
        
        override fun onSuccess(result: CardWriteResult) {
            if (result.isWritten) {
                // 写入成功，result.cardNumber为卡号
                println("卡片写入成功，卡号: ${result.cardNumber}")
            } else {
                println("卡片写入失败: ${result.message}")
            }
        }
        
        override fun onFailure(error: CardEncoderException) {
            // 写入失败
            println("写入卡片失败: ${error.message}")
        }
    }
) 
   //sampleEnd
}
```



