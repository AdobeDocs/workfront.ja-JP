---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] キャンペーンリクエスト
description: この統合シナリオでは、 [!DNL Adobe Workfront] プロジェクトに [!DNL Anaplan] 予算リスト項目。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 2%

---

# の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] キャンペーンリクエスト

この統合シナリオでは、 [!DNL Adobe Workfront] プロジェクトに [!DNL Anaplan] 予算リスト項目。

このシナリオは、リクエストキューに追加された新しいキャンペーンリクエストを監視します。 キャンペーンリクエストが記録されるとすぐに、予算行項目が [!DNL Anaplan] 資金調達プロセスを開始します。

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
   <td role="rowheader">[!UICONTROL Adobe Workfront] プラン*</td> 
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

* のユーザープロファイル [!DNL Workfront] 名前付き **[!UICONTROL [!DNL Anaplan]統合]**：システム管理者権限を持ちます。

   でのユーザーの作成に関する情報 [!DNL Workfront]を参照してください。 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL キャンペーンの概要]** に添付されたカスタムフォーム [!UICONTROL リクエスト] オブジェクト。

   Analyplan へのデータマッピングに役立つように、次の必須フィールドをカスタムフォームに含める必要があります。

   | フィールド名 | フィールドタイプ |
   |---|---|
   | [!UICONTROL 要求された資金の合計] |  |
   | [!UICONTROL 希望労働基金] |  |
   | [!UICONTROL 要求された費用基金] |  |
   | [!UICONTROL 送信先 [!DNL Anaplan]] | チェックボックス |

   次のオプションフィールドがフォームに存在する場合があります。 このシナリオでは上記のフィールドのみをマッピングしますが、キャンペーン概要の追加フィールドはマッピングできます。

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
     <td>日付 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>日付</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign の概要 ]</td> 
     <td>段落テキストフィールド</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL キーメッセージ ]</td> 
     <td>段落テキストフィールド</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>ドロップダウン</p> <p>プロセスに適したオプションを含めます。</p> </td> 
    </tr> 
   </tbody> 
  </table>

   カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* 新しいキャンペーンリクエストをキャプチャするためのリクエストキューとして設定されたプロジェクト。 この [!UICONTROL キャンペーンの概要] フォームは、これらの要求に添付する必要があります。

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
   * [!UICONTROL 要求された費用基金]
   * [!UICONTROL 予算要求タイプ]

   このリストとモジュールには、の通常の機能に必要な追加の詳細を格納する必要があります。 [!DNL Anaplan]（予算を設定し、予算リスト項目を再度に同期する準備ができたことを伝える機能を含む） [!DNL Workfront].

これらの操作の手順については、 [!DNL Anaplan] ドキュメント。

## へのデプロイ [!DNL Workfront Fusion]

次の手順を実行して、この統合シナリオを [!DNL Fusion] アカウント これは、必要な [!DNL Workfront] および [!DNL Anaplan] 設定。

1. 次に移動： [!UICONTROL テンプレート] メニュー [!DNL Workfront Fusion] をクリックし、 **[!UICONTROL の作成 [!DNL Anaplan] Workfront campaign リクエストの項目のリスト]** シナリオテンプレート。
1. 次の変数値を置き換えます [!DNL Anaplan] 変数：

   | 変数名 | 値を次で置換 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ワークスペース ID] | のワークスペースの ID [!DNL Anaplan] アカウント |
   | [!UICONTROL [!DNL Anaplan] モデル ID] | のモデルの ID [!DNL Anaplan] アカウントと選択したワークスペース。 |
   | [!UICONTROL [!DNL Anaplan] モジュール名] | 選択した内のキャンペーン属性を説明するモジュールの名前 [!DNL Anaplan] リスト。 |
   | [!UICONTROL キャンペーンリスト名] | リストの名前 [!DNL Anaplan] アカウントと選択したワークスペースおよびモデル。 |

   {style=&quot;table-layout:auto&quot;}

   ファイルとプロセスの設定方法の詳細については、 [!DNL Anaplan] 設定ドキュメント。

1. を選択または追加します。 [!DNL Anaplan] 接続プロファイル。
1. 残りのすべてを更新 [!DNL Anaplan] モジュール [!DNL Anaplan] 接続を求められた場合。
1. を選択または追加します。 [!DNL Workfront] 接続プロファイル。

   テンプレートをデプロイした後、デフォルトのマッピングされたフィールドをに変更する場合は、これが更新し、fields プロパティの値にカスタムフィールド参照を追加または削除するモジュールです。 [!DNL Anaplan].

1. 残りのすべてを更新 [!DNL Workfront] モジュール [!DNL Workfront] 接続を求められた場合。

## その他の推奨シナリオテンプレート

このテンプレートで表されるワークフローを完了するには、次の追加テンプレートもデプロイする必要があります。

* [[!UICONTROL 適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] キャンペーンリクエストまたはキャンペーンプロジェクト]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

支出の最適化に関するその他のシナリオは次のとおりです。

* [[!UICONTROL 送信 [!DNL Adobe Workfront] プロジェクトの更新 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 送信 [!DNL Adobe Workfront] の実際の更新時間 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 送信 [!DNL Adobe Workfront] ～への費用 [!DNL Anaplan] リスト項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
