---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートを手動で生成
description: タイムシートプロファイルに対して行った変更を現在のタイムシートに反映させるには、最初に既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。 この記事で説明するように、[ タイムシート ] 領域または [ セットアップ ] の [ 診断 ] 領域から、手動でタイムシートを生成できます。
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# タイムシートを手動で生成

タイムシートプロファイルに対して行った変更を現在のタイムシートに反映させるには、最初に既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。 この記事で説明するように、[ タイムシート ] 領域または [ セットアップ ] の [ 診断 ] 領域から、手動でタイムシートを生成できます。

タイムシートの削除手順については、 [Adobe Workfrontのタイムシートを削除](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront管理者であるか、グループのタイムシートプロファイルを扱う場合は、グループ管理者 ( またはWorkfront管理者 ) である必要があります。 詳しくは、 <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>.</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 手動で生成したタイムシートに関する考慮事項

タイムシートを手動で生成する場合：

* ユーザーに関連付けられたタイムシートプロファイルに従って作成されます。 タイムシートプロファイルが関連付けられていないユーザーは、タイムシートを受け取りません。 
* 現在のタイムシートと従うタイムシートのみが生成されます。 Workfrontは、同じ期間に対して 2 つのタイムシートを生成しません。 特定の期間のタイムシートが既にある場合、手動プロセスを使用してタイムシートを生成する際に、別のタイムシートが生成されません。

## [ タイムシートと時間 ] 領域からタイムシートを手動で生成する

[ セットアップ ] の [ タイムシートと時間 ] 領域から、システムレベルまたはグループレベルのタイムシートを手動で生成できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. システム全体で使用中のタイムシートを生成する場合は、 **タイムシートと時間。**

   または

   特定のグループが使用するタイムシートを生成する場合は、 **グループ**&#x200B;をクリックし、グループの名前をクリックします。

1. クリック **タイムシートプロファイル**.
1. クリック **詳細**&#x200B;を、 **タイムシートの生成**.

   新しいタイムシートは、タイムシートプロファイルに関連付けられたユーザーに対して、最大 2 期間作成されます。

## [ 診断 ] 領域からシステムレベルのタイムシートを手動で生成する

[ セットアップ ] の [ 診断 ] 領域から、システムレベルのタイムシートを手動で生成できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **システム**&#x200B;を選択し、「 **診断**.

1. クリック **診断の実施**. 
1. クリック **タイムシートの生成**.
