---
title: getSectorConfig
---
//[ScienerCardEncoder](index.html)/[getSectorConfig](get-sector-config.html)



# getSectorConfig



[androidJvm]\
abstract fun [getSectorConfig](get-sector-config.html)(callback: CardEncoderCallback&lt;[String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)&gt;)



获取当前扇区配置



获取当前设置的扇区选择配置参数。



#### Parameters


androidJvm

| | |
|---|---|
| callback | 获取结果回调，成功时返回配置字符串，失败时返回错误信息 |



#### See also


| | |
|---|---|
| [ScienerCardEncoder.setSectorConfig](set-sector-config.html) | 设置扇区配置方法 |


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

sdk.getSectorConfig(object : CardEncoderCallback<String> {
    override fun onSuccess(result: String) {
        // 使用扇区配置
        println("当前扇区配置: $result")
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 获取失败
        println("获取扇区配置失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



