//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[beep](beep.md)

# beep

[androidJvm]\
open override fun [beep](beep.md)(voiceLen: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), interval: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), voiceCount: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), callback: [CardEncoderCallback](../-card-encoder-callback/index.md)&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)

控制蜂鸣器发声

控制发卡器的蜂鸣器发出提示音，用于用户操作反馈。 可以设置发声的长度、间隔和次数。

#### Parameters

androidJvm

| | |
|---|---|
| voiceLen | 单次发声长度，单位毫秒，建议范围：100-2000ms |
| interval | 发声间隔时间，单位毫秒，建议范围：100-1000ms |
| voiceCount | 发声次数，建议范围：1-10次 |
| callback | 控制结果回调，成功时表示蜂鸣器已启动，失败时返回错误信息 |

#### Samples
