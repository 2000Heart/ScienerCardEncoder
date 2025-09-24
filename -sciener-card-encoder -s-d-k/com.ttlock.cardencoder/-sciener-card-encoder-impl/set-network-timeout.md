//[ScienerCardEncoder SDK](../../../index.md)/[com.ttlock.cardencoder](../index.md)/[ScienerCardEncoderImpl](index.md)/[setNetworkTimeout](set-network-timeout.md)

# setNetworkTimeout

[androidJvm]\
open override fun [setNetworkTimeout](set-network-timeout.md)(timeout: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin-stdlib/kotlin/-int/index.html))

设置网络超时时间

配置网络请求的超时时间，防止网络请求长时间无响应。 建议设置为5-30秒之间。

#### Parameters

androidJvm

| | |
|---|---|
| timeout | 超时时间，单位毫秒，建议范围：5000-30000ms |

#### See also

| | |
|---|---|
| [ScienerCardEncoderImpl.getNetworkTimeout](get-network-timeout.md) | 获取当前超时时间方法 |

#### Samples
