# AmazonEC2におけるIAMロールの動作

## クレデンシャル称号順番
1. 環境変数
2. システムファイル
3. IAMロール

## IAMロールの実際
インスタンスメタデータにKeyがある.

```
curl http://169.254.169.254/latest/meta-data/iam/security-credentials/cmn-sand-iamrole
```

## 処理速度
t2.microにて, Jmeter 並列数2000までこなせる.
