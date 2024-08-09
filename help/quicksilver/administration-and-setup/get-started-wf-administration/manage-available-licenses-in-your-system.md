---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: システムで使用可能なライセンスの管理
description: Adobe Workfront 管理者は、組織で購入したライセンスの数や現在使用しているライセンスの数など、Workfront アカウントに関する情報にアクセスできます。
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 87%

---

# システムで使用可能なライセンスの管理

<!-- Audited: 12/2023 -->

Adobe Workfront 管理者は、組織で購入したライセンスの数や現在使用しているライセンスの数など、Workfront アカウントに関する情報にアクセスできます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
    <p>新規：標準</p>
    <p>または</p>
    <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者またはグループ管理者である必要があります。 グループ管理者は、ライセンス情報に対する表示が制限されています。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

>[!NOTE]
>
>次のステートメントは、新しいプランにのみ適用されます。
>
>「プランを選択」で、次の手順を実行します。
>
>1. システム管理者がホーム グループの制限を設定できません。
>2. システム管理者は、すべてのホーム グループで使用されているライセンスの総数のみを表示できます。
>3. グループ管理者は、ライセンス ページにまったくアクセスできません。
>
>Prime プランと Ultimate プランの場合：
>
>1. システム管理者は、[Licenses] ページにホーム・グループを追加して、それらのグループ内のライセンスの使用状況を表示できます。また、ライセンス制限を設定することもできます。
>2. グループ管理者は、「ライセンス」ページにアクセスし、システム管理者によって「ライセンス」ページに追加されたライセンスを自分が管理するグループ内のライセンスの使用状況を表示できます。
>3. グループ管理者は、他のホーム グループの情報を表示したり、最大値を追加したりできません。

+++

## 組織のライセンスを表示

使用中のライセンス数は、Workfront に追加するユーザーにアクセスレベルを割り当てると、自動的に更新されます。詳しくは、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

システムのライセンス情報を表示するには：

{{step-1-to-setup}}

1. 左側のパネルの下部で、**システム**／**ライセンス**&#x200B;をクリックします。

   このページに記載されているライセンスについて詳しくは、[ライセンスの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)を参照してください。

   >[!NOTE]
   >
   >プルーフのライセンスは、Workfront ライセンスに加えて Workfront Proof アドオンを購入したお客様のみが利用できます。このアドオンについて詳しくは、[Workfront Proof：記事インデックス](../../workfront-proof/workfront-proof.md)を参照してください。

