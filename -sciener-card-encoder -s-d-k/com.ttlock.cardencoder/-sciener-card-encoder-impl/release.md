---
title: release
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoderImpl](index.html)/[release](release.html)



# release



[androidJvm]\
open override fun [release](release.html)(callback: [CardEncoderCallback](../-card-encoder-callback/index.html)&lt;[Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html)&gt;)



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
| [ScienerCardEncoderImpl.disconnect](disconnect.html) | 断开设备连接方法 |


#### Samples

```kotlin
import com.ttlock.cardencoder.ScienerCardEncoder
import com.ttlock.cardencoder.CardEncoderDevice
import com.ttlock.cardencoder.CardEncoderCallback
import com.ttlock.cardencoder.CardEncoderTwoStepCallback
import com.ttlock.cardencoder.CardEncoderException
import com.ttlock.cardencoder.CardWriteResult
import com.ttlock.cardencoder.CardReadResult
import com.ttlock.cardencoder.CardClearResult

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



