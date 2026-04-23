---
title: Adobe Workfront Planningのリクエストフォームへの承認の追加
description: Adobe Workfront Planning リクエストフォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストの承認を開始できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 5%

---

# Adobe Workfront Planning でリクエストフォームへの承認の追加

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planning リクエストフォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストの承認を開始できます。

この記事では、ワークスペース管理者が、レコードタイプに関連付けられたリクエストフォームに承認を追加する方法について説明します。

Workfront Planningでのリクエストフォームの作成について詳しくは、[Adobe Workfront Planningでのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)を参照してください。

レコードを作成するためのレコードタイプへのリクエストの送信について詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront計画リクエストの送信](/help/quicksilver/planning/requests/submit-requests.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfront パッケージと任意のPlanning パッケージ</p>
または
<p>任意のワークフローパッケージと任意のプランニングパッケージ</p>

<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースとレコードタイプ </a>に対する権限を管理 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## リクエストフォームへの承認の追加に関する考慮事項

* 1つのリクエストフォームに1人または複数の承認者を追加できます。 ユーザーとチームを承認者として追加できます。
* 「承認者」フィールドと「承認日」フィールドでリクエストフォームを送信して作成したレコードに承認情報を表示できます。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。
* 1つのリクエストフォームに複数の承認者を追加する場合、すべての承認者は、レコードをWorkfront Planningで作成する前にリクエストを受け入れる必要があります。
* すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプのレコードが作成されます。
* 少なくとも1人の承認者がリクエストを拒否し、他のすべての承認者がリクエストを承認した場合、Workfrontのリクエスト領域にリクエストが作成されますが、リクエストフォームに関連付けられたレコードタイプのレコードは作成されません。
* リクエストフォームへの承認の追加はオプションです。 Workfront Planningは、リクエストが送信されたときに、リクエストフォームが承認に関連付けられていない場合は、直ちにレコードを作成します。

<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->

## リクエストフォームへの承認ルールの追加

承認ルールは、送信されたリクエストのフィールド値に基づいて承認プロセスを定義します。

例えば、リクエストフォームに「Campaign type」フィールドがある場合、そのフィールドに「Digital」という値がある場合は1人に、そのフィールドに「Print」という値がある場合は別のユーザーにリクエストを送信するルールを作成できます。

承認ルールを追加する際には、次の点を考慮してください。

* 承認ルールには、1人または複数の承認者を追加できます。
* 少なくとも1人の承認者がリクエストを拒否すると、リクエストは拒否され、レコードは作成されません。 リクエストはWorkfrontのリクエスト領域に残ります。
* 複数の承認者を追加し、「1つの決定のみが必要」オプションが有効になっていない場合、リクエストが承認または却下される前に、すべての承認者が決定を下す必要があります。
* チームが承認者として設定されている場合、チームの1人のメンバーから1つの決定のみが必要です。

リクエストフォームの承認ルールを設定するには：

1. 記事[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)のリクエストフォームの作成と管理の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. リクエストフォームが開いたら、**設定**&#x200B;をクリックします。

   「**設定**」タブが開きます。

1. 承認ルールの設定を開始するには、左側のパネルで&#x200B;**承認** ![承認アイコン &#x200B;](assets/approvals-icon-on-form.png)をクリックします。

1. （オプション）デフォルトの承認プロセスを設定する場合は、**デフォルトの承認ルール**&#x200B;領域の&#x200B;**承認者** フィールドに少なくとも1人のユーザーまたはチームを追加し、**デフォルトの承認者のいずれかが承認した後にレコードを作成する場合は、「1つの決定のみが必要です**」チェックボックスをクリックします。

   ![既定の承認ルール領域](assets/default-approvers.png)

1. （オプション）承認ルールの追加を開始します。 カスタム承認ルールごとに、次の操作を行います。

   1. **承認ルールを追加**&#x200B;をクリックします
   1. プレースホルダータイトル **名称未設定の承認ルール**&#x200B;をクリックし、承認ルールの名前を入力します。
   1. 「**フィールドを選択**」をクリックし、ルールをアクティブ化するフィールドを選択します。
   1. ルールの演算子を選択します。 演算子は、フィールドのタイプによって異なります。
   1. 選択した演算子に値が必要な場合は、プラスアイコンをクリックして1つ以上の値を追加します。
   1. （オプション）「**条件を追加**」をクリックして、さらに条件を追加し、手順C-Eに従って追加条件を設定して&#x200B;**And**&#x200B;または&#x200B;**Or** ステートメントで接続します。
   1. 承認ルールの&#x200B;**アクション**&#x200B;領域の&#x200B;**承認者** フィールドに、条件が満たされたときに承認者で設定するユーザーまたはチームを少なくとも1つ追加します。
   1. （条件付き、オプション）承認者のいずれかがレコードを承認した後にレコードを作成する場合は、「**1つの決定のみが必要です**」チェックボックスをオンにします。 そうでない場合、すべての承認者は、リクエストが承認または却下される前に、承認を決定する必要があります。

   >[!NOTE]
   >
   >   承認ルールを追加する際には、次の点を考慮してください。
   >
   >   * デフォルトのルールのみが設定されている場合、送信されたすべてのリクエストに適用されます。
   >   * カスタムルールが満たされた場合、デフォルトはリクエスト承認ワークフローに適用されません。 一致したカスタムルールのみが承認に適用され、デフォルトのルールは無視されます。
   >   * 複数のカスタムルールが満たされた場合、順序の最初のルールが適用されます。 この場合、デフォルトの承認は適用されません（存在する場合）。

1. **保存**&#x200B;をクリックして、承認ルールを保存します。
1. （オプション） リクエストフォームを一度も共有したことがない場合は、**公開**&#x200B;をクリックします。