1. （条件付き）「**最大値を設定するには、ホームグループを追加する必要があります**」というメッセージが表示された場合は、システムにホームグループを追加します。詳しくは、この記事の[ライセンスページへのホームグループの追加または削除](#add-or-remove-a-home-group-to-the-licenses-page)の節を参照してください。

   >[!NOTE]
   >
   >新しいプランの場合、Select プランでは、管理者がホームグループ別のライセンス数を表示できません。使用中のライセンスの合計数のみを表示できます。Prime プランと Ultimate プランでは、ホームグループ別の最大ライセンス数を設定できます。

## Workfront アドオンのライセンスに関する情報の表示

組織で有料の Workfront Proof アドオンを使用している場合、使用中のライセンス数と使用可能なライセンス数が表示されます。例： **5/10 プルーフライセンス**&#x200B;は、組織が購入した 10 個の Workfront Proof ライセンスのうち 5 個を現在使用していることを示します。

![Workfront アドオンのライセンス](assets/updated-licenses-page.png)

組織が Workfront Goals を購入している場合は、その製品のライセンス情報もここに表示されます。この例では、次の情報を確認できます。

* 会社が購入した Workfront Goals ライセンスの合計数
* ユーザーに関連付けられている Workfront Goals ライセンスの数です。これは、アクセスレベルで Goals に対する表示アクセス権以上を付与されているユーザーの数です。

Workfront Goals について詳しくは、[Adobe Workfront Gloals の概要](../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。Workfront Goals へのアクセス権について詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

>[!NOTE]
>
>Workfront では、購入した Workfront Goals ライセンス以上を割り当てることができます。ただし、Workfront Goals の契約で許可されている数を超えるライセンスを割り当てると、Workfront のアカウントマネージャーから連絡があり、契約上の数を超えたことが通知されます。
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>管理アクセス権を持たないユーザーは、グループレポートを使用してライセンス数を表示できます。「レポート」タブで新しいグループレポートを作成し、次の列を追加します。
>
>* ライセンスタイプ制限：作業者制限
>* ライセンスタイプ制限：計画担当者制限
>
>レポートの作成について詳しくは、[カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

## 毎月のプルーフおよびドキュメントの決定の割り当てに関する情報の表示

>[!IMPORTANT]
>
>プルーフとドキュメントの決定の制限は、新しいライセンスのユーザーにのみ適用されます。詳しくは、[新しいライセンスの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)を参照してください。

プルーフおよびドキュメントの決定は、すべての無償 Workfront ライセンスで制限されています。制限は、毎月ユーザーごとにリセットされます。

各ライセンスの決定制限は、使用するプランによって異なります。毎月の割り当ては、設定／ライセンスで確認できます。

プルーフとドキュメントの決定の制限について詳しくは、[無償ユーザーに対する限定的なドキュメントおよびプルーフの決定の概要](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)を参照してください。

![毎月の決定割り当て](assets/monthly-decision-allotment.png)

## ライセンスページへのホームグループの追加または削除 {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

各ユーザーは、1 つのホームグループにのみ割り当てることができます。Workfront では、各ホームグループに割り当てられ現在使用されているライセンスの数を計算することで、グループ指向のライセンス数を提供します。

ライセンスページに「**最大数を設定するには、ホーム グループを追加してください。**」というメッセージが表示された場合は、少なくとも 1 つのホームグループをライセンスページに追加する必要があります。

>[!IMPORTANT]
>
>* ホームグループでライセンスを効果的に管理するには、最大ライセンス数を更新する前に、ビジネスユニットに特定のホームグループを設定することをお勧めします。詳しくは、[ホームグループの概要](../../administration-and-setup/manage-groups/groups-overview/home-groups.md)を参照してください。
>* ホームグループとして追加できるのは最上位のグループのみで、サブグループは対象外です。ユーザーにサブグループがホームグループとして割り当てられている場合、ユーザーのライセンスは、そのサブグループの上の最上位グループのライセンス数に追加されます。
>

ホームグループをライセンスページに追加または削除するには、次の手順に従います。

{{step-1-to-setup}}

1. 左パネルの下部で、**システム**／**ライセンス**&#x200B;をクリックします。

1. 「**グループ リストの管理**」をクリックします。
1. 最上位グループの名前を「**ホームグループ**」ボックスに入力していきます。
1. グループを追加するには、その名前が表示されたらクリックします。

   または

   グループを削除するには、名前の右にある「X」アイコンをクリックします。

1. 「**保存**」をクリックします。

Workfront 管理者は、ホームグループの最大ライセンス数を設定して、あるビジネスユニットが他のビジネスユニット用に購入された Workfront ライセンスを使用するのを防止できます。その手順については、[ホームグループの最大ライセンス数の設定](#set-the-maximum-license-count-for-a-home-group)を参照してください。

## ホームグループの最大ライセンス数の設定 {#set-the-maximum-license-count-for-a-home-group}

Workfront 管理者は、システムの最上位ホームグループに対して最大ライセンス数を設定できます。これにより、あるビジネスユニットが組織内の他のビジネスユニット用に購入された Workfront ライセンスを使用するのを防止できます。

デフォルトでは、最大ライセンス数は「N/A」に設定されています。これは、制限がないことを意味します。

グループ管理者は、担当するホームグループに割り当てられ使用されているライセンスの数を表示できます。詳しくは、[グループ内で割り当ておよび使用されているライセンス数の表示](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)を参照してください。

ホームグループの最大ライセンス数を設定するには、次の手順に従います。

{{step-1-to-setup}}

1. 左パネルの下部で、**システム**／**ライセンス**&#x200B;をクリックします。

1. リスト内でホームグループを探します。
1. グループの&#x200B;**最大**&#x200B;列で、最大値を設定する値をクリックします。
1. 最大値を入力し、Enter キーを押します。

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >グループの最大ライセンス値をデフォルトに戻すには、0 を入力しないでください。代わりに、ボックス内の数値を削除します。最大ライセンス値を 0 に設定すると、そのグループに割り当てられたライセンスがないことを示します。
