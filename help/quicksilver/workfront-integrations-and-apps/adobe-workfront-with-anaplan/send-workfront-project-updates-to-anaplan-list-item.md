---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 送信 [!DNL Adobe Workfront] プロジェクトの更新 [!DNL Anaplan] リスト項目
description: この統合シナリオは、 [!DNL Adobe Workfront] プロジェクトに [!DNL Anaplan] 予算リスト項目。 この情報を共有すると、支出の最適化と財務分析をより有効に活用できます。 [!DNL Anaplan] 提供。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# 送信 [!DNL Adobe Workfront] プロジェクトの更新 [!DNL Anaplan] リスト項目

この統合シナリオは、 [!DNL Adobe Workfront] プロジェクトに [!DNL Anaplan] 予算リスト項目。 この情報を共有すると、支出の最適化と財務分析をより有効に活用できます。 [!DNL Anaplan] 提供。

>[!IMPORTANT]
>
>この記事の「キャンペーン」は、このシナリオが表すマーケティングキャンペーンの使用例を指し、 [!DNL Workfront Fusion] Adobe Campaignコネクタ、または最近廃止された [!UICONTROL Campaign] オブジェクト [!DNL Workfront].

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

&#42;&#42;詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## トリガーイベント

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 予測 [!DNL Workfront] 設定

で以下をおこなう必要があります。 [!DNL Workfront] このシナリオを使用するには、次の手順に従います。

* のユーザープロファイル [!DNL Workfront] 名前付き **[!UICONTROL [!DNL Anaplan]統合]**：システム管理者権限を持ちます。

   でのユーザーの作成に関する情報 [!DNL Workfront]を参照してください。 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL キャンペーンの概要]** Anaplan に送信するように選択したカスタムデータ値を保存するために、プロジェクトオブジェクトに添付されたカスタムフォーム。

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
     <td>[!UICONTROL 日付 ] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL 日付 ]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign の概要 ]</td> 
     <td>[!UICONTROL 段落テキストフィールド ]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL キーメッセージ ]</td> 
     <td>[!UICONTROL 段落テキストフィールド ]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL ドロップダウン ]</p> <p>プロセスに適したオプションを含めます。</p> </td> 
    </tr> 
   </tbody> 
  </table>

   カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## 予測 [!DNL Anaplan] 設定

で以下をおこなう必要があります。 [!DNL Anaplan] このシナリオを使用するには、次の手順に従います。

* のユーザープロファイル [!DNL Anaplan] 名前付き **[!UICONTROL [!DNL Workfront]統合]**：システム管理者権限を持ちます。
* この [!DNL Anaplan] このシナリオに使用するモデル。
* リスト [!DNL Anaplan] このシナリオに使用するモデル。
* A **[!UICONTROL プロジェクト更新の読み込み]** 次の列を含むファイルを、次の順序で並べ替えます。

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

を準備するには、以下を実行します。 [!UICONTROL [!DNL Anaplan] 計画経費インポート] ファイル：

1. 次の内容をテキストエディターにコピー&amp;ペーストします。 [!DNL Excel]
1. ファイルを CSV 形式で保存
1. ファイルを Anaplan にアップロードします。

   手順については、 [!DNL Anaplan] ファイルからモジュールにデータをインポートする方法に関するドキュメント。

1. ファイルに付けた名前をメモしておきます。これは、 [!UICONTROL 統合] シナリオテンプレート。

CSV コンテンツの例

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL キャンペーンの概要]

2. [!UICONTROL 主要なメッセージ]

3. [!UICONTROL 市場開始日]

4. [!UICONTROL 市場終了日]

5. [!UICONTROL ターゲットオーディエンス]

また、マッピングで設定する他のフィールドも含めます。

* A **[!UICONTROL プロジェクト更新の読み込み]** ファイルのアップロードで配信されたデータのインポートを実行するための準備が整ったプロセス。

これらの操作の手順については、 [!DNL Anaplan] ドキュメント。

## へのデプロイ [!DNL Workfront Fusion]

次の手順を実行して、この統合シナリオを Fusion アカウントにデプロイします。 これは、必要な [!DNL Workfront] および [!DNL Anaplan] 設定。

1. 次に移動： [!UICONTROL テンプレート] メニュー [!DNL Workfront Fusion] をクリックし、 **[!UICONTROL Workfrontプロジェクトの更新情報の送信先 [!DNL Anaplan] リスト項目]** シナリオテンプレート。
1. 次の変数値を置き換えます [!DNL Anaplan] 変数：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>変数名</th> 
      <th>値を次で置換</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ワークスペース ID]</td> 
      <td>のワークスペースの ID [!DNL Anaplan] アカウント</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] モデル ID] </td> 
      <td>のモデルの ID [!DNL Anaplan] アカウントと選択したワークスペース。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL キャンペーンリスト名 ]</td> 
      <td>リストの名前 [!DNL Anaplan] アカウントと選択したワークスペースおよびモデル。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ファイル名：プロジェクト更新の読み込み ]</td> 
      <td>プロジェクトの更新データを受け取るファイルの名前。<p>( 例：WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL プロセス名：プロジェクト更新の読み込み ]</td> 
      <td> <p>プロジェクトデータのインポートを実行するプロセスの名前。</p> <p>( 例：WF 整数 — キャンペーン詳細の更新 )</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] サブドメイン ]</td> 
      <td>のサブドメイン [!DNL Workfront] アカウント これは、 [!DNL Workfront] プロジェクトをメモに書き込んで、生成される場合があります。</td> 
     </tr> 
    </tbody> 
   </table>

   ファイルとプロセスの設定方法の詳細については、 [!DNL Anaplan] 設定ドキュメント。

1. を選択または追加します。 [!DNL Anaplan] 接続プロファイル。
1. 残りのすべてを更新 [!DNL Anaplan] モジュール [!DNL Anaplan] 接続を求められた場合。
1. を選択または追加します。 [!DNL Workfront] 接続プロファイル。

   フィルターは、不完全なリンク済みプロジェクトと過去 29 分間に完了したプロジェクトをすべて取り込むように設定されます。 この [!DNL Fusion] シナリオを選択します。

1. の **[!UICONTROL プロジェクトの作成 CSV の更新]** モジュールで、プロジェクト属性を CSV 列にマッピングする新しいデータ構造を追加します。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 残りのすべてを更新 [!DNL Workfront] モジュール [!DNL Workfront] 接続を求められた場合。

## その他の推奨シナリオテンプレート

このシナリオテンプレートは、次の支出最適化シナリオテンプレートを補完するもので、デプロイすることもできます。

* [[!UICONTROL 送信 [!DNL Adobe Workfront] の実際の更新時間 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 送信 [!DNL Adobe Workfront] ～への費用 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

予算要求のリンクに関するその他のシナリオ：

* [[!UICONTROL の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] 予算リクエスト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] プロジェクト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

キャンペーンリクエストのリンクに関するその他のシナリオ：

* [[!UICONTROL の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] キャンペーンリクエスト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] キャンペーンリクエストまたはキャンペーンプロジェクト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
