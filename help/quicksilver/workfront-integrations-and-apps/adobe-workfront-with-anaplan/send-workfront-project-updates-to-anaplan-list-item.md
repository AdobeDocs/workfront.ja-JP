---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront]  プロジェクトアップデートの  [!DNL Anaplan]  リスト項目への送信'
description: この統合シナリオは、 [!DNL Anaplan]  予算リスト項目を持つ  [!DNL Adobe Workfront]  プロジェクトの進捗状況、ステータスおよび主要なスケジュールの詳細を共有します。この情報を共有すると、 [!DNL Anaplan]  が提供する支出の最適化と財務分析をより有効に活用できます。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: ht
source-wordcount: '909'
ht-degree: 100%

---

# [!DNL Adobe Workfront] プロジェクトアップデートの [!DNL Anaplan] リスト項目への送信

この統合シナリオは、[!DNL Anaplan] 予算リスト項目を持つ [!DNL Adobe Workfront] プロジェクトの進捗状況、ステータスおよび主要なスケジュールの詳細を共有します。この情報を共有すると、[!DNL Anaplan] が提供する支出の最適化と財務分析をより有効に活用できます。

>[!IMPORTANT]
>
>この記事の「キャンペーン」は、このシナリオが表すマーケティングキャンペーンのユースケースを指し、[!DNL Workfront Fusion] Adobe Campaign コネクタ、または最近非推奨になった [!DNL Workfront] の[!UICONTROL キャンペーン]オブジェクトにはまったく接続されていません。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## イベントのトリガー

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 予期される [!DNL Workfront] 設定

このシナリオを使用するには、[!DNL Workfront] に次のものが必要です。

* システム管理者権限が付与されている、**[!UICONTROL [!DNL Anaplan]統合]**&#x200B;という名前の [!DNL Workfront] でのユーザープロファイル。

  [!DNL Workfront] でのユーザーの作成について詳しくは、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

* Anaplan に送信することを選択したカスタムデータ値を保存するために、プロジェクトオブジェクトに添付された&#x200B;**[!UICONTROL キャンペーンの概要]**&#x200B;カスタムフォーム。

  次のフィールドは、Analyplan へのデータマッピングに役立つカスタムフォームに含めることができるフィールドの例を示していますが、この統合シナリオでは必須ではありません。

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>フィールド名</th> 
     <th>フィールドタイプ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>プロセスに適したオプションを含めます。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  カスタムフォームの作成について詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## 想定される [!DNL Anaplan] 設定

このシナリオを使用するには、[!DNL Anaplan] において次が必要になります。

* システム管理者権限が付与されている、**[!UICONTROL [!DNL Workfront]統合]**&#x200B;という名前の [!DNL Anaplan] のユーザープロファイル。
* このシナリオに使用する [!DNL Anaplan] モデル。
* このシナリオに使用する [!DNL Anaplan] モデル内のリスト。
* **[!UICONTROL プロジェクト更新の読み込み]**&#x200B;ファイルは、この順序で次の列を含みます。

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] プロジェクト GUID]

3. [!UICONTROL キャンペーン名]

4. [!UICONTROL 完了率]

5. [!UICONTROL 予定開始日]

6. [!UICONTROL 予定完了日]

7. [!UICONTROL 予定時間数]

8. [!UICONTROL 予定コスト]

9. [!UICONTROL 予定費用コスト]

10. [!UICONTROL 実際の労力コスト]

11. [!UICONTROL 予定労力コスト]

12. [!UICONTROL ステータス]

[!UICONTROL [!DNL Anaplan] 予定費用読み込み]ファイルを準備するには、以下を実行します。

1. 次の内容をテキストエディターまたは [!DNL Excel] にコピーして貼り付けます。
1. ファイルを CSV 形式で保存
1. ファイルを Anaplan にアップロードします。

   手順については、ファイルからモジュールにデータを読み込む方法に関する [!DNL Anaplan] ドキュメントを参照してください。

