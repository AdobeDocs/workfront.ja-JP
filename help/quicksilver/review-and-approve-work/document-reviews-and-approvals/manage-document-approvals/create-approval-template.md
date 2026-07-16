---
product-area: documents
navigation-topic: approvals
title: ドキュメントの承認ワークフローテンプレートの作成
description: 承認テンプレートを作成すると、承認プロセスを効率化できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 684
ht-degree: 14%

---

# ドキュメントの承認ワークフローテンプレートの作成

Workfrontの設定領域で、標準ライセンスを持つユーザーは、再利用可能な承認テンプレートを作成できます。 作成した承認テンプレートは、オブジェクトの「ドキュメント」領域のアセットに適用できます。
>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。 標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>従来のWorkfrontストレージを使用して承認を管理する、あらゆるWorkfrontパッケージ</p>
<p>Adobeのクラウドストレージを使用して承認を管理する任意のワークフローパッケージ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>プラン</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
## Create an Approval Template in Production

{{step-1-to-setup}}

1. In the left panel, click **Review and Approval** > **Approval Templates**.
1. Click **New Template** on the right side of the page. 

1. Fill in the following details:

   <table>
     <tr>
   <td><strong>Template name</strong></td>
   <td>Add a template name. </td>
   </tr>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Workdays until due date</strong></td>
   <td>Choose how many workdays until the approval is due after a stage is activated.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)
    
1. Click **Save**.

Once the template is created, it can be applied to documents in the Documents area of an object to begin the formal review and approval process in Workfront.
-->

## 承認テンプレートの作成

承認テンプレートダイアログは、常に詳細設定モードで開きます。 テンプレートの基本モードはありません。 テンプレートには、最大30個の並列パスを設定でき、合計ステージ数は最大100個です。 各パスは独立して実行され、1つ以上のシーケンシャルステージを含めることができます。

承認テンプレートを作成するには：

{{step-1-to-setup}}

1. 左パネルで&#x200B;**レビューと承認**／**承認テンプレート**&#x200B;をクリックします。

1. ページの右側で「**新規テンプレート**」をクリックします。

1. **テンプレート名**&#x200B;を追加します。

1. パス 1のステージ 1の詳細を入力：

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージには、デフォルトで<em> ステージ 1</em>、<em> ステージ 2</em>などの名前が付けられます。 ステージの名前を、<em>初期審査</em>や<em>最終承認</em>などのより記述的な名前に変更します。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールの追加（オプション）</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 参加者はテンプレートではオプションです。 テンプレートをドキュメントに適用するときに追加できます。<p>注意：レビュアーまたは承認者は、同じアセットで一度に1つのオープンステージにのみ割り当てることができます。 複数の並行ステージが同時に開いている場合、同じ人物を複数に追加することはできません。</p></td>
   </tr>
   <tr>
   <td><strong>1つの決定のみが必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期日までの稼働日数（オプション）</strong></td>
   <td>ステージが開いてから完了するまでの作業日数を選択します。 各パスの最初のステージでは、絶対的な期日もサポートされます。 パスの後続の各ステージは、相対的な期日のみをサポートします。</td>
   </tr>
   <tr>
   <td><strong>カスタムメッセージの追加（オプション）</strong></td>
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。 テンプレートがドキュメントに適用されると、そのメッセージは承認電子メール通知およびWorkfrontの「承認」タブに表示されます。<p>2番目のステージを追加すると、<strong>すべてのステージでこのメッセージを表示</strong>がデフォルトで選択されます。 各段階で同じメッセージを使用するように選択したままにします。 各ステージに異なるメッセージを使用するには、<strong>すべてのステージでこのメッセージを表示</strong>をクリアしてから、各ステージの<strong> カスタムメッセージを追加</strong> テキストボックスにステージ固有のメッセージを入力します。</p></td>
   </tr>
   </table>

   ![ ステージを追加](assets/add-stage.png)

1. （オプション）「**ステージを追加**」をクリックして、パスに別のステージを追加します。 パス内のステージは、リストされている順序で順次実行されます。 ステージで必要なすべての決定が行われると、そのパスの次のステージが開始され、前のステージがロックされます。 パス内のステージを並べ替えることはできますが、あるパスから別のパスにステージを移動することはできません。 各パスには異なる数のステージを設定できます。

1. （オプション）「**並列パス**」で、「**パスを追加**」をクリックして別のパスを追加します。 新しいパスは、1つの空のステージから始まり、選択したパスになります。 パスは並べ替えできません。

   ![並行パスを追加](assets/add-path.png)

1. （オプション）パスの名前を変更するには、パスのラベルにカーソルを合わせて鉛筆アイコンをクリックし、新しい名前を入力します。 パスを削除するには、パスラベルにカーソルを合わせて、ごみ箱アイコンをクリックします。 **パス 1**&#x200B;を削除できません。他のパスは、パス内のステージがロックまたは完了していない場合にのみ削除できます。

1. （オプション）すべてのパスとステージをクリアして最初からやり直すには、右上隅の「**リセット**」をクリックします。

1. 「**保存**」をクリックします。

テンプレートを作成したら、そのテンプレートをオブジェクトの「ドキュメント」領域のドキュメントに適用して、Workfrontで正式なレビューと承認プロセスを開始できます。

<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
