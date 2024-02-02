---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront]  の実際の時間数のアップデートを  [!DNL Anaplan]  リスト項目に送信'
description: この統合シナリオでは、 [!DNL Adobe Workfront]  プロジェクトで取得された実際の時間数の詳細を  [!DNL Anaplan]  の予算リスト項目と共有します。この情報を共有すると、 [!DNL Anaplan]  が提供する支出の最適化と財務分析をより有効に活用できます。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: ht
source-wordcount: '725'
ht-degree: 100%

---

# [!DNL Adobe Workfront] の実際の時間数のアップデートを [!DNL Anaplan] リスト項目に送信

この統合シナリオでは、[!DNL Adobe Workfront] プロジェクトで取得された実際の時間数の詳細を [!DNL Anaplan] の予算リスト項目と共有します。この情報を共有すると、[!DNL Anaplan] が提供する支出の最適化と財務分析をより有効に活用できます。

このシナリオテンプレートは、過去 3 か月間にアクティブなプロジェクトで記録された、プロジェクト、日、役割別に要約された時間のリストを提供します。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## イベントのトリガー

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 想定される [!DNL Workfront] 設定

このシナリオを使用するには、[!DNL Workfront] で以下のものが必要です。

* システム管理者権限が付与された **[!UICONTROL Anaplan Integration]** という名前の [!DNL Workfront] のユーザープロファイル。

  [!DNL Workfront] でのユーザーの作成について詳しくは、[ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

## 想定される [!DNL Anaplan] 設定

このシナリオを使用するには、[!DNL Anaplan] で以下のものが必要です。

* システム管理者権限が付与された **[!UICONTROL [!DNL Workfront]Anaplan Integration]** という名前の [!DNL Anaplan] のユーザープロファイル。
* このシナリオに使用する [!DNL Anaplan] モデル。
* このシナリオに使用する [!DNL Anaplan] モデル内のリスト。
* 次の列をこの順序で含んでいる、[!DNL Anaplan] の **[!UICONTROL Anaplan Actual Hours Import]** という名前のファイル。

   1. [!UICONTROL Workfront プロジェクト GUID]

   2. [!UICONTROL Hours]

   3. [!UICONTROL Hours Estimated Cost]

   4. [!UICONTROL エントリ日]

   5. [!UICONTROL Role Name]

   6. [!UICONTROL Campaign Name]

   7. [!UICONTROL [!DNL Anaplan] List Item ID]

  [!DNL Anaplan] 実費レポートファイルを準備するには、以下を行います。

   1. 次の内容をテキストエディターまたは [!DNL Excel] にコピーして貼り付けます。
   1. ファイルを CSV 形式で保存
   1. ファイルを [!DNL Anaplan] にアップロードします。

      手順については、ファイルからモジュールにデータをインポートする方法に関する [!DNL Anaplan] ドキュメントを参照してください。

   1. ファイルに付けた名前をメモしておきます。この名前は、[!UICONTROL Fusion] シナリオテンプレートをデプロイする際に使用されます。

  CSV コンテンツの例

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* ファイルのアップロードで配信されたデータのインポートを実行するために準備された、**[!UICONTROL プロジェクトの実際時間数の読み込み]**&#x200B;プロセス。

これらの操作の手順については、[!DNL Anaplan] ドキュメントを参照してください。

## [!DNL Workfront Fusion] へのデプロイ

この統合シナリオを [!DNL Fusion] アカウントにデプロイするには、次の手順を実行します。これは、必要な [!DNL Workfront] および [!DNL Anaplan] の設定を完了した後にのみ実行してください。

1. [!DNL Workfront Fusion] の[!UICONTROL テンプレート]メニューに移動し、**[!UICONTROL Workfront の実際の時間数の更新を [!DNL Anaplan] リスト項目に送信]**&#x200B;シナリオテンプレートをクリックします。
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
      <td role="rowheader">[!UICONTROL File Name: Actual Hours Import]</td> 
      <td> <p>プロジェクトの実際の時間数データを受け取るファイルの名前。</p> <p> （例： WorkfrontUpdateLinkedProjects_HoursRoles.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Actual Hours Import]</td> 
      <td> <p>プロジェクトの時間データの読み込みを実行するプロセスの名前。</p> <p>（例： WF Int — ロール別のプロジェクト時間の読み込み）</p> </td> 
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
1. プロンプトが表示されたら、残りのすべての [!DNL Workfront] モジュールを [!DNL Workfront] 接続で更新します。

## その他の推奨シナリオテンプレート

このシナリオテンプレートは、次の支出最適化シナリオテンプレートを補完するもので、デプロイすることもできます。

* [[!UICONTROL  [!DNL Adobe Workfront]  プロジェクトの更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL  [!DNL Adobe Workfront]  費用を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

予算リクエストのリンクに関する追加のシナリオ：

* [[!UICONTROL  [!DNL Adobe Workfront]  予算リクエストから  [!DNL Anaplan]  リスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL  [!DNL Anaplan]  予算配分を  [!DNL Adobe Workfront]  プロジェクトに適用]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

キャンペーンリクエストのリンクに関する追加のシナリオ：

* [[!UICONTROL  [!DNL Adobe Workfront]  キャンペーンリクエストから  [!DNL Anaplan]  リスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL  [!DNL Anaplan]  予算配分を  [!DNL Adobe Workfront]  キャンペーンリクエストまたはキャンペーンプロジェクトに適用する]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
