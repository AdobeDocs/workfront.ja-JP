---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: グループのステータスの並べ替え
description: グループ管理者は、管理するグループのプロジェクト、タスク、課題ステータスの順序を変更できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# グループのステータスの並べ替え

グループ管理者は、管理するグループのプロジェクト、タスク、課題ステータスの順序を変更できます。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>* Workfront 管理者は、システムレベルでステータスを並べ替えることができます。これは、グループ内のステータスの順序には影響しません。
>
>  ただし、新しく作成されたトップレベルグループ内のステータスは、システムレベルのステータスの順序を継承します。（新しいサブグループは、1 レベル上のグループ内のステータスの順序を継承します）。
>
>* ロックされたステータスは並べ替えることができます。ロックされたステータスについて詳しくは、[グループステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。
>

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン* </td> 
   <td>任意</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## デフォルトのステータス順序

デフォルトでは、ステータスは次の順序で表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">プロジェクト</th> 
   <th width="33.33%">タスク</th> 
   <th width="33.33%">イシュー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>現在</p> 
     <p>停止</p> 
     <p> 保留中 </p> 
     <p> プラン </p> 
     <p> 完了 </p> 
     <p> リクエスト日 </p> 
     <p> 承認済み </p> 
     <p> 却下 </p> 
     <p> アイデア </p> 
   </td> 
   <td> 
     <p>新規</p> 
     <p>処理中</p> 
     <p>完了</p> 
   </td> 
   <td> 
     <p>新規</p> 
     <p>処理中</p> 
     <p>再オープン</p> 
     <p>フィードバック待ち</p> 
     <p>保留中</p> 
     <p>複製不可</p> 
     <p>クローズ</p> 
     <p>解決済み</p> 
     <p>完了確認</p> 
     <p>解決されない</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## 管理するグループ内のタスクとプロジェクトのステータスを並べ替える

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、**グループ**&#x200B;をクリックし、グループの名前を選択します。
1. 左側のパネルで、**ステータス**&#x200B;をクリックします。
1. 表示されるステータスリストの「**プロジェクト**」または「**タスク**」タブをクリックします。

1. ステータスを目的の順序でドラッグ＆ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序を調べるには、グループに関連付けられているタスクまたはプロジェクトに移動し、右上隅にあるステータスをクリックして、表示されるステータスが構成した順序に従っていることを確認します。

## イシューのステータスを並べ替える

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、**グループ**&#x200B;をクリックし、グループの名前を選択します。
1. 左側のパネルで、**ステータス**&#x200B;をクリックします。
1. 「**イシュー**」タブをクリックします。
1. （オプション）イシュータイプ（**バグレポート**、**変更依頼**、**イシュー**&#x200B;または **リクエスト**）を選択します。

   >[!NOTE]
   >
   >* メインリストのステータスの順序はカスタマイズできません。
   >* 各イシュータイプについては、同じ方法でステータスの順序を指定することをお勧めします。イシュータイプについて詳しくは、[リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)を参照してください。

1. ステータスを目的の順序でドラッグ＆ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序を調べるするには、グループに関連付けられているイシューに移動し、右上隅のステータスをクリックして、表示されるステータスが構成した順序に従っていることを確認します。
