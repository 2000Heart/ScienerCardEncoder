---
title: beep
---
//[ScienerCardEncoder](index.html)/[beep](beep.html)



# beep



[androidJvm]\
abstract fun [beep](beep.html)(voiceLen: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), interval: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), voiceCount: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html), callback: CardEncoderCallback&lt;[Unit](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-unit/index.html)&gt;)



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

// 短促提示音
sdk.beep(200, 0, 1, object : CardEncoderCallback<Unit> {
    override fun onSuccess(result: Unit) {
        println("蜂鸣器发声成功")
    }
    
    override fun onFailure(error: CardEncoderException) {
        println("蜂鸣器发声失败: ${error.message}")
    }
})

// 长提示音
sdk.beep(500, 200, 3, object : CardEncoderCallback<Unit> {
    override fun onSuccess(result: Unit) {
        println("长提示音播放成功")
    }
    
    override fun onFailure(error: CardEncoderException) {
        println("长提示音播放失败: ${error.message}")
    }
}) 
   //sampleEnd
}
```



