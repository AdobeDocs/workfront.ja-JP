---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 送信 [!DNL Adobe Workfront] の実際の更新時間 [!DNL Anaplan] リスト項目
description: この統合シナリオは、 [!DNL Adobe Workfront] プロジェクトに [!DNL Anaplan] 予算リスト項目。 この情報を共有すると、支出の最適化と財務分析をより有効に活用できます。 [!DNL Anaplan] 提供。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# 送信 [!DNL Adobe Workfront] の実際の更新時間 [!DNL Anaplan] リスト項目

この統合シナリオは、 [!DNL Adobe Workfront] プロジェクトに [!DNL Anaplan] 予算リスト項目。 この情報を共有すると、支出の最適化と財務分析をより有効に活用できます。 [!DNL Anaplan] 提供。

このシナリオテンプレートは、過去 3 か月間にアクティブなプロジェクトで記録された、プロジェクト、日、役割別に要約された時間のリストを配信します。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
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

* のユーザープロファイル [!DNL Workfront] 名前付き **[!UICONTROL Analyplan 統合]**：システム管理者権限を持ちます。

   でのユーザーの作成に関する情報 [!DNL Workfront]を参照してください。 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 予測 [!DNL Anaplan] 設定

で以下をおこなう必要があります。 [!DNL Anaplan] このシナリオを使用するには、次の手順に従います。

* のユーザープロファイル [!DNL Anaplan] 名前付き **[!UICONTROL [!DNL Workfront ]統合]**：システム管理者権限を持ちます。
* この [!DNL Anaplan] このシナリオに使用するモデル。
* リスト [!DNL Anaplan] このシナリオに使用するモデル。
* 内のファイル [!DNL Anaplan] 名前付き **[!UICONTROL アナプランの実際の時間インポート]** 次の列を含む、この順序で：

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL 時間]

   3. [!UICONTROL 推定コスト（時間）]

   4. [!UICONTROL エントリ日]

   5. [!UICONTROL ロール名]

   6. [!UICONTROL キャンペーン名]

   7. [!UICONTROL [!DNL Anaplan] リスト項目 ID]
   を準備するには、以下を実行します。 [!DNL Anaplan] 実費レポートファイル：

   1. 次の内容をテキストエディターにコピー&amp;ペーストします。 [!DNL Excel]
   1. ファイルを CSV 形式で保存
   1. ファイルのアップロード先 [!DNL Anaplan].

      手順については、 [!DNL Anaplan] ファイルからモジュールにデータをインポートする方法に関するドキュメント。

   1. ファイルに付けた名前をメモしておきます。これは、 [!UICONTROL 統合] シナリオテンプレート。

   CSV コンテンツの例

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL プロジェクトの実績時間インポート]** ファイルのアップロードで配信されたデータのインポートを実行するための準備が整ったプロセス。

これらの操作の手順については、 [!DNL Anaplan] ドキュメント。

## へのデプロイ [!DNL Workfront Fusion]

次の手順を実行して、この統合シナリオを [!DNL Fusion] アカウント これは、必要な [!DNL Workfront] および [!DNL Anaplan] 設定。

1. 次に移動： [!UICONTROL テンプレート] メニュー [!DNL Workfront Fusion] をクリックし、 **[!UICONTROL Workfrontの実際の時間更新を次に送信： [!DNL Anaplan] リスト項目]** シナリオテンプレート。
1. 次の変数値を置き換えます [!DNL Anaplan] 変数：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
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
      <td role="rowheader">[!UICONTROL ファイル名：実際の時間のインポート ]</td> 
      <td> <p>プロジェクトの実績時間データを受け取るファイルの名前。</p> <p> ( 例：WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL プロセス名：実際の時間のインポート ]</td> 
      <td> <p>プロジェクト時間データのインポートを実行するプロセスの名前。</p> <p>( 例：WF 整数 — ロードプロジェクト時間（ロール別）</p> </td> 
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
1. 残りのすべてを更新 [!DNL Workfront] モジュール [!DNL Workfront] 接続を求められた場合。

## その他の推奨シナリオテンプレート

このシナリオテンプレートは、次の支出最適化シナリオテンプレートを補完するもので、デプロイすることもできます。

* [[!UICONTROL 送信 [!DNL Adobe Workfront] プロジェクトの更新 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 送信 [!DNL Adobe Workfront] ～への費用 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

予算要求のリンクに関するその他のシナリオ：

* [[!UICONTROL の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] 予算リクエスト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] プロジェクト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

キャンペーンリクエストのリンクに関するその他のシナリオ：

* [[!UICONTROL の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] キャンペーンリクエスト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] キャンペーンリクエストまたはキャンペーンプロジェクト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
