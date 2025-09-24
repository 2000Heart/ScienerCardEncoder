---
title: setSectorConfig
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[setSectorConfig](set-sector-config.html)



# setSectorConfig



[androidJvm]\
abstract fun [setSectorConfig](set-sector-config.html)(sectorSelect: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html), callback: CardEncoderCallback&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)



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
| [ScienerCardEncoder.getSectorConfig](get-sector-config.html) | 获取扇区配置方法 |


#### Samples

```kotlin
import com.ttlock.cardencoder.ScienerCardEncoder
import com.ttlock.cardencoder.api.CardEncoderDevice
import com.ttlock.cardencoder.api.CardEncoderCallback
import com.ttlock.cardencoder.api.CardEncoderTwoStepCallback
import com.ttlock.cardencoder.api.CardEncoderException
import com.ttlock.cardencoder.api.CardWriteResult
import com.ttlock.cardencoder.api.CardReadResult
import com.ttlock.cardencoder.api.CardClearResult

fun main() { 
   //sampleStart 
   val sdk = ScienerCardEncoder.getInstance()

sdk.setSectorConfig("FF0000", object : CardEncoderCallback<Boolean> {
    override fun onSuccess(result: Boolean) {
        if (result) {
            // 扇区配置设置成功
            println("扇区配置设置成功")
        } else {
            println("扇区配置设置失败")
        }
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 设置失败
        println("扇区配置设置失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



