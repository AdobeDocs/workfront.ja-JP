---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront]  の費用を  [!DNL Anaplan]  のリスト項目に送信'
description: この統合シナリオは、 [!DNL Adobe Workfront]  プロジェクトの費用関連の詳細を  [!DNL Anaplan]  予算リスト項目と共有します。この情報を共有すると、 [!DNL Anaplan]  が提供する支出の最適化と財務分析をより有効に活用できます。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 87%

---

# [!DNL Adobe Workfront] の費用を [!DNL Anaplan] のリスト項目に送信

この統合シナリオは、[!DNL Adobe Workfront] プロジェクトの費用関連の詳細を [!DNL Anaplan] 予算リスト項目と共有します。この情報を共有すると、[!DNL Anaplan] が提供する支出の最適化と財務分析をより有効に活用できます。

>[!IMPORTANT]
>
>この記事の「キャンペーン」は、このシナリオが表すマーケティングキャンペーンのユースケースを指し、[!DNL Workfront Fusion] Adobe Campaign コネクタ、または最近非推奨になった [!DNL Workfront] の[!UICONTROL キャンペーン]オブジェクトにはまったく接続されていません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意のAdobe Workfront ワークフローパッケージと任意のAdobe Workfront Automation and Integration パッケージ</p><p>WorkfrontUltimate</p><p>Workfront Fusion を追加購入したWorkfront Primeおよび Select パッケージ。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>標準</p><p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion ライセンス</td> 
   <td>
   <p>オペレーションベース：Workfront Fusion ライセンス要件なし</p>
   <p>コネクタベース（従来）：作業の自動化と統合のためのWorkfront Fusion </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>組織がWorkfront Automation and Integration を含まない Select またはPrime Workfront パッケージを持っている場合は、Adobe Workfront Fusion を購入する必要があります。</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

