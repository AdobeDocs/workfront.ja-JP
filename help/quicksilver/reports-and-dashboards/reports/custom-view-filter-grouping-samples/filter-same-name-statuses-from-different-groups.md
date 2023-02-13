---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''フィルター：異なるグループの'
description: 3 文字のキー NST を使用して、タスク・ステータスを Group A に割り当て、New Status という名前を付けることができます。 3 文字のキー NES を持つ New Status という名前の別のタスクステータスがグループ B に割り当てられている可能性があります。 2 つのステータスの名前は同じにすることができますが、3 文字のコードは常に一意です。 グループステータスの詳細については、「グループステータスを作成または編集する」を参照してください。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# フィルター：ステータスが異なるグループに関連付けられている場合は、同じ名前のステータスで項目を表示

次の名前のグループ A にタスクステータスを割り当てることができます *新しいステータス* 3 文字の鍵で *NST*. 別のタスクステータスがグループ B に割り当てられていて、グループ B にも *新しいステータス* 3 文字の鍵で *NES.* 2 つのステータスの名前は同じにすることができますが、3 文字のコードは常に一意です。\
グループのステータスについて詳しくは、 [グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

フィルタービルダーを使用すると、同じ名前の 2 つのステータスを識別できません。 2 つのステータスを区別するには、テキストモードを使用する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ステータスが異なるグループに関連付けられている場合は、同じ名前のステータスでアイテムを表示

1. 例えば、タスクのリスト用にカスタマイズするフィルターに移動します。\
   これは、プロジェクトや問題でも同じように機能します。
1. クリック **フィルタールールを追加** の **ステータス** リストのオブジェクトのフィールド。\
   例えば、タスクレポートで、 **ステータスが新しいステータスと等しい**&#x200B;ステータスが「 **新しいステータス**.

   >[!TIP]
   >
   >「新規ステータス」という名前のステータスに対するオプションは 1 つだけです。

1. クリック **テキストモードに切り替え**.\
   次のコードが表示されます。

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >ここに表示されるステータスは 1 つだけです。 ステータス行には、いずれかのステータスの 3 文字のキーの 1 つが表示されます。

1. 次の 2 行のコードを追加して、フィルターにないステータスを追加します。

   <pre>または:1:status=NES<br>または:1:status_Mod=in</pre>

1. クリック **完了**&#x200B;を、 **フィルターを保存**.

   このリストには、グループ A のステータスが「新しいステータス」、グループ B のステータスが「新しいステータス」の両方のタスクが表示されます。
