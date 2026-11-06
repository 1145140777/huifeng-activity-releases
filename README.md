# huifeng-activity-releases

灰风助手「活动资源包」的发布区。

客户端从这里拉两样东西：

- 清单（签名信封）：`releases/latest/download/latest.json`
- 资源包：`releases/download/<tag>/activity-pack.zip`

## 为什么单独一个仓

活动资源包会频繁更新，跟 APK 的 Release 混在一起会互相干扰 `latest` 标记。

## 签名

清单是 `huifeng.activity-envelope@1` 信封，用 Ed25519 对 descriptor 的 UTF-8 原始字节签名。
公钥已内置在客户端（keyId `96189e3b87602d6b`）。私钥不在仓库里，也不在客户端里。