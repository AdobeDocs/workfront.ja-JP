---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: グループ状態の並べ替え
description: グループ管理者は、管理するグループのプロジェクト、タスク、課題ステータスの順序を変更できます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 94%

---

# グループのステータスの並べ替え

グループ管理者は、管理するグループのプロジェクト、タスク、課題ステータスの順序を変更できます。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![&#x200B; ステータス &#x200B;](assets/statuses.png)

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>* Workfront 管理者は、システムレベルでステータスを並べ替えることができます。これは、グループ内のステータスの順序には影響しません。
>
>  ただし、新しく作成されたトップレベルグループ内のステータスは、システムレベルのステータスの順序を継承します。（新しいサブグループは、1 レベル上のグループ内のステータスの順序を継承します）。
>
>* ロックされたステータスは並べ替えることができます。ロックされたステータスについて詳しくは、[グループステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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

{{step-1-to-setup}}

1. 左側のパネルで、**グループ**&#x200B;をクリックし、グループの名前を選択します。
1. 左側のパネルで、**ステータス**&#x200B;をクリックします。
1. 表示されるステータスリストの「**プロジェクト**」または「**タスク**」タブをクリックします。

1. ステータスを目的の順序でドラッグ＆ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序を調べるには、グループに関連付けられているタスクまたはプロジェクトに移動し、右上隅にあるステータスをクリックして、表示されるステータスが構成した順序に従っていることを確認します。

## イシューのステータスを並べ替える

{{step-1-to-setup}}

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
