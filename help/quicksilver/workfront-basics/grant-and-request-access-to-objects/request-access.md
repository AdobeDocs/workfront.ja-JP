---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトへのアクセスをリクエスト
description: Adobe Workfront でのオブジェクトの表示は、そのタイプのオブジェクトに対するアクセス権と、個々のオブジェクトに対する権限によって異なります。
author: Courtney
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 63%

---

# オブジェクトへのアクセスをリクエスト

<!-- Audited: 4/2025 -->

Adobe Workfront でのオブジェクトの表示は、そのタイプのオブジェクトに対するアクセス権と、個々のオブジェクトに対する権限によって異なります。

>[!NOTE]
>
>この記事では、次のオブジェクトを除くすべてのオブジェクトに対する権限をリクエストする方法について説明します。
>
>* Adobe Workfront シナリオプランナー内のシナリオプランナープラン。 詳しくは、[&#x200B; シナリオプランナーのプランに対する権限のリクエスト &#x200B;](../../scenario-planner/request-access-to-plan.md) を参照してください。 追加のライセンスが必要です。
>
>* Workfront Planning のビューとワークスペース。 詳しくは、[Adobe Workfront Planning での共有権限の概要 &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md) を参照してください。 追加のライセンスが必要です。


Workfront 管理者は、アクセスレベルの特定のタイプのオブジェクトにアクセス権を設定します。詳しくは、[アクセスレベルと権限の連携方法](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

Workfront 内の特定のオブジェクトに権限が必要な場合は、そのオブジェクトへのアクセスをリクエストできます。Workfront管理者やオブジェクト所有者にメールを送ってニーズを説明するのではなく、Workfront内の追加のアクセス（権限）をリクエストできます。

他のユーザーがオブジェクトへのリンクを共有している場合は、オブジェクトへの初期アクセスをリクエストできます。または、既に表示権限を持っているオブジェクトへの追加アクセスをリクエストできます。 例えば、プロジェクトに表示権限があるものの、タスクを追加する必要がある場合です。 この場合、プロジェクトに投稿権限をリクエストできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>ワークまたはそれ以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>権限をリクエストするオブジェクトに対する表示アクセス以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 標準の共有ルールについて

次の標準共有ルールは、Workfront システムのデフォルトオプションで、自動的に有効になります。

* タスクまたはイシューに割り当てられたユーザーは、そのタスクまたはイシューに対する投稿アクセス権を持ちます。
* プロジェクト、ポートフォリオ、プログラムのマネージャーは、自分が所有するオブジェクトに対する管理アクセス権を持っています。
* 会話に含まれるユーザーは、会話が発生するオブジェクトに対して表示アクセス権を持っています。
* 承認者として割り当てられたユーザーは、承認を待機しているオブジェクトに対して表示アクセス権を持ちます。
* ダッシュボードを共有すると、ダッシュボード上のすべてのレポートも同じユーザーに対する同じアクセス権で共有されます。
* オブジェクトの所有者は、管理者が定義したオブジェクトへのアクセス権を超えて、そのオブジェクトへのアクセス権を拡張することはできません。

## アクセスを要求

現在アクセスできないオブジェクトに対する初期アクセスをリクエストしたり、アクセスが制限されたオブジェクトに対する追加アクセスをリクエストしたりできます。

* [初期アクセスをリクエスト](#request-initial-access)
* [追加アクセスをリクエスト](#request-additional-access)

### 初期アクセスのリクエスト  {#request-initial-access}

オブジェクトへのアクセス権をまだ持っていない場合に、リンクからそのオブジェクトに移動すると、情報を表示するアクセス権がないことを示す画面が表示されます。

オブジェクトへの初期アクセスをリクエストするには：

1. **アクセスをリクエスト** をクリックします。 **アクセスをリクエスト** ダイアログボックスが表示されます。

1. （条件付き）複数のユーザーが追加のアクセス権を付与するための適切なアクセス権を持っている場合、ユーザー名の横にドロップダウン矢印が表示されます。 ドロップダウンリストからアクセス要求を受信するユーザーを選択します。

   ドロップダウンリストには 10 人のユーザーのみが表示され、アルファベット順に表示されます。 このドロップダウンメニューに表示されるユーザーの順序について詳しくは、[「アクセスを要求」と「さらにアクセスを要求する」のドロップダウンメニューの階層](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus)を参照してください。

1. ドロップダウンリストから、リクエストするアクセスのタイプを選択します。
1. （オプション）「**P.S.**」フィールドに、追加のアクセス権が必要な理由に関するメモを入力します。

   ![&#x200B; アクセスをリクエストダイアログボックス &#x200B;](assets/request-access-to-project.png)

1. 「**アクセスの要求**」をクリックします。

<!--
If you do not have access level rights to an object and you try to access that object from a link, a screen is displayed informing you to contact the Workfront administrator.

For example, if you do not have portfolio access, but you were given a link to a portfolio, you would see the following message:  
![](assets/permission-request-initial2-350x96.png)
-->

### 追加アクセスをリクエスト {#request-additional-access}

既にアクセスが制限されているオブジェクトへの追加アクセスをリクエストするには、次の手順に従います。

1. 追加のアクセスをリクエストするオブジェクトに移動します。

1. プロジェクト名の右にある&#x200B;**その他**&#x200B;メニューをクリックして、「**さらにアクセスを要求する**」をクリックします。

   ![&#x200B; さらにアクセスを要求 &#x200B;](assets/more-menu-request-more-access.png)

1. （条件付き）複数のユーザーが追加のアクセス権を付与するための適切なアクセス権を持っている場合、ユーザー名の横にドロップダウン矢印が表示されます。 ドロップダウンリストからアクセス要求を受信するユーザーを選択します。

   ドロップダウンリストには 10 人のユーザーのみが表示され、アルファベット順に表示されます。 このドロップダウンメニューに表示されるユーザーの順序について詳しくは、[「アクセスを要求」および「さらにアクセスを要求する」ドロップダウンメニューの階層](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus)を参照してください。

1. ドロップダウンリストから、要求するアクセスレベルを選択します。
1. （オプション）「**P.S.**」フィールドに、追加のアクセス権が必要な理由に関するメモを入力します。

   ![&#x200B; アクセスをリクエストダイアログボックス &#x200B;](assets/request-access-to-project.png)

1. 「**アクセスの要求**」をクリックします。

## アクセスをリクエストおよび他のアクセスをリクエスト ドロップダウンメニューの階層 {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [「アクセスの要求」および「さらにアクセスを要求する」ドロップダウンメニューに表示されるユーザーの階層について](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [オブジェクトの所有者について](#understand-the-owner-of-an-object)

### 「アクセスを要求」および「さらにアクセスを要求する」ドロップダウンメニューに表示されるユーザーの階層について {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

オブジェクトに「アクセスをリクエスト」リストまたは「その他のアクセスをリクエスト」リストを入力する場合、Workfrontは、リクエストを行うユーザーにオブジェクトアクセスを付与できる様々なロールを果たす、最大 10 人のユーザーのリストを選択します。 結果のリストは、名前の昇順で並べ替えられます。

アクセスをリクエストまたは追加のアクセスをリクエスト ドロップダウンでのユーザーの順序は、次のルールによって決まります。

* リストの最初のユーザーは、オブジェクト「所有者」です。詳しくは、[オブジェクトの所有者について](#understand-the-owner-of-an-object)を参照してください。
* 次に、オブジェクトを個別に共有するユーザーがリストに入力されます。 これらのユーザーはアルファベット順にリストされます。
* さらに、チーム、グループまたは会社との共有を通じて必要なアクセス権を取得するユーザーがリストに入力されます。 これらのユーザーはアルファベット順にリストされます。
* このリストが空の場合、Workfront 管理者が追加され、常に誰かにアクセスを要求できるようになります。これらのユーザーはアルファベット順にリストされます。
* リスト内の各ユーザーは、オブジェクトへの要求されたアクセス権と、オブジェクトを共有するためのアクセス権を持っている必要があります。

### オブジェクトの所有者について {#understand-the-owner-of-an-object}

オブジェクトの所有者は、次のように定義されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>オブジェクト</strong> </th> 
   <th><strong>オブジェクトの所有者の定義</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プロジェクト</td> 
   <td>所有者は、プロジェクト所有者であるか、またはプロジェクト所有者が見つからない場合やプロジェクト所有者に必要なアクセス権がない場合は、親ポートフォリオの所有者です。 <p>プロジェクトの作成者とは異なる可能性があります。 </p></td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>所有者は、プライマリ担当者であるか、またはプライマリ担当者が見つからない場合やプライマリ担当者に必要なアクセス権がない場合は、タスクが存在するプロジェクトの所有者です（上記の定義を参照）。 <p>タスクの作成者とは異なるユーザーである可能性があります。 </p></td> 
  </tr> 
  <tr> 
   <td>イシュー</td> 
   <td> <p>所有者は、イシューのプライマリ連絡先であるか、またはイシューが見つからない場合や必要なアクセス権がない場合は、イシューが存在するプロジェクトの所有者です（上記の定義を参照）。 </p> <p>所有者とイシューの作成者とは異なる可能性があります。 </p> </td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>所有者はポートフォリオ所有者です。 <p>ポートフォリオの作成者と異なる可能性があります。 </p></td> 
  </tr> 
  <tr> 
   <td>ドキュメント</td> 
   <td>所有者は、ドキュメントの所有者（ドキュメントをアップロードしたユーザー）であるか、またはドキュメントが見つからない場合やドキュメントの所有者に必要なアクセス権がない場合は、ドキュメントが存在するオブジェクトの所有者です。</td> 
  </tr> 
  <tr> 
   <td>レポートとダッシュボード</td> 
   <td>所有者は、レポートまたはダッシュボードの作成者です。 </td> 
  </tr> 
  <tr> 
   <td>カレンダー</td> 
   <td>所有者は、カレンダーの作成者です。すべてのユーザーには、デフォルトでカレンダーが割り当てられています。ユーザーは、そのカレンダーの所有者と見なされます。 </td> 
  </tr> 
  <tr> 
   <td>フィルター、ビュー、グループ化</td> 
   <td>フィルター、ビューまたはグループの所有者は、作成者です。 </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>プラン</span> </td> 
   <td> <p><span>所有者は、計画の作成者です。</span> </p> <p>追加のライセンスが必要です。 </p> <p><span>Workfront シナリオプランナーについて詳しくは、</span><a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">シナリオプランナーの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Goals</td> 
   <td> <p>所有者は、所有者に指定されたユーザーです。目標の作成者とは異なる可能性があります。 </p> <p>追加のライセンスが必要です。 </p> <p>Workfront Goals について詳しくは、<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals の概要</a>を参照してください。 </p> </td> 
  </tr> 
 </tbody> 
</table>


