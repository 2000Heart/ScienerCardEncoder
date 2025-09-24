---
title: initialize
---
//[ScienerCardEncoder SDK](../../../../index.html)/[com.ttlock.cardencoder](../../index.html)/[ScienerCardEncoder](../index.html)/[Companion](index.html)/[initialize](initialize.html)



# initialize



[androidJvm]\
fun [initialize](initialize.html)(context: [Application](https://developer.android.com/reference/kotlin/android/app/Application.html), enableLogging: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html) = true, enableErrorHandling: [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-boolean/index.html) = true, serverBaseUrl: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) = &quot;https://cnapi.ttlock.com/v3&quot;): [ScienerCardEncoder](../index.html)



初始化SDK（只能调用一次）



#### Return



SDK实例



#### Parameters


androidJvm

| | |
|---|---|
| context | 应用上下文 |
| enableLogging | 是否启用日志 |
| enableErrorHandling | 是否启用错误处理 |
| serverBaseUrl | 服务器基础URL |



#### Throws


| | |
|---|---|
| [IllegalStateException](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-illegal-state-exception/index.html) | 如果已经初始化过 |



