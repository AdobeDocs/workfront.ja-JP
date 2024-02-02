---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: ' [!DNL Anaplan]  予算配分を  [!DNL Adobe Workfront]  プロジェクトに適用する'
description: この統合シナリオは、 [!DNL Anaplan]  で行われた予算割り当てを  [!DNL Workfront] に同期します。シナリオでは、リンクされたキャンペーン予算項目をすべて取り込み、予算値が変更されている場合は、その予算値をリンクされた Workfront プロジェクトに渡します。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: ht
source-wordcount: '677'
ht-degree: 100%

---

# [!DNL Anaplan] 予算配分を [!DNL Adobe Workfront] プロジェクトに適用する

この統合シナリオは、[!DNL Anaplan] で行われた予算割り当てを [!DNL Workfront] に同期します。シナリオでは、リンクされたキャンペーン予算項目をすべて取り込み、予算値が変更されている場合は、その予算値をリンクされた [!DNL Workfront] プロジェクトに渡します。

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
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## イベントのトリガー

このシナリオは、15 分ごとに実行されるようにスケジュールされています。

## 期待される [!DNL Workfront] 設定

このシナリオを使用するには、[!DNL Workfront] に以下のものが必要です。

* **Anaplan Integration** という名前の [!DNL Workfront] のユーザープロファイル。システム管理者権限が付与されています。

  [!DNL Workfront] でのユーザーの作成について詳しくは、[ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

## 期待される [!DNL Anaplan] 設定

このシナリオを使用するには、[!DNL Anaplan] に以下のものが必要です。

* **[!DNL Workfront]統合**&#x200B;という名前の [!DNL Anaplan] のユーザープロファイル。システム管理者権限が付与されています。
* このシナリオに使用する [!DNL Anaplan] モデル。
* キャンペーン予算を取得する [!DNL Anaplan] モデル内のリスト。

  リストのモジュールは、次の属性の受信をサポートする必要があります。

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL キャンペーン名]
   * [!UICONTROL 要求労働資金]
   * [!UICONTROL 推定売上高]
   * [!UICONTROL ブランド]

  このリストとモジュールには、予算を設定し、予算リスト項目を [!DNL Workfront] に同期する準備ができていることを伝える機能など、[!DNL Anaplan] の通常の機能に必要な追加の詳細を保存する必要があります。

* [!DNL Anaplan] の&#x200B;**[!UICONTROL キャンペーンという名前のビュー。Adobe Workfront でキャンペーンを更新します]**。

  このビューには、以下の列がこの順序で含まれている必要があります。

   1. [!UICONTROL 項目名]

   2. [!UICONTROL [!DNL Workfront] プロジェクト GUID]

   3. [!UICONTROL キャンペーン名]

   4. [!UICONTROL 予算]

   5. [!UICONTROL 推定売上高]

   6. [!UICONTROL ブランド]

  [!UICONTROL [!DNL Workfront] プロジェクト GUID] を持つ項目と、予算割り当てを [!DNL Workfront] に送信する必要があることを示すインジケーターを表示するには、ビューをフィルタリングする必要があります。

これらのアクションの手順については、[!DNL Anaplan] ドキュメントを参照してください。

## [!DNL Workfront Fusion] へのデプロイ

この統合シナリオを [!DNL Fusion] アカウントにデプロイするには、次の手順を実行します。これは、必要な [!DNL Workfront] および [!DNL Anaplan] の設定を完了した後にのみ実行してください。

1. [!DNL Workfront Fusion] の[!UICONTROL テンプレート]メニューに移動し、**[!UICONTROL Workfront プロジェクトに [!DNL Anaplan] の予算割り当てを適用]**&#x200B;シナリオテンプレートをクリックします。
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Module Name]</td> 
      <td>選択した [!DNL Anaplan] リスト内のキャンペーン属性を説明するモジュールの名前。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>[!DNL Anaplan] アカウントのリスト名、および選択したワークスペースとモデル。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] View Name]</td> 
      <td> <p>[!DNL Workfront] にすぐに送信できるキャンペーン予算を含むビューの名前。</p> <p>（例：[!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]） </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ファイルとプロセスの設定方法について詳しくは、[!DNL Anaplan] の設定ドキュメントを参照してください。

1. [!DNL Anaplan] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Anaplan] モジュールを [!DNL Anaplan] 接続で更新します。
1. **[!UICONTROL CSV を JSON オブジェクトに変換モジュール]**&#x200B;で、CSV 列を使用可能な JSON オブジェクトにマッピングする新しいデータ構造を追加します。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. プロンプトが表示されたら、このシナリオのデプロイメントで他のモジュールに対してこのデータ構造を選択します。
1. **[!UICONTROL リンクされたプロジェクトを確認]**&#x200B;モジュールで、[!DNL Workfront] 接続プロファイルを選択または追加します。
1. プロンプトが表示されたら、残りのすべての [!DNL Workfront] モジュールを [!DNL Workfront] 接続で更新します。

## その他の推奨シナリオテンプレート

このテンプレートで表されるワークフローを完了するには、次の追加のテンプレートもデプロイする必要があります。

* [[!UICONTROL  [!DNL Adobe Workfront]  の予算リクエストから  [!DNL Anaplan]  リスト項目を作成]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

支出を最適化するための追加のシナリオには次のものがあります。

* [[!UICONTROL  [!DNL Adobe Workfront]  プロジェクトの更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL  [!DNL Adobe Workfront]  の実際の時間数の更新を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL  [!DNL Adobe Workfront]  の費用を  [!DNL Anaplan]  リスト項目に送信]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
