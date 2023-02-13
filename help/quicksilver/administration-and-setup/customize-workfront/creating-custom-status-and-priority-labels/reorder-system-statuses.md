---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: システムレベルとグループのステータスの並べ替え
description: Workfrontの管理者は、システム内の全員または 1 つのグループの全員に対して、プロジェクト、タスクおよび問題のステータスの順序を変更できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# システムレベルとグループのステータスの並べ替え

Workfrontの管理者は、システム内の全員または 1 つのグループの全員に対して、プロジェクト、タスクおよび問題のステータスの順序を変更できます。

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* システムレベルでステータスを並べ替えても、グループ内のステータスの順序には影響しません。
>
>  ただし、新しく作成されたトップレベルグループ内のステータスは、システムレベルのステータスの順序を継承します。 （新しいサブグループは、1 レベル上のグループ内のステータスの順序を継承します）。
>
>* ロックされたステータスは並べ替えることができます。 ロックされたステータスについて詳しくは、 [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* グループ管理者は、グループで使用されているステータスを並べ替えることもできます。 詳しくは、 [グループステータスの並べ替え](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
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
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>Workfront管理者である。 Workfront管理者について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
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
    <ul> 
     <li>現在</li> 
     <li>停止</li> 
     <li> 保留中 </li> 
     <li> 計画 </li> 
     <li> 完了 </li> 
     <li> 要求済み </li> 
     <li> 承認済み </li> 
     <li> 拒否 </li> 
     <li> アイデア </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>新規</li> 
     <li>処理中</li> 
     <li>完了</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>新規</li> 
     <li>処理中</li> 
     <li>再オープン</li> 
     <li>フィードバック待ち</li> 
     <li>保留中</li> 
     <li>複製不可</li> 
     <li>クローズ</li> 
     <li>解決済み</li> 
     <li>完了確認</li> 
     <li>解決されない</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## タスクやプロジェクトのステータスをシステム全体またはグループ全体で並べ替える

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **プロジェクト環境設定/ステータス**.
1. （条件付き）グループのステータスを並べ替える場合は、右上隅のボックスにグループの名前を入力し、表示されたら名前をクリックします。

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. 表示されるステータスリストの上にある **プロジェクト** または **タスク** タブをクリックします。

1. ステータスを目的の順序でドラッグ&amp;ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序をテストするには、タスクまたはプロジェクトに移動し、右上隅にあるステータスをクリックして、表示されるステータスが設定した順序になっていることを確認します。

## 問題のステータスを並べ替え

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **プロジェクト環境設定/ステータス**
1. （条件付き）グループのステータスを並べ替える場合は、右上隅のボックスにグループの名前を入力し、表示されたら名前をクリックします。

   ![](assets/issue-statuses-group-name.png)

1. 次をクリック： **問題** タブをクリックします。
1. （オプション）問題のタイプ (**バグレポート**, **変更管理**, **問題**&#x200B;または **リクエスト**) をクリックします。

   >[!NOTE]
   >
   >* マスター・リストのステータスの順序はカスタマイズできません。
   >* 各イシューのタイプについては、同じ方法でステータスの順序を指定することをお勧めします。 問題のタイプについて詳しくは、 [リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. ステータスを目的の順序でドラッグ&amp;ドロップします。

   新しいステータスの順序は自動的に保存されます。

1. 新しいステータスの順序をテストするには、問題に移動し、右上隅のステータスをクリックして、表示されるステータスが設定した順序になっていることを確認します。
