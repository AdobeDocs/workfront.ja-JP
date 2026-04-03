---
title: プロジェクトへのアクセス権の付与
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront でユーザーのプロジェクトへのアクセス権を定義できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 82%

---

# プロジェクトへのアクセスを許可

<!-- Audited: 12/2023 -->

Adobe Workfront 管理者は、アクセスレベルを使用して、プロジェクトに対するユーザーのアクセス権を定義できます。詳しくは、次の記事を参照してください。

* [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [新規アクセスレベルの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

カスタムアクセスレベルを使用して、Workfront の他のオブジェクトタイプへのユーザーのアクセスを管理する方法について詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
    <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>プラン</p>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムアクセスレベルを使用してプロジェクトへのユーザーのアクセス権を設定

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. プロジェクトの右側にある![表示](assets/gear-icon-settings.png)または&#x200B;**編集** ボタンの歯車アイコン **歯車設定アイコン**&#x200B;をクリックし、**設定を微調整**&#x200B;で付与する機能を選択します。

   ![&#x200B; プロジェクトのコピーの設定を微調整](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* 作業ライセンスを持つユーザーは、限られたプロジェクト権限を持ちます。プロジェクトに参加することはできますが、管理はできません。
   >* レビューライセンスを持つユーザーは、変換されたイシューからのプロジェクトに対する表示権限を持ちますが、その表示権限は制限されています。
   >* ユーザーが他のユーザーとプロジェクトを共有する際に付与できる権限について詳しくは、[Adobe Workfront でのプロジェクトの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。
   >* 特定の種類のオブジェクトに対してアクセスレベルの設定を行う場合、その設定は、低いランクのオブジェクトに対するユーザーのアクセスには影響しません。例えば、ユーザーのアクセスレベルでユーザーによるプロジェクトの削除を制限できますが、プロジェクトよりも下位にあるタスクの削除は制限されません。オブジェクトの階層について詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の記事にある[オブジェクトの相互依存性と階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)の節を参照してください。
   >* アクセス レベルが財務データへのアクセスを許可していないユーザーは、他のユーザーが財務データを表示できるようにするアクセスを許可できません。 これには、財務データを表示するプロジェクトへのアクセス権を与えたり、財務データを表示できるようにアクセスレベルを変更したりすることが含まれます。


1. （オプション）「作成」オプションの右側にある&#x200B;**共有のデフォルトを設定**&#x200B;をクリックし、続いて&#x200B;**ルールを追加**&#x200B;をクリックして、新しいプロジェクト用の共有ルールを追加します。

   このアクセスレベルのユーザーがプロジェクトを作成すると、プロジェクトが左側のメニューで選択したユーザーと自動的に共有されます。

   ![](assets/project-sharing-menu.png)

   右側のメニューで、プロジェクトをこれらのユーザーと共有する方法を指定します。

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >このアクセスレベルのユーザーがプロジェクトアクセステンプレートを使用している場合、テンプレートはアクセスレベルの共有設定を上書きします。プロジェクトアクセステンプレートについて詳しくは、[Adobe Workfront でのプロジェクトの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

   この手順を繰り返すことにより、アクセスレベルに必要な数のプロジェクト共有ルールを追加できます。

1. X をクリックして、**設定を微調整**&#x200B;ボックスを閉じます。
1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ライセンスタイプ別プロジェクトへのアクセス

各アクセスレベルのユーザーがプロジェクトで実行できる処理について詳しくは、記事[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects)の「[&#x200B; プロジェクト &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)」の節を参照してください。

## 共有プロジェクトへのアクセス権

イシューの所有者または作成者として、[Adobe Workfront でのプロジェクトの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)の説明に従って、イシューに対する権限を付与することで、他のユーザーとイシューを共有できます。

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つ項目の組み合わせによって決まります。

* オブジェクトについて受信者に付与する権限
* オブジェクトのタイプについての受信者のアクセスレベル設定
