---
title: グループに割り当てられ使用されているライセンスの数を表示します
description: Adobe Workfront 管理者は、現在グループおよびそのサブグループで使用されている個々のタイプのライセンスの数を表示できます。これは、ライセンスを再配布すべきかどうかを評価する必要がある場合に役立ちます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 88%

---

# グループで割り当てられて使用されているライセンス数を表示

Adobe Workfront 管理者は、現在グループおよびそのサブグループで使用されている個々のタイプのライセンスの数を表示できます。これは、ライセンスを再配布すべきかどうかを評価する必要がある場合に役立ちます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

>[!IMPORTANT]
>
>ユーザーのライセンスは、そのグループがユーザーのホームグループである場合にのみ、特定のグループでカウントされます。

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

## グループで使用されているライセンス数を表示

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![&#x200B; グループ &#x200B;](assets/groups-icon.png)」をクリックします。

1. グループの名前をクリックします。
1. 表示されるページの右上隅付近のヘッダー領域で、**使用中のライセンス**&#x200B;エリアの、現在使用中の&#x200B;**プラン**&#x200B;および&#x200B;**作業**&#x200B;ライセンスの数を見ます。

   最上位のグループが表示されていて、Workfront 管理者がグループの各ライセンスタイプの最大数を定義した場合は、その数も表示されます。例えば、以下のグループでは、プランライセンスを取得できるユーザーは最大 10 人で、作業ライセンスを取得できるユーザーは最大 15 人です。

   ![&#x200B; 割り当て済みライセンス &#x200B;](assets/licenses-used-allocated.png)

   Workfront 管理者がグループに割り当てるライセンスの最大数を定義する方法について詳しくは、記事[システムで使用可能なライセンスを管理](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)の[ホームグループに最大ライセンス数を設定](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set)を参照してください。

   >[!NOTE]
   >
   >対象のグループがサブグループの場合は、使用中のライセンスの数のみが表示され、グループに割り当てられたライセンスの最大数は表示されません。これは、Workfront 管理者がサブグループに対しては最大ライセンス数を定義していないためです。
   >
   >![&#x200B; サブグループ内の使用済みライセンス &#x200B;](assets/subgroup-used-licenses-only.png)
   >

1. グループで現在使用されているライセンスのタイプ（レビューやリクエストなど）別の数を表示するには、**使用中のライセンス**&#x200B;のすぐ下のテキスト領域をクリックします。

   ![&#x200B; クリックすると詳細が表示されます &#x200B;](assets/click-text-to-see-more.png)

   表示されるボックスには、プラン、作業、レビュー、リクエストの 4 つの Workfront ライセンスタイプすべてに対して同じ情報が表示されます。ボックスの下部には、このグループまたはそのサブグループの 1 つのメンバーが使用しているライセンスの総数が表示されます。

   ![&#x200B; その他のライセンス情報 &#x200B;](assets/more-license-info.png)

   レビューライセンスおよびリクエストライセンスについては、最大値列には常に無制限と表示されます。
