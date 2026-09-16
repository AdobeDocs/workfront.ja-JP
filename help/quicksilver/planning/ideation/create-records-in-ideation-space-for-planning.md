---
title: アイデア立案スペースの概要からプランニングレコードを作成
description: Adobe Workfront Planningの新しい機能であるアイデア創出スペースを使用すると、ブリーフをプランニングレコードに変換できます。 書き出されたブリーフは、新しいレコードを作成したり、既存のレコードを更新したりできます。 この記事では、アイデア創出スペースを使用して、既存のプランニングレコードを作成または編集する方法について説明します。
role: User, Admin
author: Alina
source-git-commit: bef848df8b263de89bfa90b7fec74b14734dfeff
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 3%
---

# アイデア立案スペースの概要からプランニングレコードを作成

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 これは、**アイデア創出スペース Beta** プログラムの一部としてのみ使用できます。</span>

<span class="preview">詳細については、[Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planningの新しい機能であるアイデア創出スペースを使用すると、ブリーフをプランニングレコードに変換できます。 書き出されたブリーフは、新しいレコードを作成したり、既存のレコードを更新したりできます。

この記事では、アイデア創出スペースを使用して、既存のプランニングレコードを作成または編集する方法について説明します。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<ul> 
<li><p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p></li>
または
<li><p>スタンドアロン製品として購入された場合の任意のプランニング・パッケージ</p></li></ul>
   </td> 
    <!--
    <tr> 
    <td role="rowheader"><p>Additional products</p></td> 
    <td><ul>
    <li><p>Adobe GenStudio for Performance Marketing</p></li>
    <li><p>Adobe Customer Journey Analytics</p></li>
    </ul>
    </td> 
    </tr> 
    -->
  <tr> 
   <td role="rowheader"><p>Adobe Workflow ライセンス</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> 
   <ul>
   <li><p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>   </li>
   <li><p>アクセスレベルの「アイデア創出スペースを無効にする」設定を選択解除する必要があります</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードを追加するワークスペースおよびレコードタイプに対する権限を設定します </p>
      <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
      <p>Workfront オブジェクトに対する権限を表示して、ブリーフに追加する <!--not sure if this is available--></p>
      <p>ブリーフを作成するためのアイデア創出スペースの編集者権限</p>
   </td> 
  </tr>  
    <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

## アイデア創出スペースを使用したレコード作成に関する考慮事項

* アイデア創出スペースは、レコードを作成または編集する際に、Workfront計画またはWorkfrontのメインメニューからのみ起動できます。 アイデア創出スペースは、Workfront以外には存在しません。
* アイデア創出スペースにアクセスするには、Workfront Planningにワークスペースとレコードタイプが必要です。
* 新しいレコードは、作成方法に関係なく、常にプレースホルダーコンテンツから開始されます。
* アイデア概要にリンクされたプランニングレコードを削除すると、アイデア概要はアイデア作成スペースに残り、アイデア作成スペース内の関連するキャンバスは削除されません。
* 情報の同期は、アイデア立案スペースからWorkfront Planningにのみ行われます。 プランニングレコードからアイデア創出スペースブリーフへの逆同期や自動同期はありません。
* Workfront Planningでフィールドを作成、編集または削除する場合、次のシナリオが存在します。

  * アイデア立案ブリーフにリンクされたレコードに作成された新しいフィールドは、毎日ブリーフに追加されます。 新しいフィールドは、アイデアの概要では空で表示されます。
  * 削除されたフィールドはブリーフに残り、以前の値を保持します。
  * 名前を変更したフィールドは、ブリーフ内の名前を更新します。
* アイデア出しスペースでは、ドキュメントをカードとして追加できます。 これには画像も含まれます。

  サポートされているファイル形式は、PDF、Excel、CSV、PNG （およびその他の画像形式）、Word、PowerPointです。 ビデオはサポートされていません。

  アップロードされたすべてのドキュメントは、バックエンドのPDFに変換され、処理されます。
* レコードをWorkfront Planningから直接スペースにドラッグ&amp;ドロップすることができ、手動でアップロードしたファイルと同じように表示されます。

## アイデア創出スペースを使用したレコードの作成

1. Workfront Planningのランディングページで、管理できるワークスペースのカードをクリックします。
1. レコードを追加できるレコードタイプのカードをクリックします。
1. レコードを作成するには、次のいずれかの操作を行います。

   * レコードタイプページの任意のビューで、ページの右上隅にある&#x200B;**新しいレコード**&#x200B;をクリックし、**レコードを追加する方法を選択** ボックスで、**アイデア創出スペースを開く**&#x200B;をクリックし、**続行**&#x200B;をクリックします。
   * レコードテーブルの一番下までスクロールして&#x200B;**新しい行**&#x200B;をクリックし、**アイデア創出スペースを開く**&#x200B;をクリックします。

     >[!TIP]
     >
     >「**表示しない**」を選択すると、今後のプロンプトが完全に閉じられます。 閉じるアイコン **X**&#x200B;をクリックすると、このボックスは閉じますが、次回レコードをインラインに追加すると再度表示されます。

   ![ アイデア創出スペースを開くボタンを含む新しいレコードボックス ](assets/new-record-creation-picker-with-ideation.png)

   アイデア創出スペースが新しいタブで開き、空のプロンプトが表示されます。

   レコードは、プレースホルダーテキストを使用してすぐに作成されます。

1. （オプション）プロンプトボックスの「**既存の概要を使用**」をクリックして、アイデア創出スペースで概要と今後のレコードの作成に使用する既存の文書を参照して追加します。<!--CORRECT THIS PART: this is possible ONLY when you launch Ideation from the Main Menu, not from a record-->

   ![ アイデアの概要プロンプトが空です](assets/empty-ideation-prompt.png)

1. （オプション）プロンプトボックスの右上隅にある「**前のキャンバスを開く** <!--accurate??-->」アイコン「![既存のブリーフを開く](assets/open-existing-briefs-icon.png)」をクリックして、既存のブリーフを開きます

1. **で何に取り組んでいますか？** プロンプトボックスに入力し、作成するレコードの種類を指定します。

   共有する詳細情報が多ければ多いほど、アイデア創出スペースから提供される情報がより有用になります。 例えば、計画しているキャンペーンの説明を「マーケティングエージェンシーの学校戻りキャンペーン」と入力します。

1. 「**アイデア出しを開始**」をクリックします。

   アイデア創出スペースは、アイデアを作成する間、次の手順を実行します：<!--check some of these in the UI - there might have been UI text changes-->

   1. 目標とコンテクストの把握
   2. スペースと選択したマテリアルのレビュー
   3. ドキュメント、web、データから証拠を収集します
   4. 調査結果を調査サマリーに合成
   5. 引用を使用したカードの作成と調整

   このプロセスでは、接続されたWorkfront Planning データまたはweb上で利用可能な情報をアクティブに検索するアイデア創出スペースが表示されます。

   例えば、既存のプログラム、製品、ペルソナ、地域だけでなく、オンラインで利用可能な類似の概念を検索できます。<!--check on this with Et-->

   アイデア創出が完了すると、アイデア創出スペースに次のものが追加されます。

   * 考慮すべき事項に関する詳細な情報が記載された、複数のカードにリンクされたAI調査結果の概要。 詳細カードが新しいセクションに表示されます。 コネクタは、どのカードセクションがどのサマリーに属するかを示します。

   * アイデア創出スペースの左下隅にある&#x200B;**概要** ファイル。 概要は、今後のレコードのドラフトであり、レコードの詳細ページとして表示されます。

   ![分岐を含むアイデア創出カード ](assets/ideation-card-with-branched-off-additional-cards.png)

1. アイデア創出スペースに引き続き情報を追加して、ブリーフの作成を完了します。

1. （条件付き）概要が完了したら、左下隅にあるプレビュー画像をクリックし、次のいずれかをクリックします。

   * **ファイルに書き出し**：ファイルを作成
   * **Workfront Planning**&#x200B;に書き出して、プランニング レコードを作成します

   ブリーフへのアイテムの追加とエクスポートについて詳しくは、[ アイデア創出スペースでのブリーフの作成](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)を参照してください。

   これにより、追加情報を含むレコードの作成が完了し、最初に選択したレコードタイプに追加されます。

## アイデア立案スペースでの既存レコードの編集

既存のレコードからアイデア創出スペースを開いて更新できます。

アイデア出しスペースでレコードを一括編集することはできません。

1. Workfront Planningの既存のレコードに移動し、その詳細ページを開きます。

1. 「**アイデア創出スペースで開く**」をクリックします。 これにより、新しいタブでアイデア創出スペースが開きます。

   レコードのアイデアが既に存在する場合、そのスペースが開きます。

   アイデアが存在しない場合は、アイデア創出スペースと概要を作成します。

   >[!TIP]
   >
   >アイデア立案スペースを使用したレコードの一括編集は使用できません。

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. この記事の「[ アイデア創出スペース ](#create-records-using-the-ideation-space)」の節で説明しているように、引き続き概要を編集します。






<!--
this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


