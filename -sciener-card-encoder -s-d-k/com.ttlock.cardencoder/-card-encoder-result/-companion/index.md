---
title: Companion
---
//[ScienerCardEncoder SDK](../../../../index.html)/[com.ttlock.cardencoder](../../index.html)/[CardEncoderResult](../index.html)/[Companion](index.html)



# Companion



[androidJvm]\
object [Companion](index.html)



## Functions


| Name | Summary |
|---|---|
| [failure](failure.html) | [androidJvm]<br>fun &lt;[T](failure.html)&gt; [failure](failure.html)(error: [CardEncoderException](../../-card-encoder-exception/index.html)): [CardEncoderResult](../index.html)&lt;[T](failure.html)&gt;<br>创建失败结果<br>[androidJvm]<br>fun &lt;[T](failure.html)&gt; [failure](failure.html)(code: [CardEncoderCode](../../-card-encoder-code/index.html), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)): [CardEncoderResult](../index.html)&lt;[T](failure.html)&gt;<br>创建失败结果（使用错误码和消息） |
| [success](success.html) | [androidJvm]<br>fun &lt;[T](success.html)&gt; [success](success.html)(data: [T](success.html)): [CardEncoderResult](../index.html)&lt;[T](success.html)&gt;<br>创建成功结果 |

