---
title: release
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[release](release.html)



# release



[androidJvm]\
abstract fun [release](release.html)(callback: CardEncoderCallback&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)



释放SDK资源



释放SDK占用的所有资源，包括设备连接、网络连接等。 在应用退出或不再使用SDK时调用此方法。



#### Parameters


androidJvm

| | |
|---|---|
| callback | 释放结果回调，成功时返回true，失败时返回false |



#### See also


| | |
|---|---|
| [ScienerCardEncoder.disconnect](disconnect.html) | 断开设备连接方法 |


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

sdk.release(object : CardEncoderCallback<Boolean> {
    override fun onSuccess(result: Boolean) {
        if (result) {
            // 资源释放成功
            println("SDK资源释放成功")
        } else {
            println("资源释放失败")
        }
    }
    
    override fun onFailure(error: CardEncoderException) {
        // 释放失败
        println("资源释放失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



