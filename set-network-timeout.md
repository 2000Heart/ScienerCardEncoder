---
title: setNetworkTimeout
---
//[ScienerCardEncoder](index.html)/[setNetworkTimeout](set-network-timeout.html)



# setNetworkTimeout



[androidJvm]\
abstract fun [setNetworkTimeout](set-network-timeout.html)(timeout: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html))



设置网络超时时间



配置网络请求的超时时间，防止网络请求长时间无响应。 建议设置为5-30秒之间。



#### Parameters


androidJvm

| | |
|---|---|
| timeout | 超时时间，单位毫秒，建议范围：5000-30000ms |



#### See also


| | |
|---|---|
| [ScienerCardEncoder.getNetworkTimeout](get-network-timeout.html) | 获取当前超时时间方法 |


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

// 设置10秒超时
sdk.setNetworkTimeout(10000)

// 设置30秒超时
sdk.setNetworkTimeout(30000)

// 获取当前超时时间
val timeout = sdk.getNetworkTimeout()
println("当前超时时间: ${timeout}ms") 
   //sampleEnd
}
```



