---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートの手動生成
description: タイムシートプロファイルに加えた変更を現在のタイムシートに反映させるようにするには、まず既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。この記事で説明するように、タイムシートエリアまたは設定の診断エリアから、手動でタイムシートを生成できます。
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: ht
source-wordcount: '450'
ht-degree: 100%

---

# タイムシートの手動生成

タイムシートプロファイルに加えた変更を現在のタイムシートに反映させるようにするには、まず既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。この記事で説明するように、タイムシートエリアまたは設定の診断エリアから、手動でタイムシートを生成できます。

タイムシートの削除手順については、[Adobe Workfrontのタイムシートを削除](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront 管理者であるか、グループのタイムシートプロファイルを扱う場合は、グループ管理者（または Workfront 管理者）である必要があります。詳しくは、<a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>を参照してください。</p> <p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 手動で生成したタイムシートに関する考慮事項

タイムシートを手動で生成する場合、以下の手順を実行します。

* これらは、ユーザーに関連付けられたタイムシートプロファイルに従って生成されます。タイムシートプロファイルが関連付けられていないユーザーは、タイムシートを受け取りません。 
* 現在のタイムシートとその後のタイムシートのみが生成されます。Workfront は、同じ期間に 2 つのタイムシートを生成しません。特定の期間のタイムシートが既にある場合、手動プロセスを使用してタイムシートを生成する際に、別のタイムシートは生成されません。

## タイムシートと時間エリアからタイムシートを手動で生成する

設定のタイムシートと時間エリアから、システムレベルまたはグループレベルのタイムシートを手動で生成できます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. システム全体で使用中のタイムシートを生成する場合は、「**タイムシートと時間**」をクリックします。

   または

   特定のグループが使用するタイムシートを生成する場合は、「**グループ**」をクリックし、グループの名前をクリックします。

1. 「**定期タイムシート**」をクリックします。
1. 「**その他**」をクリックして、「**タイムシートの生成**」をクリックします。

   新しいタイムシートは、タイムシートプロファイルに関連付けられたユーザーに対して、最大 2 期間作成されます。

## 診断エリアからシステムレベルのタイムシートを手動で生成する

設定の診断エリアから、システムレベルのタイムシートを手動で生成できます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 「**システム**」を展開し、「**診断**」をクリックします。

1. 「**診断を実施**」をクリックします。
1. 「**タイムシートの生成**」をクリックします。
