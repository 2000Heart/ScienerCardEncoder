---
title: CardEncoderException
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[CardEncoderException](index.html)



# CardEncoderException



[androidJvm]\
class [CardEncoderException](index.html)(val code: [CardEncoderCode](../-card-encoder-code/index.html), val message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)) : [Exception](https://developer.android.com/reference/kotlin/java/lang/Exception.html)

卡片编码器统一异常类



## Constructors


| | |
|---|---|
| [CardEncoderException](-card-encoder-exception.html) | [androidJvm]<br>constructor(code: [CardEncoderCode](../-card-encoder-code/index.html), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)) |


## Properties


| Name | Summary |
|---|---|
| [cause](index.html#-654012527%2FProperties%2F-1858324531) | [androidJvm]<br>open val [cause](index.html#-654012527%2FProperties%2F-1858324531): [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)? |
| [code](code.html) | [androidJvm]<br>val [code](code.html): [CardEncoderCode](../-card-encoder-code/index.html) |
| [message](message.html) | [androidJvm]<br>open override val [message](message.html): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |


## Functions


| Name | Summary |
|---|---|
| [addSuppressed](index.html#282858770%2FFunctions%2F-1858324531) | [androidJvm]<br>fun [addSuppressed](index.html#282858770%2FFunctions%2F-1858324531)(p0: [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)) |
| [fillInStackTrace](index.html#-1102069925%2FFunctions%2F-1858324531) | [androidJvm]<br>open fun [fillInStackTrace](index.html#-1102069925%2FFunctions%2F-1858324531)(): [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html) |
| [getLocalizedMessage](index.html#1043865560%2FFunctions%2F-1858324531) | [androidJvm]<br>open fun [getLocalizedMessage](index.html#1043865560%2FFunctions%2F-1858324531)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |
| [getStackTrace](index.html#2050903719%2FFunctions%2F-1858324531) | [androidJvm]<br>open fun [getStackTrace](index.html#2050903719%2FFunctions%2F-1858324531)(): [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-array/index.html)&lt;[StackTraceElement](https://developer.android.com/reference/kotlin/java/lang/StackTraceElement.html)&gt; |
| [getSuppressed](index.html#672492560%2FFunctions%2F-1858324531) | [androidJvm]<br>fun [getSuppressed](index.html#672492560%2FFunctions%2F-1858324531)(): [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-array/index.html)&lt;[Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)&gt; |
| [initCause](index.html#-418225042%2FFunctions%2F-1858324531) | [androidJvm]<br>open fun [initCause](index.html#-418225042%2FFunctions%2F-1858324531)(p0: [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)): [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html) |
| [printStackTrace](index.html#-1769529168%2FFunctions%2F-1858324531) | [androidJvm]<br>open fun [printStackTrace](index.html#-1769529168%2FFunctions%2F-1858324531)()<br>open fun [printStackTrace](index.html#1841853697%2FFunctions%2F-1858324531)(p0: [PrintStream](https://developer.android.com/reference/kotlin/java/io/PrintStream.html))<br>open fun [printStackTrace](index.html#1175535278%2FFunctions%2F-1858324531)(p0: [PrintWriter](https://developer.android.com/reference/kotlin/java/io/PrintWriter.html)) |
| [setStackTrace](index.html#2135801318%2FFunctions%2F-1858324531) | [androidJvm]<br>open fun [setStackTrace](index.html#2135801318%2FFunctions%2F-1858324531)(p0: [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-array/index.html)&lt;[StackTraceElement](https://developer.android.com/reference/kotlin/java/lang/StackTraceElement.html)&gt;) |
| [toString](to-string.html) | [androidJvm]<br>open override fun [toString](to-string.html)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |

