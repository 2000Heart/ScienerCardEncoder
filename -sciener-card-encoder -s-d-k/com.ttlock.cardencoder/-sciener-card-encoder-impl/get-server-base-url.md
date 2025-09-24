---
title: getServerBaseUrl
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[ScienerCardEncoderImpl](index.html)/[getServerBaseUrl](get-server-base-url.html)



# getServerBaseUrl



[androidJvm]\
open override fun [getServerBaseUrl](get-server-base-url.html)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)



获取当前服务器基础URL



获取当前配置的服务器地址。



#### Return



当前服务器基础URL字符串



#### See also


| | |
|---|---|
| [ScienerCardEncoderImpl.setServerBaseUrl](set-server-base-url.html) | 设置服务器URL方法 |


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

// 使用默认服务器
sdk.setServerBaseUrl("https://cnapi.ttlock.com/v3")

// 使用测试服务器
sdk.setServerBaseUrl("https://testapi.ttlock.com/v3")

// 获取当前服务器URL
val currentUrl = sdk.getServerBaseUrl()
println("当前服务器: $currentUrl") 
   //sampleEnd
}
```



