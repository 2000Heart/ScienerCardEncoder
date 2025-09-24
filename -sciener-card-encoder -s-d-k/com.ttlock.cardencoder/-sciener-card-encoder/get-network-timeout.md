---
title: getNetworkTimeout
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoder](index.html)/[getNetworkTimeout](get-network-timeout.html)



# getNetworkTimeout



[androidJvm]\
abstract fun [getNetworkTimeout](get-network-timeout.html)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html)



获取当前网络超时时间



获取当前配置的网络请求超时时间。



#### Return



当前网络超时时间，单位毫秒



#### See also


| | |
|---|---|
| [ScienerCardEncoder.setNetworkTimeout](set-network-timeout.html) | 设置网络超时时间方法 |


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



