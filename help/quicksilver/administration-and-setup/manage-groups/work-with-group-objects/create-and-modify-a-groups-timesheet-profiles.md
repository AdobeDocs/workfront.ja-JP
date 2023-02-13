---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのタイムシートプロファイルを作成および管理する
description: '[ グループ ] 領域で管理するグループを表示している場合は、そのグループの管理者またはそのサブグループの 1 人が管理アクセス権を持つタイムシートプロファイルを表示し、操作できます。'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# グループのタイムシートプロファイルを作成および管理する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

[ グループ ] 領域で管理するグループを表示している場合は、そのグループの管理者またはそのサブグループの 1 人が管理アクセス権を持つタイムシートプロファイルを表示し、操作できます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>グループのグループ管理者である必要があります。</p>  <p>また、タイムシートに対する管理者アクセス権も持っている必要があります。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p>  <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## グループレベルのタイムシートプロファイルの作成と編集

管理するグループで使用するタイムシートプロファイルを作成および編集できます。 手順については、 [タイムシートプロファイルの作成、編集、割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## グループレベルのタイムシートプロファイルを削除

管理するグループが使用しているタイムシートプロファイルを削除できます。 手順については、 [タイムシートプロファイルを削除](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## グループタイムシートを手動で生成

現在のグループタイムシートに反映するように、タイムシートプロファイルのグループ化に対して行った変更を有効にするには、最初に既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。 手順については、 [[ タイムシートと時間 ] 領域からタイムシートを手動で生成する](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [タイムシートを手動で生成](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

グループタイムシートの削除の詳細については、 [Adobe Workfrontのタイムシートを削除](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## グループレベルのタイムシートプロファイルのエクスポート

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).
1. クリック **グループ**.

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. エクスポートするタイムシートプロファイルを含むグループの名前をクリックします。
1. クリック **タイムシートプロファイル**.
1. クリック **書き出し** グループのタイムシートプロファイルの一覧をエクスポートするには、次の手順を実行します。
