---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Adobe Workfront]  の予算リクエストからの  [!DNL Anaplan]  のリスト項目の作成'
description: この統合シナリオは、 [!DNL Adobe Workfront]  プロジェクト（キャンペーン）を  [!DNL Anaplan]  の予算リスト項目にリンクします。これは、資金調達が必要な  [!DNL Workfront]  プロジェクトに予算リクエストを追加することで達成できます。このシナリオでは、未処理の予算リクエストを監視し、 [!DNL Anaplan]  で空の予算リスト項目を作成するプロセスを実行して、Anaplan で予算配分プロセスを開始します。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: ht
source-wordcount: '807'
ht-degree: 100%

---

# [!DNL Adobe Workfront] の予算リクエストから [!DNL Anaplan] のリスト項目を作成

この統合シナリオは、[!DNL Adobe Workfront] プロジェクト（キャンペーン）を [!DNL Anaplan] の予算リスト項目にリンクします。これは、資金調達が必要な [!DNL Workfront] プロジェクトに予算リクエストを追加することで達成できます。このシナリオでは、未処理の予算リクエストを監視し、[!DNL Anaplan] で空の予算リスト項目を作成するプロセスを実行して、[!DNL Anaplan] で予算配分プロセスを開始します。

>[!IMPORTANT]
>
>この記事の「キャンペーン」は、このシナリオが表すマーケティングキャンペーンのユースケースを指し、[!DNL Workfront Fusion] Adobe Campaign コネクタや、最近非推奨になった [!DNL Workfront] の [!UICONTROL Campaign] オブジェクトとは関係ありません。

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
   <td role="rowheader" [!DNL>Adobe Workfront Fusion ライセンス**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr>
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL  Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## イベントのトリガー

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 想定される [!DNL Workfront] の設定

このシナリオを使用するには、[!DNL Workfront] に以下のものが必要です。

* *[!UICONTROL *[!DNL Anaplan] 統合]**という名前の、システム管理者権限が付与されている [!DNL Workfront] のユーザープロファイル。

  [!DNL Workfront] でのユーザーの作成について詳しくは、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

* [!UICONTROL Request] オブジェクトに添付された&#x200B;**[!UICONTROL 予算リクエスト]**&#x200B;カスタムフォーム。

  [!DNL Anaplan] へのデータのマッピングを補助するために、以下の必須フィールドをカスタムフォームに含める必要があります。

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>フィールド名</th> 
     <th>フィールドタイプ</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Budget Request Type]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>オプション：</p> 
      <ul> 
       <li> <p>[!UICONTROL Adjustment to Funding]</p> </li> 
       <li> <p>[!UICONTROL Initial Funding]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Labor Funds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Expense Funds]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  カスタムフォームの作成について詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

* [!UICONTROL 予算リクエスト]キューのトピックで設定された、資金調達を必要とするキャンペーンやその他のプロジェクトを表すプロジェクトテンプレート。[!UICONTROL 予算リクエスト]キュートのピックは、[!UICONTROL 予算リクエスト]カスタムフォームを使用するように割り当てられています。
* プロジェクトオブジェクトの&#x200B;**[!UICONTROL キャンペーンの概要]**&#x200B;フォーム。

  このフォームには、以下のフィールドが含まれている必要があります。

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>プロセスに適したオプションを含めます。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  カスタムフォームの作成について詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

## 想定される [!DNL Anaplan] の設定

このシナリオを使用するには、[!DNL Anaplan] に以下のものが必要です。

* **[!UICONTROL [!DNL Workfront]統合]**&#x200B;という名前の、システム管理者権限が付与されている [!DNL Anaplan] のユーザープロファイル。
* このシナリオで使用する [!DNL Anaplan] モデル。
* キャンペーン予算を取得する [!DNL Anaplan] モデル内のリスト。

  リストのモジュールは、次の属性の受信をサポートする必要があります。

   * [!UICONTROL Workfront プロジェクト GUID]
   * [!UICONTROL キャンペーン名]
   * [!UICONTROL 要求労働資金]
   * [!UICONTROL 要求費用資金]
   * [!UICONTROL 予算要求タイプ]
   * [!UICONTROL 資金調整の理由]

  このリストとモジュールには、予算を設定する機能や、予算リスト項目を [!DNL Workfront] に同期し直す準備ができていることを伝える機能など、[!DNL Anaplan] の通常の機能に追加する必要がある機能の詳細を保存する必要があります。

これらのアクションの手順については、[!DNL Anaplan] ドキュメントを参照してください。

## [!DNL Workfront Fusion] へのデプロイ

この統合シナリオを [!DNL Fusion] アカウントにデプロイするには、次の手順を実行します。これは、必要な [!DNL Workfront] と [!DNL Anaplan] の設定を完了した後にのみ実行してください。

1. [!DNL Workfront Fusion] の[!UICONTROL テンプレート]メニューに移動し、**[!UICONTROL Workfront 予算要求から [!DNL Anaplan] リスト項目を作成]**&#x200B;シナリオテンプレートをクリックします。
1. 次の [!DNL Anaplan] 変数の変数値を置換します。

   | 変数名 | 値を次のように置換します。 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ワークスペース ID] | [!DNL Anaplan] アカウントのワークスペースの ID。 |
   | [!UICONTROL [!DNL Anaplan] モデル ID] | [!DNL Anaplan] アカウントと選択したワークスペースのモデルの ID。 |
   | [!UICONTROL [!DNL Anaplan] モジュール名] | 選択した [!DNL Anaplan] リスト内のキャンペーン属性を説明するモジュールの名前。 |
   | [!UICONTROL キャンペーンリスト名] | [!DNL Anaplan] アカウントのリスト名、および選択したワークスペースとモデル。 |

   {style="table-layout:auto"}

   ファイルとプロセスの設定方法について詳しくは、[!DNL Anaplan] の設定ドキュメントを参照してください。

1. [!DNL Anaplan] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Anaplan] モジュールを [!DNL Anaplan] 接続で更新します。
1. [!DNL Workfront] 接続プロファイルを選択または追加します。

   テンプレートをデプロイした後、デフォルトで [!DNL Anaplan] にマッピングされたフィールドを変更する場合に、フィールドプロパティの値からカスタムフィールド参照を追加または削除するために更新するモジュールです。

1. プロンプトが表示されたら、残りのすべての [!DNL Workfront] モジュールを [!DNL Workfront] 接続で更新します。

## その他の推奨シナリオテンプレート

このテンプレートで表されるワークフローを完了するには、次の追加のテンプレートもデプロイする必要があります。

* [[!UICONTROL  [!DNL Anaplan]  予算配分を  [!DNL Adobe Workfront]  プロジェクトに適用します]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

支出を最適化するための追加のシナリオには次のものがあります。

* [[!UICONTROL  [!DNL Adobe Workfront]  プロジェクトの更新を  [!DNL Anaplan]  のリスト項目に送信します]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL  [!DNL Adobe Workfront]  の実際の時間の更新を  [!DNL Anaplan]  のリスト項目に送信します]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL  [!DNL Adobe Workfront]  の経費を  [!DNL Anaplan]  のリスト項目に送信します] ](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
