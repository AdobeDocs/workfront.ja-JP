---
product-area: projects
navigation-topic: create-projects
title: プロジェクトのリクエスト
description: プロジェクトの作業を開始する前に、プロジェクトの承認をリクエストできます。これにより、ステータスが「アイデア」のプロジェクトが作成されます。プロジェクトのビジネスケースを作成して、それを完了することで達成したい重要なポイントの概要を示し、経営陣に人件費と経費の予算を提示することをお勧めします。
author: Alina
feature: Work Management
exl-id: 6557a7a5-3d5e-476d-b834-007c9e120397
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: ht
source-wordcount: '501'
ht-degree: 100%

---

# プロジェクトのリクエスト

プロジェクトの作業を開始する前に、プロジェクトの承認をリクエストできます。これにより、ステータスが「アイデア」のプロジェクトが作成されます。プロジェクトのビジネスケースを作成して、それを完了することで達成したい重要なポイントの概要を示し、経営陣に人件費と経費の予算を提示することをお勧めします。

Adobe Workfront の次のエリアで新しいプロジェクトを追加する際に、プロジェクトをリクエストできます。

* プロジェクトエリアの場合
* ポートフォリオのプロジェクトエリアの場合
* プログラムのプロジェクトエリアの場合
* プロジェクトのグループのグループエリアで、グループ管理者の場合。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront ライセンス*</p> </td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。プロジェクトへのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>を参照してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトのリクエストを作成すると、プロジェクトに対する管理権限が自動的に付与されます。 </p> <p> プロジェクト権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>を参照してください。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## プロジェクトのリクエスト

1. 次のいずれかの操作を行います。

   * **メインメニュー** ![](assets/main-menu-icon.png)、**プロジェクト**&#x200B;の順にクリックしてから、「**新規プロジェクト**」を展開します。
   * ポートフォリオに移動し、「**新規プロジェクト**」を展開します。
   * プログラムに移動し、「**新規プロジェクト**」を展開します。
   * グループ管理者の場合は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。詳しくは、[グループのプロジェクトを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

1. 「**プロジェクトをリクエスト**」をクリックします。

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 次のいずれかの操作を行います。

   * ビジネスケースを定義する際に、プロジェクトを作成する場合と同じ手順に従います。（推奨）

     ビジネスケースの定義とプロジェクトのリクエストについて詳しくは、[プロジェクトのビジネスケースを作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

   * プロジェクトを最初から作成するか、テンプレートを使用して、ステータスを「**リクエスト済み**」に変更します。

     プロジェクトの作成について詳しくは、[プロジェクトを作成](../../../manage-work/projects/create-projects/create-project.md)または[テンプレートを使用してプロジェクトを作成](../../../manage-work/projects/create-projects/create-project-from-template.md)を参照してください。

   リクエストしたプロジェクトのステータスは「**リクエスト済み**」で、ポートフォリオに関連付けている場合は、ポートフォリオの「**リクエストされたプロジェクト**」タブに表示されます。ポートフォリオマネージャーは、レビューを行い、承認または拒否できるようになりました。この場合、プロジェクトのステータスは「**承認済み**」または「**却下**」に変わります。
