---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートのコピー
description: 新しいプロジェクトテンプレートを最初から作成するのではなく、必要に応じて既存のテンプレートをコピーし、それに変更を加えることができます。
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 83%

---

# プロジェクトテンプレートのコピー

新しいプロジェクトテンプレートを最初から作成するのではなく、必要に応じて既存のテンプレートをコピーし、それに変更を加えることができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>テンプレートへの編集アクセス</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートに対する表示権限またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。


## テンプレートのコピーに関する考慮事項

次の項目は、常に既存のプロジェクトから新しいプロジェクトにコピーされます。

* テンプレートタスク
* テンプレートタスクのデフォルト情報 ( タスクのデフォルト承認プロセス、タスクのデフォルトカスタムForms)
* カスタムフォーム
* リスク
* キューの設定情報
* ポートフォリオとプログラム
* 承認
* ドキュメント
* 元のテンプレートタスクの日数が新しいテンプレートに転送されます。 必要に応じて、テンプレートの開始日または完了日を（スケジュールモードに応じて）変更して、テンプレートタスクの日を更新する必要があります。

次の項目は、既存のプロジェクトから新規プロジェクトにコピーされません。

* 請求レート
* ユーザーコメント

## テンプレートをコピーする

1. コピーするテンプレートに移動します。
1. 「**その他**」メニュー![](assets/qs-more-icon-on-an-object.png)、「**コピー**」の順にクリックします。
1. 「**新しいテンプレート名**」フィールドにテンプレートの名前を指定します。

   デフォルトでは、新しい名前は **`<original template name>` のコピー**&#x200B;です。

1. **タスクとテンプレートのユーザー割り当てを保持する**&#x200B;かどうかを選択します。元のテンプレートから新しいテンプレートにすべてのタスクとテンプレートの割り当てを引き継ぐには、このオプションを選択します。
1. 「**保存**」をクリックしてテンプレートのコピーを作成します。
