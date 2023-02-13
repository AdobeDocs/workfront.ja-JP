---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] キャンペーンリクエストまたはキャンペーンプロジェクト
description: この統合シナリオは、 [!DNL Anaplan] 戻る [!DNL Workfront]. シナリオでは、リンクされたキャンペーン予算項目をすべて取り込み、予算値が変更されている場合は、その予算値をリンクされたWorkfrontプロジェクトに渡します。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] キャンペーンリクエストまたはキャンペーンプロジェクト

この統合シナリオは、 [!DNL Anaplan] 戻る [!DNL Workfront]. シナリオは、リンクされたキャンペーン予算項目をすべて取り込み、予算値をリンクされた [!DNL Workfront] 予算の値が変更された場合はプロジェクト。

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

* のユーザープロファイル [!DNL Workfront] 名前付き **[!DNL Anaplan Integration]**：システム管理者権限を持ちます。

   でのユーザーの作成に関する情報 [!DNL Workfront]を参照してください。 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 予測 [!DNL Anaplan] 設定

で以下をおこなう必要があります。 [!DNL Anaplan] このシナリオを使用するには、次の手順に従います。

* のユーザープロファイル [!DNL Anaplan] 名前付き **[!UICONTROL [!DNL Workfront]統合]**：システム管理者権限を持ちます。
* この [!DNL Anaplan] このシナリオに使用するモデル。
* リスト [!DNL Anaplan] キャンペーン予算をキャプチャするモデル。

   リストのモジュールは、次の属性の受け取りをサポートしている必要があります。

   * [!UICONTROL [!DNL Workfront] リクエスト GUID]
   * [!UICONTROL [!DNL Workfront] プロジェクト GUID]
   * [!UICONTROL キャンペーン名]
   * [!UICONTROL 希望労働基金]
   * [!UICONTROL 推定売上高]
   * [!UICONTROL ブランド]

   このリストとモジュールには、の通常の機能に必要な追加の詳細を格納する必要があります。 [!DNL Anaplan]（予算を設定し、予算リスト項目を再度に同期する準備ができたことを伝える機能を含む） [!DNL Workfront].

* のビュー [!DNL Anaplan] 呼び出し **[!UICONTROL Adobe Workfrontの Campaigns.Update Campaigns]**.

   このビューには、次の列がこの順序で含まれている必要があります。

   1. [!UICONTROL 項目名]

   2. [!UICONTROL [!DNL Workfront] リクエスト GUID]

   3. [!UICONTROL [!DNL Workfront] プロジェクト GUID]

   4. [!UICONTROL キャンペーン名]

   5. [!UICONTROL 予算]

   6. [!UICONTROL 推定売上高]

   7. [!UICONTROL ブランド]
   ビューをフィルタリングして、 [!UICONTROL [!DNL Workfront] プロジェクト GUID] 予算配分をWorkfrontに送信する必要があるという指標が含まれています。

これらの操作の手順については、 [!DNL Anaplan] ドキュメント。

## Workfront Fusion へのデプロイ

次の手順を実行して、この統合シナリオを Fusion アカウントにデプロイします。 これは、必要な [!DNL Workfront] および [!DNL Anaplan] 設定。

1. 次に移動： [!UICONTROL テンプレート] メニュー [!DNL Workfront Fusion] をクリックし、 **[!UICONTROL 適用 [!DNL Anaplan] Workfront campaign のリクエストとプロジェクトへの予算の割り当て]** シナリオテンプレート。
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ビュー名 ]</td> 
      <td> <p>送信準備完了のキャンペーン予算を含むビューの名前 [!DNL Workfront].</p> <p>( 例：[!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ファイルとプロセスの設定方法の詳細については、 [!DNL Anaplan] 設定ドキュメント。

1. を選択または追加します。 [!DNL Anaplan] 接続プロファイル。
1. 残りのすべてを更新 [!DNL Anaplan] モジュール [!DNL Anaplan] 接続を求められた場合。
1. の **[!UICONTROL CSV を JSON オブジェクトに変換]** モジュールで、CSV 列を使用可能な JSON オブジェクトにマッピングする新しいデータ構造を追加します。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. プロンプトが表示されたら、このシナリオのデプロイメントで他のモジュールに対してこのデータ構造を選択します。
1. の **[!UICONTROL リンクされたプロジェクトを確認]** モジュール、選択または追加 [!DNL Workfront] 接続プロファイル。
1. 残りのすべてを更新 [!DNL Workfront] モジュール [!DNL Workfront] 接続を求められた場合。

## その他の推奨シナリオテンプレート

このテンプレートで表されるワークフローを完了するには、次の追加テンプレートもデプロイする必要があります。

* [[!UICONTROL の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] キャンペーンリクエスト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

支出の最適化に関するその他のシナリオは次のとおりです。

* [[!UICONTROL 送信 [!DNL Adobe Workfront] プロジェクトの更新 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 送信 [!DNL Adobe Workfront] の実際の更新時間 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 送信 [!DNL Adobe Workfront] ～への費用 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
