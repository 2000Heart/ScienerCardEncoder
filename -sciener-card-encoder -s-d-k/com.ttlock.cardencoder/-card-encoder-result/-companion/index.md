//[ScienerCardEncoder SDK](../../../../index.md)/[com.ttlock.cardencoder](../../index.md)/[CardEncoderResult](../index.md)/[Companion](index.md)

# Companion

[androidJvm]\
object [Companion](index.md)

## Functions

| Name | Summary |
|---|---|
| [failure](failure.md) | [androidJvm]<br>fun &lt;[T](failure.md)&gt; [failure](failure.md)(error: [CardEncoderException](../../-card-encoder-exception/index.md)): [CardEncoderResult](../index.md)&lt;[T](failure.md)&gt;<br>创建失败结果<br>[androidJvm]<br>fun &lt;[T](failure.md)&gt; [failure](failure.md)(code: [CardEncoderCode](../../-card-encoder-code/index.md), message: [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-string/index.html)): [CardEncoderResult](../index.md)&lt;[T](failure.md)&gt;<br>创建失败结果（使用错误码和消息） |
| [success](success.md) | [androidJvm]<br>fun &lt;[T](success.md)&gt; [success](success.md)(data: [T](success.md)): [CardEncoderResult](../index.md)&lt;[T](success.md)&gt;<br>创建成功结果 |
