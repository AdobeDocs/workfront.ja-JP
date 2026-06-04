---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI ツールは、指定されたパスワードで接続できません
description: Power BI ツールからData Connectにログインしようとすると、ログインエラーが表示されます。
author: Courtney
feature: Reports and Dashboards
exl-id: c3f2b4a9-0831-48f0-871b-486d09ae5ea4
TQID: https://experienceleague.adobe.com/Z4RrMAPGd3CCti-cQFiJ7hlf-h8-suXeuoYfzk-9aKo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 6%

---

# Power BI ツールは、指定されたパスワードに接続できません

## 問題

Power BI ツールからData Connectにサインインしようとすると、次のエラーが表示されます。

`Cannot connect from BI tool with provided password`

## 原因

JDBC接続を作成する場合、WorkfrontはData Connectの一時パスワードを提供します。

Power BIを介してData Connectにアクセスする前に、最初に提供された接続詳細を使用してログインし、一時パスワードを更新してからログインを進める必要があります。


## ソリューション

Workfrontで接続パスワードをリセットし、接続を編集ダイアログボックスに表示されたリンクを使用して新しいパスワードを作成します。

### Workfrontで接続パスワードをリセットする

1. Workfront/設定/システム/Data Connectに移動します。
1. リストから接続を検索して開きます。
1. 「**接続パスワードをリセット**」で、パスワードをリセットするかどうかを確認するチェックボックスをオンにします。
1. **接続パスワードのリセット**をクリックします。
   ![接続パスワードのリセット ](assets/reset-password.png)
1. 以下のセクションに進みます。

### 接続の新しいパスワードを作成

1. URLをコピーし、新しいブラウザータブに貼り付けます。
1. Workfrontで、Connection User nameとDefault Passwordをコピーして、新しいブラウザータブに貼り付けます。
   ![urlとデフォルトのパスワードをコピー](assets/link-password.png)
1. 「**ログイン**」をクリックします。
1. 新しいパスワードを入力し、**送信**&#x200B;をクリックします。
1. Power BI ツールに移動し、新しいパスワードでログインします。
