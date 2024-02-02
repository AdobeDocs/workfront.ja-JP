---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront]  キャンペーンリクエストから  [!DNL Anaplan]  リスト項目の作成'
description: この統合シナリオでは、 [!DNL Adobe Workfront]  プロジェクトを  [!DNL Anaplan]  の予算リスト項目にリンクします。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: ht
source-wordcount: '730'
ht-degree: 100%

---

# [!DNL Adobe Workfront] キャンペーンリクエストから [!DNL Anaplan] リスト項目の作成

この統合シナリオでは、[!DNL Adobe Workfront] プロジェクトを [!DNL Anaplan] の予算リスト項目にリンクします。

このシナリオは、リクエストキューに追加された新規キャンペーンリクエストを監視します。キャンペーンリクエストが記録されるとすぐに、予算行項目が [!DNL Anaplan] に追加され、資金調達プロセスが開始されます。

>[!IMPORTANT]
>
>この記事の「キャンペーン」は、このシナリオが表すマーケティングキャンペーンのユースケースを指しており、[!DNL Workfront Fusion] Adobe Campaign コネクタや、[!DNL Workfront] にある、最近非推奨になった [!UICONTROL Campaign] オブジェクトにはまったく関係ありません。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

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

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## イベントのトリガー

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 予期される [!DNL Workfront] 設定

このシナリオを使用するには、[!DNL Workfront] に次のものが必要です。

* システム管理者権限が付与されている、**[!UICONTROL [!DNL Anaplan]統合]**&#x200B;という名前の [!DNL Workfront] でのユーザープロファイル。

  [!DNL Workfront] でのユーザーの作成について詳しくは、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

* [!UICONTROL リクエスト]オブジェクトに添付された&#x200B;**[!UICONTROL キャンペーンの概要]**&#x200B;カスタムフォーム。

  Analyplan へのデータのマッピングを支援するために、以下の必須フィールドをカスタムフォームに含める必要があります。

  | フィールド名 | フィールドタイプ |
  |---|---|
  | [!UICONTROL 要求資金の合計] |   |
  | [!UICONTROL 要求労働資金] |   |
  | [!UICONTROL 要求費用基金] |   |
  | [!UICONTROL [!DNL Anaplan]] に送信済み | チェックボックス |

  以下のオプションフィールドがフォームに存在する場合があります。このシナリオでは上記のフィールドのみがマッピングされますが、キャンペーン概要の追加フィールドがマッピングされる場合があります。

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
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>段落テキストフィールド</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>段落テキストフィールド</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>ドロップダウン</p> <p>プロセスに適したオプションを含めます。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  カスタムフォームの作成について詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください

* 新しいキャンペーンリクエストをキャプチャするためのリクエストキューとして設定されたプロジェクト。[!UICONTROL キャンペーンの概要]フォームを、これらのリクエストに添付する必要があります。

## 期待される [!DNL Anaplan] 設定

このシナリオを使用するには、[!DNL Anaplan] に以下のものが必要です。

* **[!UICONTROL [!DNL Workfront]統合]**&#x200B;という名前の [!DNL Anaplan] のユーザープロファイル。システム管理者権限が付与されています。
* このシナリオに使用する [!DNL Anaplan] モデル。
* キャンペーン予算を取得する [!DNL Anaplan] モデル内のリスト。

  リストのモジュールは、次の属性の受信をサポートする必要があります。

   * [!UICONTROL [!DNL Workfront] リクエスト GUID]
   * [!UICONTROL [!DNL Workfront] プロジェクト GUID]
   * [!UICONTROL キャンペーン名]
   * [!UICONTROL 要求労働資金]
   * [!UICONTROL 要求費用基金]
   * [!UICONTROL 予算要求タイプ]

  このリストとモジュールには、予算を設定し、予算リスト項目を [!DNL Workfront] に同期する準備ができていることを伝える機能など、[!DNL Anaplan] の通常の機能に必要な追加の詳細を保存する必要があります。

これらのアクションの手順については、[!DNL Anaplan] ドキュメントを参照してください。

## [!DNL Workfront Fusion] へのデプロイ

この統合シナリオを [!DNL Fusion] アカウントにデプロイするには、次の手順を実行します。これは、必要な [!DNL Workfront] および [!DNL Anaplan] の設定を完了した後にのみ実行してください。

1. [!DNL Workfront Fusion] の[!UICONTROL テンプレート]メニューに移動し、**[!UICONTROL Workfront キャンペーンリクエストから [!DNL Anaplan] リスト項目を作成]**&#x200B;シナリオテンプレートをクリックします。
1. 次の [!DNL Anaplan] 変数の変数値を置換します。

   | 変数名 | 値を次のように置換します。 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan]ワークスペース ID] | [!DNL Anaplan] アカウントのワークスペースの ID。 |
   | [!UICONTROL [!DNL Anaplan]モデル ID] | [!DNL Anaplan] アカウントと選択したワークスペースのモデルの ID。 |
   | [!UICONTROL [!DNL Anaplan]モジュール名] | 選択した [!DNL Anaplan] リスト内のキャンペーン属性を説明するモジュールの名前。 |
   | [!UICONTROL キャンペーンリスト名] | [!DNL Anaplan] アカウントのリスト名、および選択したワークスペースとモデル。 |

   {style="table-layout:auto"}

   ファイルとプロセスの設定方法について詳しくは、[!DNL Anaplan] の設定ドキュメントを参照してください。

1. [!DNL Anaplan] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Anaplan] モジュールを [!DNL Anaplan] 接続で更新します。
1. [!DNL Workfront] 接続プロファイルを選択または追加します。

   テンプレートを導入後、デフォルトのマップされたフィールドを [!DNL Anaplan] に変更する場合、これはフィールドプロパティの値にカスタムフィールド参照を追加または削除するために更新するモジュールです。

1. プロンプトが表示されたら、残りのすべての [!DNL Workfront] モジュールを [!DNL Workfront] 接続で更新します。

## その他の推奨シナリオテンプレート

このテンプレートで表されるワークフローを完了するには、次の追加のテンプレートもデプロイする必要があります。

* [[!UICONTROL  [!DNL Anaplan]  の予算配分を  [!DNL Adobe Workfront]  キャンペーンリクエストまたはキャンペーンプロジェクトに適用]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

支出を最適化するための追加のシナリオには次のものがあります。

* [[!UICONTROL  [!DNL Adobe Workfront]  プロジェクトの更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL  [!DNL Adobe Workfront]  の実際の時間数の更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL  [!DNL Adobe Workfront]  の費用を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