このテーブルの情報について詳しくは、[&#x200B; ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

Adobe Workfront Fusion ライセンスについて詳しくは、[Adobe Workfront Fusion ライセンス &#x200B;](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration) を参照してください。

## イベントのトリガー

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 想定される [!DNL Workfront] 設定

このシナリオを使用するには、[!DNL Workfront] に以下のものが必要です。

* *[!UICONTROL *[!DNL Anaplan] 統合]**という名前の、システム管理者権限が付与されている [!DNL Workfront] のユーザープロファイル。

  [!DNL Workfront] でのユーザーの作成について詳しくは、[ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

* [!DNL Anaplan] に送信することを選択したカスタムデータ値を保存するために、プロジェクトオブジェクトに添付された&#x200B;**[!UICONTROL キャンペーンの概要]**&#x200B;カスタムフォーム。

  フォームには次のフィールドが含まれている必要があります。

  | フィールド名 | フィールドタイプ |
  |---|---|
  | [!UICONTROL 最終送信日] | 日付 |
  | [!UICONTROL 統合に関するメモ] | 段落テキストフィールド |

  カスタムフォームの作成について詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

## 想定される [!DNL Anaplan] 設定

このシナリオを使用するには、[!DNL Anaplan] で以下のものが必要です。

* システム管理者権限が付与された **[!UICONTROL [!DNL Workfront]Anaplan Integration]** という名前の [!DNL Anaplan] のユーザープロファイル。
* このシナリオで使用する [!DNL Anaplan] モデル。
* キャンペーン予算を取得する [!DNL Anaplan] モデル内のリスト。
* 以下の順序で次の列を含む&#x200B;**[!UICONTROL 分析計画実費の読み込み]**&#x200B;ファイル：

   1. [!UICONTROL [!DNL Workfront]費用 GUID]

   2. [!UICONTROL [!DNL Workfront]プロジェクト GUID]

   3. [!UICONTROL 実際の金額]

   4. [!UICONTROL 説明]

   5. [!UICONTROL 費用タイプ]

   6. [!UICONTROL 発効日]

   7. [!UICONTROL キャンペーン名]

   8. [!UICONTROL [!DNL Anaplan]リスト項目 ID]

  [!UICONTROL [!DNL Anaplan] 実際の費用の読み込み]ファイルを準備するには、以下を実行します。

   1. 次の内容をテキストエディターまたは [!DNL Excel] にコピーして貼り付けます。
   1. ファイルを CSV 形式で保存します。
   1. ファイルを [!DNL Anaplan] にアップロードします。

      手順については、ファイルからモジュールにデータをインポートする方法に関する [!DNL Anaplan] ドキュメントを参照してください。

   1. ファイルに付けた名前をメモしておきます。この名前は、[!UICONTROL Fusion] シナリオテンプレートをデプロイする際に使用されます。

  CSV コンテンツの例

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* 以下の順序で次の列を含む **[!UICONTROL [!DNL Anaplan]予定費用の読み込み]**&#x200B;ファイル：

   1. [!UICONTROL [!DNL Workfront] 費用 GUID]

   2. [!UICONTROL [!DNL Workfront]プロジェクト GUID]

   3. [!UICONTROL 実際の金額]

   4. [!UICONTROL 説明]

   5. [!UICONTROL 費用タイプ]

   6. [!UICONTROL 発効日]

   7. [!UICONTROL キャンペーン名]

   8. [!UICONTROL [!DNL Anaplan] リスト項目 ID]

  [!UICONTROL [!DNL Anaplan] 予定費用の読み込み]ファイルを準備するには、以下を実行します。

   1. 次の内容をテキストエディターまたは [!DNL Excel] にコピーして貼り付けます。
   1. ファイルを CSV 形式で保存
   1. ファイルを Anaplan にアップロードします。

      手順については、ファイルからモジュールにデータを読み込む方法に関する [!DNL Anaplan] ドキュメントを参照してください。

   1. ファイルに付けた名前をメモしておきます。この名前は、[!UICONTROL Fusion] シナリオテンプレートをデプロイする際に使用されます。

  CSV コンテンツの例

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* ファイルのアップロードで配信されたデータの読み込みを実行するために準備された、**[!UICONTROL プロジェクト更新の読み込み]**&#x200B;プロセス。

>[!NOTE]
>
>予定の費用と実際の費用には個別に読み込みファイルがあり、それぞれの予定日と有効日にわたって個別にレポートできます。

これらのアクションの手順については、[!DNL Anaplan] ドキュメントを参照してください。

## [!DNL Fusion] へのデプロイ

この統合シナリオを [!DNL Fusion] アカウントにデプロイするには、次の手順を実行します。これは、必要な [!DNL Workfront] および [!DNL Anaplan] の設定を完了した後にのみ実行してください。

1. [!DNL Workfront Fusion] の[!UICONTROL テンプレート]メニューに移動し、**[!UICONTROL Workfront 費用の更新を [!DNL Anaplan] リスト項目に送信]**&#x200B;シナリオテンプレートをクリックします。
1. 次の [!DNL Anaplan] 変数の変数値を置換します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>変数名</th> 
      <th>値を次のように置換します。</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>このシナリオで使用する [!DNL Anaplan] アカウントのワークスペースの ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>[!DNL Anaplan] アカウントのモデルの ID と、このシナリオで使用する選択済みのワークスペース。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>[!DNL Anaplan] アカウントのリストの名前と、このシナリオで使用する選択済みのワークスペースおよびモデル。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Actual Expense Import]</td> 
      <td> <p>プロジェクトの実際の費用データを受け取るファイルの名前。</p> <p> （例：WorkfrontUpdateLinkedProjects_ActExpenses.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Planned Expense Import]</td> 
      <td> <p>プロジェクトの予定の費用データを受け取るファイルの名前。</p> <p> （例：WorkfrontUpdateLinkedProjects_PlannedExpenses.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>プロジェクトの費用データの読み込みを実行するプロセスの名前。</p> <p>（例：WF Int - Load Project Expenses）</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ファイルとプロセスの設定方法について詳しくは、[!DNL Anaplan] の設定ドキュメントを参照してください。

1. [!DNL Anaplan] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Anaplan] モジュールを [!DNL Anaplan] 接続で更新します。
1. [!DNL Workfront] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Workfront] モジュールを [!DNL Workfront] 接続で更新します。
1. **[!UICONTROL 実際の費用の CSV を作成]**&#x200B;モジュールで、プロジェクト属性を CSV 列にマッピングするための新しいデータ構造を追加します。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. **[!UICONTROL 予定の費用の CSV を作成]**&#x200B;モジュールで、プロジェクト属性を CSV 列にマッピングするための新しいデータ構造を追加します。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## その他の推奨シナリオテンプレート

このシナリオテンプレートは、次の支出最適化シナリオテンプレートを補完するもので、デプロイすることもできます。

* [[!UICONTROL &#x200B; [!DNL Adobe Workfront]  プロジェクトの更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL &#x200B; [!DNL Adobe Workfront]  の実際の時間の更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

予算リクエストのリンクに関する追加のシナリオ：

* [[!UICONTROL &#x200B; [!DNL Adobe Workfront]  予算リクエストから  [!DNL Anaplan]  リスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL &#x200B; [!DNL Anaplan]  予算配分を  [!DNL Adobe Workfront]  プロジェクトに適用]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

キャンペーンリクエストのリンクに関する追加のシナリオ：

* [[!UICONTROL &#x200B; [!DNL Adobe Workfront]  キャンペーンリクエストから  [!DNL Anaplan]  リスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL &#x200B; [!DNL Anaplan]  予算配分を  [!DNL Adobe Workfront]  キャンペーンリクエストまたはキャンペーンプロジェクトに適用する]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
