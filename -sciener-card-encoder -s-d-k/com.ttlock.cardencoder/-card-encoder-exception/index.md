//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[CardEncoderException](index.md)

# CardEncoderException

[androidJvm]\
class [CardEncoderException](index.md)(val code: [CardEncoderCode](../-card-encoder-code/index.md), val message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)) : [Exception](https://developer.android.com/reference/kotlin/java/lang/Exception.html)

卡片编码器统一异常类

## Constructors

| | |
|---|---|
| [CardEncoderException](-card-encoder-exception.md) | [androidJvm]<br>constructor(code: [CardEncoderCode](../-card-encoder-code/index.md), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)) |

## Properties

| Name | Summary |
|---|---|
| [cause](index.md#-654012527%2FProperties%2F-756506834) | [androidJvm]<br>open val [cause](index.md#-654012527%2FProperties%2F-756506834): [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)? |
| [code](code.md) | [androidJvm]<br>val [code](code.md): [CardEncoderCode](../-card-encoder-code/index.md) |
| [message](message.md) | [androidJvm]<br>open override val [message](message.md): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |

## Functions

| Name | Summary |
|---|---|
| [addSuppressed](index.md#282858770%2FFunctions%2F-756506834) | [androidJvm]<br>fun [addSuppressed](index.md#282858770%2FFunctions%2F-756506834)(p0: [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)) |
| [fillInStackTrace](index.md#-1102069925%2FFunctions%2F-756506834) | [androidJvm]<br>open fun [fillInStackTrace](index.md#-1102069925%2FFunctions%2F-756506834)(): [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html) |
| [getLocalizedMessage](index.md#1043865560%2FFunctions%2F-756506834) | [androidJvm]<br>open fun [getLocalizedMessage](index.md#1043865560%2FFunctions%2F-756506834)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |
| [getStackTrace](index.md#2050903719%2FFunctions%2F-756506834) | [androidJvm]<br>open fun [getStackTrace](index.md#2050903719%2FFunctions%2F-756506834)(): [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-array/index.html)&lt;[StackTraceElement](https://developer.android.com/reference/kotlin/java/lang/StackTraceElement.html)&gt; |
| [getSuppressed](index.md#672492560%2FFunctions%2F-756506834) | [androidJvm]<br>fun [getSuppressed](index.md#672492560%2FFunctions%2F-756506834)(): [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-array/index.html)&lt;[Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)&gt; |
| [initCause](index.md#-418225042%2FFunctions%2F-756506834) | [androidJvm]<br>open fun [initCause](index.md#-418225042%2FFunctions%2F-756506834)(p0: [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html)): [Throwable](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-throwable/index.html) |
| [printStackTrace](index.md#-1769529168%2FFunctions%2F-756506834) | [androidJvm]<br>open fun [printStackTrace](index.md#-1769529168%2FFunctions%2F-756506834)()<br>open fun [printStackTrace](index.md#1841853697%2FFunctions%2F-756506834)(p0: [PrintStream](https://developer.android.com/reference/kotlin/java/io/PrintStream.html))<br>open fun [printStackTrace](index.md#1175535278%2FFunctions%2F-756506834)(p0: [PrintWriter](https://developer.android.com/reference/kotlin/java/io/PrintWriter.html)) |
| [setStackTrace](index.md#2135801318%2FFunctions%2F-756506834) | [androidJvm]<br>open fun [setStackTrace](index.md#2135801318%2FFunctions%2F-756506834)(p0: [Array](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-array/index.html)&lt;[StackTraceElement](https://developer.android.com/reference/kotlin/java/lang/StackTraceElement.html)&gt;) |
| [toString](to-string.md) | [androidJvm]<br>open override fun [toString](to-string.md)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html) |
