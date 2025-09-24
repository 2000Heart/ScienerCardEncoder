//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[CardEncoderTwoStepCallback](index.md)

# CardEncoderTwoStepCallback

interface [CardEncoderTwoStepCallback](index.md)&lt;[T](index.md)&gt;

统一的卡片编码器回调接口

#### Parameters

androidJvm

| | |
|---|---|
| T | 返回数据的类型 |

## Functions

| Name | Summary |
|---|---|
| [onFailure](on-failure.md) | [androidJvm]<br>abstract fun [onFailure](on-failure.md)(error: [CardEncoderException](../-card-encoder-exception/index.md))<br>操作失败回调 |
| [onReceive](on-receive.md) | [androidJvm]<br>abstract fun [onReceive](on-receive.md)()<br>发卡器响应命令等待回调 |
| [onSuccess](on-success.md) | [androidJvm]<br>abstract fun [onSuccess](on-success.md)(result: [T](index.md))<br>操作成功回调 |
