---
product-area: projects
navigation-topic: create-projects
title: プロジェクトのリクエスト
description: プロジェクトの作業を開始する前に、プロジェクトの承認をリクエストできます。 これにより、ステータスが「アイデア」のプロジェクトが作成されます。 プロジェクトのビジネスケースを作成して、完了して達成する重要なポイントの一部を示し、管理者の人件費と費用予算について提示することをお勧めします。
author: Alina
feature: Work Management
exl-id: 6557a7a5-3d5e-476d-b834-007c9e120397
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 2%

---

# プロジェクトのリクエスト

プロジェクトの作業を開始する前に、プロジェクトの承認をリクエストできます。 これにより、ステータスが「アイデア」のプロジェクトが作成されます。 プロジェクトのビジネスケースを作成して、完了して達成する重要なポイントの一部を示し、管理者の人件費と費用予算について提示することをお勧めします。

Adobe Workfrontの次の領域で新しいプロジェクトを追加する際に、プロジェクトをリクエストできます。

* 「プロジェクト」領域
* Portfolioの「プロジェクト」領域
* プログラムの「プロジェクト」領域で
* プロジェクトのグループの「グループ」領域で、グループ管理者の場合に使用します。

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project request you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->


この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 プロジェクトへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトリクエストを作成すると、プロジェクトに対する管理権限が自動的に付与されます </p> <p> プロジェクト権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトのリクエスト

1. 次のいずれかの操作を行います。

   * 次をクリック： **メインメニュー** ![](assets/main-menu-icon.png)をクリックし、 **プロジェクト**&#x200B;を展開し、 **新規プロジェクト**.
   * ポートフォリオに移動し、を展開します。 **新規プロジェクト**.
   * プログラムに移動し、を展開します。 **新規プロジェクト**.
   * グループ管理者は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。 詳しくは、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. クリック **プロジェクトをリクエスト**.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 次のいずれかの操作を行います。

   * ビジネスケースを定義する際のプロジェクトの作成と同じ手順に従います。 （推奨）

      ビジネスケースの定義とプロジェクトのリクエストについては、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   * プロジェクトを最初から作成するか、テンプレートを使用して、ステータスを「 」に変更します。 **リクエスト**.

      プロジェクトの作成について詳しくは、 [プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md) または [テンプレートを使用したプロジェクトの作成](../../../manage-work/projects/create-projects/create-project-from-template.md).
   リクエストするプロジェクトのステータスは次のとおりです **リクエスト** そして、 **リクエストされたプロジェクト** タブに表示されます (Portfolioに関連付けている場合 )。Portfolio ポートフォリオマネージャは、レビューを行い、承認または拒否できるようになりました。この場合、プロジェクトのステータスは次のいずれかに変わります。 **承認済み** または **却下**.
