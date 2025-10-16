---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのタイムシートプロファイルの作成と管理
description: 管理しているグループをグループエリアで表示する場合、グループまたはそのいずれかのサブグループの管理者が管理アクセス権を持っているタイムシートプロファイルを表示し操作することができます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 87%

---

# グループのタイムシートプロファイルの作成と管理

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

管理しているグループをグループエリアで表示する場合、グループまたはそのいずれかのサブグループの管理者が管理アクセス権を持っているタイムシートプロファイルを表示し操作することができます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr>
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>グループのグループ管理者またはシステム管理者である必要があります。</p>
   <p>また、タイムシートには管理者アクセス権が必要です。</p></td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループレベルのタイムシートプロファイルを作成および編集

管理対象のグループで使用するタイムシートプロファイルを作成および編集できます。手順については、[タイムシートプロファイルの作成、編集および割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

## グループレベルのタイムシートプロファイルを削除

管理対象のグループで使用しているタイムシートプロファイルを削除できます。手順については、[タイムシートプロファイルの削除](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md)を参照してください。

## グループタイムシートを手動で生成

グループタイムシートプロファイルに加えた変更を現在のグループタイムシートに反映させるには、まず既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。手順については、[タイムシートの手動生成](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)で[タイムシートと時間エリアからのタイムシートの手動生成](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually)を参照してください。

グループタイムシートの削除については、[Adobe Workfront でのタイムシートの削除](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md)を参照してください。

## グループレベルのタイムシートプロファイルを書き出し

{{step-1-to-setup}}

1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. 書き出すタイムシートプロファイルを持っているグループの名前をクリックします。
1. 「**定期タイムシート**」をクリックします。
1. 「**書き出し**」をクリックして、グループのタイムシートプロファイルのリストを書き出します。
