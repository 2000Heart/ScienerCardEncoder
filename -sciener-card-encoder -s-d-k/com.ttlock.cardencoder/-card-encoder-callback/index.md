---
title: CardEncoderCallback
---
//[ScienerCardEncoder SDK](../../../index.html)/[com.ttlock.cardencoder](../index.html)/[CardEncoderCallback](index.html)



# CardEncoderCallback

interface [CardEncoderCallback](index.html)&lt;[T](index.html)&gt;

统一的卡片编码器回调接口



#### Parameters


androidJvm

| | |
|---|---|
| T | 返回数据的类型 |



## Functions


| Name | Summary |
|---|---|
| [onFailure](on-failure.html) | [androidJvm]<br>abstract fun [onFailure](on-failure.html)(error: [CardEncoderException](../-card-encoder-exception/index.html))<br>操作失败回调 |
| [onSuccess](on-success.html) | [androidJvm]<br>abstract fun [onSuccess](on-success.html)(result: [T](index.html))<br>操作成功回调 |

