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
TQID: https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
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
source-git-commit: 3b3d455ded251b06084249cf9df12c1f112f05e9
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 6%
---
# Adobe Workfront Planning でリクエストフォームへの承認の追加

<!--update the metadata with real information when making this available in TOC and in the left nav-->


<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。 すべてのユーザーのプレビュー環境でのみ使用できます。 リリースからプレビューの後、高速リリースを有効にしたお客様は、同じ機能を毎月実稼動環境でも使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

Adobe Workfront Planning リクエストフォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストの承認を開始できます。

<!--<span class="preview">Multiple stages are supported in the approval process. When all required decisions in a stage are made, the next stage begins and the new stage's approvers receive an email notification.</span>-->

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
* <span class="preview">承認に1つ以上のステージを追加できます。</span>

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

1. <span class="preview"> （オプション）「**ステージを追加**」をクリックして、承認に別のステージを追加します。</span>

1. **保存**&#x200B;をクリックして、承認ルールを保存します。

1. <span class="preview"> （オプション）承認にさらにステージを追加するには、次の操作を行います。</span>

   1. <span class="preview"> クリック **ステージを追加**.</span>

      <span class="preview">複数段階の承認&#x200B;**ボックスが表示されます。**&#x200B;既に既定の承認アクションを作成している場合、これらの承認者は自動的にステージ 1に追加されます。</span>

   1. <span class="preview"> 「**ユーザーまたはチームを追加**」フィールドに、少なくとも1人のユーザーまたはチームを追加して、ステージの承認者として設定します。</span>
   1. <span class="preview"> （条件付き、オプション）承認者のいずれかがレコードを承認した後、レコードを次のステージに進める場合は、「**1つの決定のみが必要です**」チェックボックスをオンにします。 そうでない場合、すべての承認者は、リクエストが次のステージに移動する前に、承認を決定する必要があります。</span>
   1. <span class="preview"> 「**ステージを追加**」をクリックし、手順Bから繰り返して、承認にステージを追加します。</span>

      <span class="preview">2つ以上のステージが存在する場合は、**ドラッグ** アイコン ![&#x200B; ドラッグ アイコン &#x200B;](assets/drag-icon.png)をクリックして、順番にドラッグ&amp;ドロップできます。</span>

      <span class="preview">このステージを削除&#x200B;**をクリックして承認からステージを削除するか、承認者の横にある**&#x200B;削除&#x200B;**アイコン ![削除アイコン &#x200B;](assets/delete.png)をクリックして、ステージの承認者リストからユーザーまたはチームを削除します。</span>**

      ![複数段階の承認ボックス &#x200B;](assets/planning-request-multi-stage-approval-box.png)

   1. <span class="preview">承認ワークフローの作成が完了したら、**保存**&#x200B;をクリックします。</span>

      <span class="preview">複数段階の承認は、承認ページから編集または削除できます。</span>

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