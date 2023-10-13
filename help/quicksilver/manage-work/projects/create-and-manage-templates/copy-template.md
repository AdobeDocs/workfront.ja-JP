---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートのコピー
description: 新しいプロジェクトテンプレートを一から作成する代わりに、必要に応じて既存のテンプレートをコピーして変更することができます。
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# プロジェクトテンプレートのコピー

新しいプロジェクトテンプレートを一から作成する代わりに、必要に応じて既存のテンプレートをコピーして変更することができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>テンプレートへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>テンプレートに対する表示権限またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。


## テンプレートのコピーに関する考慮事項

次の項目は、常に既存のプロジェクトから新しいプロジェクトにコピーされます。

* テンプレート タスク
* テンプレートタスクのデフォルト情報 ( タスクのデフォルト承認プロセス、タスクのデフォルトカスタムForms)
* カスタムフォーム
* リスク
* キューの設定情報
* Portfolioとプログラム
* 承認
* ドキュメント
* 元のテンプレートタスクの日数が新しいテンプレートに転送されます。 必要に応じて、テンプレートの開始日または完了日を（スケジュールモードに応じて）変更して、テンプレートタスクの日を更新する必要があります。

次の項目は、既存のプロジェクトから新しいプロジェクトにコピーされません。

* 請求件の料率
* ユーザーコメント

## テンプレートのコピー

1. コピーするテンプレートに移動します。
1. 次をクリック： **その他** メニュー ![](assets/qs-more-icon-on-an-object.png)を選択し、次に **コピー**.
1. でテンプレートの名前を指定します。 **新規テンプレート名** フィールドに入力します。

   デフォルトでは、新しい名前はです。 **のコピー `<original template name>`.**

1. 必要に応じて、 **タスクとテンプレートに対するユーザー割り当てを保持する**：すべてのタスクおよびテンプレートの割り当てを元のテンプレートから新しいテンプレートに引き継ぐ場合は、このオプションを選択します。
1. クリック **保存** をクリックして、テンプレートのコピーを作成します。
