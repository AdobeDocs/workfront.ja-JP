---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: グループステータスの並べ替え
description: グループ管理者は、管理するグループのプロジェクト、タスク、および問題のステータスの順序を変更できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 6%

---

# グループステータスの並べ替え

グループ管理者は、管理するグループのプロジェクト、タスク、および問題のステータスの順序を変更できます。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>* Workfront管理者は、ステータスをシステムレベルで並べ替えることができます。 グループ内のステータスの順序は変わりません。
>
>  ただし、新しく作成されたトップレベルグループ内のステータスは、システムレベルのステータスの順序を継承します。 （新しいサブグループは、1 レベル上のグループ内のステータスの順序を継承します）。
>
>* ロックされたステータスは並べ替えることができます。 ロックされたステータスについて詳しくは、 [グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan* </td> 
   <td>任意</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

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
   <th width="33.33%">問題</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>現在</p> 
     <p>停止</p> 
     <p> 保留中 </p> 
     <p> 計画 </p> 
     <p> 完了 </p> 
     <p> 要求済み </p> 
     <p> 承認済み </p> 
     <p> 拒否 </p> 
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

## 管理するグループ内のタスクおよびプロジェクトのステータスを並べ替える

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ**&#x200B;をクリックし、グループの名前をクリックします。
1. 左側のパネルで、 **ステータス**.
1. 表示されるステータスリストの上にある **プロジェクト** または **タスク** タブをクリックします。

1. ステータスを目的の順序でドラッグ&amp;ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序をテストするには、グループに関連付けられたタスクまたはプロジェクトに移動し、右上隅のステータスをクリックして、表示されるステータスが設定した順序であることを確認します。

## 問題のステータスを並べ替え

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ**&#x200B;をクリックし、グループの名前をクリックします。
1. 左側のパネルで、 **ステータス**.
1. 次をクリック： **問題** タブをクリックします。
1. （オプション）問題のタイプ (**バグレポート**, **変更管理**, **問題**&#x200B;または **リクエスト**) をクリックします。

   >[!NOTE]
   >
   >* マスター・リストのステータスの順序はカスタマイズできません。
   >* 各イシューのタイプについては、同じ方法でステータスの順序を指定することをお勧めします。 問題のタイプについて詳しくは、 [リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. ステータスを目的の順序でドラッグ&amp;ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序をテストするには、グループに関連付けられている問題に移動し、右上隅の「 」ステータスをクリックして、表示されるステータスが設定した順序であることを確認します。
