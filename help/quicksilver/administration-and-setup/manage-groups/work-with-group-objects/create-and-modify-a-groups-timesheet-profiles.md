---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのタイムシートプロファイルの作成と管理
description: 管理しているグループをグループエリアで表示する場合、グループまたはそのいずれかのサブグループの管理者が管理アクセス権を持っているタイムシートプロファイルを表示し操作することができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: ht
source-wordcount: '412'
ht-degree: 100%

---

# グループのタイムシートプロファイルの作成と管理

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

管理しているグループをグループエリアで表示する場合、グループまたはそのいずれかのサブグループの管理者が管理アクセス権を持っているタイムシートプロファイルを表示し操作することができます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>グループのグループ管理者である必要があります。</p>  <p>また、タイムシートに対する管理アクセス権も必要です。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">ユーザーへの特定エリアに対する管理アクセス権の付与</a>を参照してください。</p>  <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## グループレベルのタイムシートプロファイルを作成および編集

管理対象のグループで使用するタイムシートプロファイルを作成および編集できます。手順については、[タイムシートプロファイルの作成、編集および割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

## グループレベルのタイムシートプロファイルを削除

管理対象のグループで使用しているタイムシートプロファイルを削除できます。手順については、[タイムシートプロファイルの削除](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md)を参照してください。

## グループタイムシートを手動で生成

グループタイムシートプロファイルに加えた変更を現在のグループタイムシートに反映させるには、まず既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。手順については、[タイムシートの手動生成](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)で[タイムシートと時間エリアからのタイムシートの手動生成](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually)を参照してください。

グループタイムシートの削除については、[Adobe Workfront でのタイムシートの削除](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md)を参照してください。

## グループレベルのタイムシートプロファイルを書き出し

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、**設定**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。
1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. 書き出すタイムシートプロファイルを持っているグループの名前をクリックします。
1. 「**定期タイムシート**」をクリックします。
1. 「**書き出し**」をクリックして、グループのタイムシートプロファイルのリストを書き出します。