1. ファイルに付けた名前をメモしておきます。この名前は、[!UICONTROL Fusion] シナリオテンプレートを展開する際に使用されます。

CSV コンテンツの例

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>オプションの列には、次のものが含まれます。

1. [!UICONTROL キャンペーンの概要]

2. [!UICONTROL 主要なメッセージ]

3. [!UICONTROL マーケット開始日]

4. [!UICONTROL マーケット終了日]

5. [!UICONTROL ターゲットオーディエンス]

また、マッピングで設定する他のフィールドも含めます。

* ファイルのアップロードで送信されたデータの読み込み実行のために作成した&#x200B;**[!UICONTROL プロジェクト更新の読み込み]**&#x200B;プロセス。

これらのアクションの手順については、[!DNL Anaplan] ドキュメントを参照してください。

## [!DNL Workfront Fusion] へのデプロイ

次の手順を実行して、この統合シナリオを Fusion アカウントにデプロイします。これは、必要な [!DNL Workfront] および [!DNL Anaplan] の設定を完了した後にのみ実行してください。

1. [!DNL Workfront Fusion] の[!UICONTROL テンプレート]メニューに移動し、**[!UICONTROL Workfront プロジェクトの更新を [!DNL Anaplan] リスト項目に送信]**&#x200B;シナリオテンプレートをクリックします。
1. 次の [!DNL Anaplan] 変数の変数値を置換します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>変数名</th> 
      <th>値を次のように置換します。</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>[!DNL Anaplan] アカウントのワークスペースの ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>[!DNL Anaplan] アカウントと選択したワークスペースのモデルの ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>[!DNL Anaplan] アカウントのリスト名、および選択したワークスペースとモデル。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>プロジェクトの更新データを受け取るファイルの名前。<p>（例：WorkfrontUpdateLinkedProject.csv）</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>プロジェクトデータの読み込みを実行するプロセスの名前。</p> <p>（例：WF Int - Update Campaign Details）</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>[!DNL Workfront] アカウントのサブドメイン。これは、生成されるメモ内に [!DNL Workfront] プロジェクトへのリンクを作成するために使用されます。</td> 
     </tr> 
    </tbody> 
   </table>

   ファイルとプロセスの設定方法について詳しくは、[!DNL Anaplan] の設定ドキュメントを参照してください。

1. [!DNL Anaplan] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Anaplan] モジュールを [!DNL Anaplan] 接続で更新します。
1. [!DNL Workfront] 接続プロファイルを選択または追加します。

   フィルターは、リンクされた未完了のプロジェクトと、過去 29 分間に完了したプロジェクトをすべて取り込むように設定されます。[!DNL Fusion] シナリオの頻度を変更する場合は、シナリオテンプレートがデプロイされた後にこの値を更新します。

1. **[!UICONTROL プロジェクトの更新 CSV を作成]**&#x200B;モジュールで、プロジェクト属性を CSV 列にマッピングする新しいデータ構造を追加します。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. プロンプトが表示されたら、残りのすべての [!DNL Workfront] モジュールを [!DNL Workfront] 接続で更新します。

## その他の推奨シナリオテンプレート

このシナリオテンプレートは、次の支出最適化シナリオテンプレートを補完するもので、デプロイすることもできます。

* [[!UICONTROL  [!DNL Adobe Workfront]  の実際の時間数の更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL  [!DNL Adobe Workfront]  の費用を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

予算リクエストのリンクに関する追加のシナリオ：

* [[!UICONTROL  [!DNL Adobe Workfront] の予算リクエストから [!DNL Anaplan] のリスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL  [!DNL Anaplan] の予算配分を [!DNL Adobe Workfront] プロジェクトに適用]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

キャンペーンリクエストのリンクに関する追加のシナリオ：

* [[!UICONTROL  [!DNL Adobe Workfront] のキャンペーンリクエストから [!DNL Anaplan] のリスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL  [!DNL Anaplan] の予算配分を [!DNL Adobe Workfront] のキャンペーンリクエストまたはキャンペーンプロジェクトに適用]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
