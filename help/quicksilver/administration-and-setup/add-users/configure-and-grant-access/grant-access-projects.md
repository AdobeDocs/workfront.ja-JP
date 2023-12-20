---
title: プロジェクトへのアクセス権の付与
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Adobe Workfront管理者は、アクセスレベルを使用して、Workfrontでユーザーのプロジェクトへのアクセスを定義できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: e47f5d06d0c7d72c171583b53b69f951e4e99afe
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# プロジェクトへのアクセス権の付与

<!-- Audited: 12/2023 -->

Adobe Workfront管理者は、次の記事で説明するように、アクセスレベルを使用して、ユーザーのプロジェクトへのアクセスを定義できます。
* [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [新しいアクセスレベルの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

カスタムアクセスレベルを使用して、Workfrontの他のオブジェクトタイプへのユーザーのアクセスを管理する方法について詳しくは、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
    <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>新規：標準 </p>
 <p>または</p> 
<p>現在：プラン </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>：まだアクセス権がない場合は、Workfront管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムアクセスレベルを使用してプロジェクトへのユーザーアクセスを設定する

1. アクセスレベルの作成または編集を開始します ( [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 歯車アイコンをクリックします。 ![](assets/gear-icon-settings.png) の **表示** または **編集** 「プロジェクト」の右側のボタンをクリックし、 **設定を微調整する**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* 作業用ライセンスを持つユーザーは、限られたプロジェクト権限を持ちます。 プロジェクトに投稿することはできますが、管理はできません。
   >* レビューライセンスを持つユーザーは、変換された問題のプロジェクトに対して表示権限を持ちますが、表示権限は制限されます。
   >* ユーザーが他のユーザーとプロジェクトを共有する際に付与できる権限について詳しくは、 [Adobe Workfrontでプロジェクトを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* 特定の種類のオブジェクトに対してアクセスレベルの設定を行う場合、その設定は、低いランクのオブジェクトに対するユーザーのアクセスには影響しません。 たとえば、ユーザーのアクセスレベルでプロジェクトの削除を制限できますが、プロジェクトより下位のタスクの削除は制限されません。オブジェクトの階層の詳細については、「 [オブジェクトの相互依存性と階層](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 記事内 [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （オプション）「 **共有のデフォルトを設定** 「作成」オプションの右側に移動し、 **ルールを追加** をクリックして、新しいプロジェクト用の共有ルールを追加します。

   このアクセスレベルのユーザーがプロジェクトを作成すると、左側のメニューで選択したユーザーとプロジェクトが自動的に共有されます。

   ![](assets/project-sharing-menu.png)

   右側のメニューで、プロジェクトをこれらのユーザーと共有する方法を指定します。

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >このアクセスレベルのユーザーがプロジェクトアクセステンプレートを使用している場合、テンプレートはアクセスレベルの共有設定を上書きします。 プロジェクトアクセステンプレートについて詳しくは、 [Adobe Workfrontでプロジェクトを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   この手順を繰り返して、アクセスレベルに必要な数のプロジェクト共有ルールを追加できます。

1. 「 X 」をクリックして「 」を閉じます。 **設定を微調整する** ボックス。
1. （オプション）作業中のアクセスレベルの他のオブジェクトや領域のアクセス設定を構成するには、 [Adobe Workfrontへのアクセスの設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)、例： [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) および [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完了したら、「 **保存**.

   アクセスレベルを作成したら、そのレベルをユーザーに割り当てることができます。 詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## ライセンスタイプ別のレポート、ダッシュボード、カレンダーへのアクセス

各アクセスレベルのユーザーが問題に対してどのような処理を行うかについて詳しくは、「 [プロジェクト](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) 記事内 [各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 共有プロジェクトへのアクセス

イシューの所有者または作成者として、イシューに対する権限を付与することで、他のユーザーと共有できます。詳しくは、 [Adobe Workfrontでプロジェクトを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つの組み合わせによって決まります。

* オブジェクトに対して受信者に付与する権限
* オブジェクトのタイプに関する受信者のアクセスレベル設定
