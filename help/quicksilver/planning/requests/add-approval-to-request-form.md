---
title: Adobe Workfront Planningのリクエストフォームへの承認の追加
description: Adobe Workfront Planning リクエストフォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストの承認を開始できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: c7c74fdba29c4c6d28d12447459c5903a34c7856
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 4%
---
# Adobe Workfront Planning でリクエストフォームへの承認の追加

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planning リクエストフォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストの承認を開始できます。

承認プロセスでは、複数の段階に対応しています。 ステージで必要なすべての意思決定が行われると、次のステージが開始され、新しいステージの承認者にメール通知が送信されます。

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
<ul> 
<li><p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p></li>
または
<li><p>スタンドアロン製品として購入された場合の任意のプランニング・パッケージ</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>計画標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>   
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

* 1人または複数の承認者（ユーザーまたはチーム）をリクエストフォームまたは承認ルールに追加できます。
* 承認ルールは、送信されたリクエスト内のフィールド値に基づいてリクエストをルーティングします（例：「キャンペーンタイプ」フィールドの異なる値に対して異なる承認者）。
* 作成したレコードの承認情報は、「承認者」フィールドと「承認日」フィールドで表示できます。 フィールドの作成を参照してください。
* すべての承認者が承認すると、リクエストフォームに関連付けられたレコードタイプのレコードが作成されます。
* 少なくとも1人の承認者が拒否した場合、レコードタイプのレコードは作成されません。代わりに、リクエストはWorkfrontのリクエスト領域に残ります。 （この点は、少し異なる文言で両方のセクションに表示されました。ここでは1つのステートメントとしてマージされます。）
* 複数の承認者が必要な場合は、「1つの決定のみが必要」オプションが有効になっていない限り、すべての承認者がリクエストを承認または却下する前に決定を下す必要があります。
* チームが承認者として設定されている場合、そのチームのひとりのメンバーから必要な決定はひとつだけです。
* 承認はオプションです。リクエストフォームに承認が添付されていない場合、Workfront Planningは送信時にすぐにレコードを作成します。
* 承認には、1つ以上のステージを追加できます。

## リクエストフォームへの承認ルールの追加

承認ルールは、送信されたリクエストのフィールド値に基づいて承認プロセスを定義します。

例えば、リクエストフォームに「Campaign type」フィールドがある場合、そのフィールドに「Digital」という値がある場合は1人に、そのフィールドに「Print」という値がある場合は別のユーザーにリクエストを送信するルールを作成できます。

リクエストフォームの承認ルールを設定するには：

1. 記事[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)のリクエストフォームの作成と管理の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. リクエストフォームが開いたら、**設定**&#x200B;をクリックします。

   「**設定**」タブが開きます。

1. 承認ルールの設定を開始するには、左側のパネルで&#x200B;**承認** ![承認アイコン &#x200B;](assets/approvals-icon-on-form.png)をクリックします。

1. （オプション）デフォルトの承認プロセスを設定する場合は、**デフォルトの承認ルール**&#x200B;領域の&#x200B;**承認者** フィールドに少なくとも1人のユーザーまたはチームを追加し、**デフォルトの承認者のいずれかが承認した後にレコードを作成する場合は、「1つの決定のみが必要です**」チェックボックスをクリックします。

   ![既定の承認ルール領域](assets/default-approvers.png)

1. （オプション）承認ルールの追加を開始します。 カスタム承認ルールごとに、次の操作を行います。

   1. 「**承認ルールを追加**」をクリックします。
   1. プレースホルダータイトル **名称未設定の承認ルール**&#x200B;をクリックし、承認ルールの名前を入力します。
   1. 「**フィールドを選択**」をクリックし、ルールをアクティブ化するフィールドを選択します。
   1. ルールの演算子を選択します。 演算子は、フィールドのタイプによって異なります。
   1. 選択した演算子に値が必要な場合は、プラスアイコンをクリックして1つ以上の値を追加します。
   1. （オプション）「**条件を追加**」をクリックして、さらに条件を追加し、手順C-Eに従って追加条件を設定して&#x200B;**And**&#x200B;または&#x200B;**Or** ステートメントで接続します。
   1. 承認ルールの&#x200B;**アクション**&#x200B;領域の&#x200B;**承認者** フィールドに、条件が満たされたときに承認者として設定するユーザーまたはチームを少なくとも1つ追加します。
   1. （条件付き、オプション）承認者のいずれかがレコードを承認した後にレコードを作成する場合は、「**1つの決定のみが必要です**」チェックボックスをオンにします。 そうでない場合、すべての承認者は、リクエストが承認または却下される前に、承認を決定する必要があります。

   >[!NOTE]
   >
   >   承認ルールを追加する際には、次の点を考慮してください。
   >
   >   * デフォルトのルールのみが設定されている場合、送信されたすべてのリクエストに適用されます。
   >   * カスタムルールが満たされた場合、デフォルトはリクエスト承認ワークフローに適用されません。 一致したカスタムルールのみが承認に適用され、デフォルトのルールは無視されます。
   >   * 複数のカスタムルールが満たされた場合、順序の最初のルールが適用されます。 この場合、デフォルトの承認は適用されません（存在する場合）。

1. （オプション）「**ステージを追加**」をクリックして、承認に別のステージを追加します。

1. **保存**&#x200B;をクリックして、承認ルールを保存します。

1. （オプション）承認にさらにステージを追加するには、次の操作を行います。

   1. 「**ステージを追加**」をクリックします。

      「**複数段階の承認**」ボックスが表示されます。 既にデフォルトの承認アクションを作成している場合、これらの承認者は自動的にステージ 1に追加されます。

   1. 「**ユーザーまたはチームを追加**」フィールドに、ステージの承認者として設定するユーザーまたはチームを少なくとも1つ追加します。
   1. （条件付き、オプション）承認者のいずれかがレコードを承認した後、レコードを次のステージに進める場合は、「**1つの決定のみが必要です**」チェックボックスをオンにします。 そうでない場合、リクエストが次のステージに移動する前に、すべての承認者が承認を決定する必要があります。
   1. 「**ステージを追加**」をクリックし、手順Bから繰り返して、さらにステージを承認に追加します。

      2つ以上のステージが存在する場合は、**ドラッグ** アイコン ![&#x200B; ドラッグアイコン &#x200B;](assets/drag-icon.png)をクリックして、順番にドラッグ&amp;ドロップできます。

      **このステージを削除**&#x200B;をクリックして承認からステージを削除するか、承認者の横にある&#x200B;**削除** アイコン ![削除アイコン &#x200B;](assets/delete.png)をクリックして、ステージの承認者リストからユーザーまたはチームを削除します。

      ![複数段階の承認ボックス &#x200B;](assets/planning-request-multi-stage-approval-box.png)

   1. 承認ワークフローの作成が完了したら、**保存**&#x200B;をクリックします。

      複数段階の承認は、「承認」ページで編集または削除できます。

1. （オプション） リクエストフォームを一度も共有したことがない場合は、**公開**&#x200B;をクリックします。



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