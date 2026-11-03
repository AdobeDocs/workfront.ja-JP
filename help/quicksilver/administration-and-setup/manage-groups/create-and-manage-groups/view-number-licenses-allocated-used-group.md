---
title: グループ内で割り当てられ、使用されるライセンスの数を表示する
description: Adobe Workfront 管理者は、現在グループおよびそのサブグループで使用されている個々のタイプのライセンスの数を表示できます。 これは、ライセンスを再配布すべきかどうかを評価する必要がある場合に役立ちます。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
TQID: 'https://experienceleague.adobe.com/z7vh7rdkB40A2gzfSYddUAHF-nOGqVCgpVyu729gYgE'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: cb0f538ff392ebff585fbdeeba3729d9b2247292
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 56%
---
# グループで割り当てられて使用されているライセンス数を表示

Adobe Workfront 管理者は、現在グループおよびそのサブグループで使用されている個々のタイプのライセンスの数を表示できます。 これは、ライセンスを再配布すべきかどうかを評価する必要がある場合に役立ちます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront 管理者（すべてのグループ）も同様です。

>[!IMPORTANT]
>
>ユーザーのライセンスは、そのグループがユーザーのホームグループである場合にのみ、特定のグループでカウントされます。

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
   <td>グループのグループ管理者またはシステム管理者でなければなりません。</td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループで使用されているライセンス数を表示

{{step-1-to-setup}}

1. 左側のパネルで、**グループ** ![&#x200B; グループ &#x200B;](assets/groups-icon.png)をクリックします。

1. グループの名前をクリックします。
1. 右上隅付近のヘッダー領域に表示されるページで、**使用中のライセンス**&#x200B;領域を表示して、現在使用されているライセンスの数を確認します。

   Workfront パッケージに応じて、ライセンスは次のようになります。

   * **標準**&#x200B;および&#x200B;**光**
   * **プラン**&#x200B;および&#x200B;**作業**

   ![割り当てられたライセンス &#x200B;](assets/how-many-licenses-standard-light.png)

   トップレベルのグループを表示している場合、Workfront管理者がそのグループの各ライセンスタイプの最大数を定義すると、これらの数も比率として表示されます。 例えば、2/10は、使用可能な10個のライセンスのうち2個のライセンスが割り当てられていることを意味します。

   Workfront 管理者がグループに割り当てるライセンスの最大数を定義する方法について詳しくは、記事[システムで使用可能なライセンスを管理](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)の[ホームグループに最大ライセンス数を設定](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set)を参照してください。

   >[!NOTE]
   >
   >対象のグループがサブグループの場合は、使用中のライセンスの数のみが表示され、グループに割り当てられたライセンスの最大数は表示されません。 これは、Workfront 管理者がサブグループに対しては最大ライセンス数を定義していないためです。
   >

1. グループで現在使用されているライセンスの種類（レビューとリクエストを含む）ごとに個別のカウントを表示するには、使用中のライセンスを表示する領域をクリックします。

   表示されるボックスには、適用されるすべてのWorkfront ライセンスタイプに同じ情報が表示されます。 Workfrontのパッケージによって、次のような方法が異なります。

   * Standard、Light、Contributor、External
   * 計画、作業、レビュー、リクエスト

   ボックスの下部には、このグループのメンバーまたはそのサブグループの1人が使用しているライセンスの合計数が表示されます。

   レビューライセンスおよびリクエストライセンスについては、最大値列には常に無制限と表示されます。
