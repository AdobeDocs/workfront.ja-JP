---
content-type: reference
navigation-topic: get-started-with-workfront
title: Workfrontに対する HIPAA 対応
description: Workfrontのお客様のうち、HIPAA で定義されているビジネスアソシエイトまたは対象エンティティ（その代わりにビジネスアソシエイトがAdobe Workfrontを提供するもの）は、次のガイドラインを使用してWorkfrontを HIPAA 対応として設定する必要があります。
feature: Get Started with Workfront
author: Courtney
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
source-git-commit: 15a703e2292883427e371603f77a99765ed9d00a
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Workfrontに対する HIPAA 対応

HIPAA で定義されているWorkfrontのお客様のうち、ビジネスアソシエイトまたは対象エンティティ（その代わりにビジネスアソシエイトがAdobe Workfrontを提供するもの）は、次のガイドラインを使用してWorkfrontを HIPAA 対応として設定する必要があります。


## パスワード要件

| **セキュリティ設定** | **何ですか？** | **要件** |
|----------------------|------------------|------------------|
| 契約のパスワード強度の最小値 | 契約パスワードの最小強度はどれくらいですか？ | 8 文字以上 |
| ユーザーパスワードのパスワード強度の最小値 | ユーザーのパスワードの最小強度はどれくらいですか？ | 次の 3 つのカテゴリの文字：<br>*大文字（ラテン アルファベット） <br>*小文字（ラテン アルファベット） <br>*基本 10 桁 <br>*英数字以外 |
| パスワードの期間 | パスワードを変更しないでおく期間はどのくらいですか。 | パスワードは少なくとも 90 日ごとに変更してください |
| パスワード履歴 | 過去のパスワードをどれくらい記憶および禁止する必要がありますか？ | 5 以上 |


## ログイン要件

| **セキュリティ設定** | **何ですか？** | **要件** |
|----------------------|------------------|------------------|
| ログイン エラーの最大数 | ログインの試行に失敗して、ユーザーがロックアウトされる原因は何件ですか？ | 5 分以内に 5 回まで試行。30 分後に再試行できます |
| SSO 検証エラーの最大数 | 失敗した SSO 検証でロックアウトが発生する回数 | 5 以下（SSO を使用しているお客様にのみ適用） |


## セッション要件

| **セキュリティ設定** | **何ですか？** | **要件** |
|----------------------|------------------|------------------|
| セッションタイムアウト | 非アクティブ状態がログアウトするまでの時間はどのくらいですか？ | 15 分以内 |

## お客様の責任

すべての従業員、代表者、担当者が、Workfrontとのデータの使用に関連して当事者間で締結されたライセンス契約またはサービス契約（該当する場合）の条件を認識し、理解していることを確認します。

特に、以下の責任と義務を精査し、伝達する必要がある。 

* お客様は、すべてのユーザーによるWorkfront サービスの使用に対して責任を負います。 

* お客様は、Workfrontへのアップロードが禁止されているデータ要素を含む、Adobeとの契約に関するすべての条件を遵守する必要があります。 

* ePHI を含むがこれに限定されない機密データは、顧客自身の責任でアップロードされます。  顧客は、すべての顧客データに対して常に責任を負います。 


## データ保護とコンプライアンス

>[!IMPORTANT]
>
>Workfrontは、電子医療記録（EHR）のリポジトリとなるようには設計されていません。 ePHI は、Adobeが書面により明示的に許可した場合にのみ処理できます。 

* ePHI にアクセスできる可能性のあるWorkfront データベースについては、**保存時の暗号化（EAR）** が有効になっていることを確認します。
   * Workfrontの購入に EAR が含まれていることを確認するには、アカウント担当者（AE）にお問い合わせください。
   * コンプライアンスに関する義務を果たすために、Workfrontからアクセス可能なシステム/データベースを設定します。
* ePHI が HIPAA に対応していない他のAdobe ソリューションに転送、リンク、共有されないようにします。
* Workfrontで処理された患者写真は、安全に保存され、一般にアクセスできないようにします。
