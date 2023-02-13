---
title: 割り当てられ、グループで使用されているライセンス数を表示
description: Adobe Workfrontの管理者は、現在グループおよびそのサブグループで使用されている個々の種類のライセンスの数を表示できます。 これは、ライセンスを再配布するかどうかを評価する必要がある場合に役立ちます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 割り当てられ、グループで使用されているライセンス数を表示

Adobe Workfrontの管理者は、現在グループおよびそのサブグループで使用されている個々の種類のライセンスの数を表示できます。 これは、ライセンスを再配布するかどうかを評価する必要がある場合に役立ちます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

>[!IMPORTANT]
>
>ユーザーのライセンスは、そのグループがユーザーのホームグループである場合にのみ、特定のグループでカウントされます。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfrontプラン</a>*</td> 
   <td> <p>チーム以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfrontライセンス</a>*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループで使用されているライセンス数の表示

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. グループの名前をクリックします。
1. 表示されるページで、右上隅付近のヘッダー領域に、 **使用中のライセンス** 数を確認する領域 **プラン** および **作業** 現在使用中のライセンスです。

   最上位のグループを表示し、Workfront管理者がグループの各ライセンスタイプの最大数を定義した場合は、これらの数も表示されます。 例えば、以下のグループでは、最大 10 人のユーザーが Plan ライセンスを取得し、15 人が Work ライセンスを取得できます。

   ![](assets/licenses-used-allocated.png)

   Workfront管理者がグループに割り当てるライセンスの最大数を定義する方法について詳しくは、 [ホームグループの最大ライセンス数を設定する](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) 記事内 [システムで使用可能なライセンスを管理](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >対象のグループがサブグループの場合、使用中のライセンスの数のみが表示され、グループに割り当てられたライセンスの最大数は表示されません。 これは、Workfront管理者がサブグループの最大ライセンス数を定義していないためです。
   >
   >![](assets/subgroup-used-licenses-only.png)

1. グループで現在使用されているライセンスの種類（「レビューとリクエスト」を含む）ごとに異なる数を表示するには、下のテキスト領域をクリックします **使用中のライセンス：**

   ![](assets/click-text-to-see-more.png)

   表示されるボックスには、次の 4 種類のWorkfrontライセンスの情報がすべて表示されます。計画、作業、レビュー、およびリクエスト。 ボックスの下部に、このグループまたはそのサブグループの 1 つのメンバーが使用しているライセンスの総数が表示されます。

   ![](assets/more-license-info.png)

   レビューおよびリクエストライセンスの場合、[ 最大値 ] 列には常に [ 無制限 ] と表示されます。
