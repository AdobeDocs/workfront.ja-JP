---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion でシナリオを作成する
description: 次のタスクでは、 [!DNL Adobe Workfront Fusion] シナリオ。
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# でのシナリオの作成 [!DNL Adobe Workfront Fusion]

次のタスクでは、 [!DNL Adobe Workfront Fusion] シナリオ。

自動化シナリオの作成手順については、 [での自動化のプラクティスシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

指定したデータを使用して統合シナリオを作成する手順については、 [Adobe Workfront Fusion でのプラクティス統合シナリオの作成](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>テンプレートからシナリオを作成するには、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion] テンプレート](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## シナリオの作成を開始

1. クリック **[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックします。

1. クリック **[!UICONTROL 新しいシナリオの作成]** をクリックします。
1. 表示される画面（シナリオエディター）で、新しいシナリオを作成する場合は、「 **[!UICONTROL 新しいシナリオ]** 左上隅にシナリオの名前を入力します。
1. 続行： [シナリオへのモジュールの追加](#add-a-module-in-a-scenario).

## シナリオへのモジュールの追加

1. 最初のモジュールをシナリオに追加するには、疑問符アイコンをクリックします。 ![](assets/question-mark-icon.gif)

   または

   シナリオにモジュールを追加するには、追跡するモジュールの右側にあるハンドルをクリックします。

1. 表示されるボックスで、開始するアプリまたはサービスを探してクリックします。

   以前に選択したアプリは、簡単にアクセスできるようにボックスに表示され、 **[!UICONTROL お気に入り]** 」セクションを使用して、画面の下部に表示されます。

   次をクリックした場合： **[!UICONTROL 別のモジュールを追加]**&#x200B;表示されるモジュールは、シナリオでモジュールを追加する場所によって異なります。 他のモジュールの間にのみ配置できるモジュールもあれば、シナリオの最初にのみ配置できます。

   >[!TIP]
   >
   >最も一般的な 2 つのタイプのモジュールは、アクションとトリガーです。 詳しくは、 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md).

1. 表示されるモジュールのリストで、シナリオに追加する最初のモジュールをクリックします。

   表示されるモジュールは、シナリオでモジュールを追加する場所によって異なります。 他のモジュールの間にのみ配置できるモジュールもあれば、シナリオの最初にのみ配置できます。

   最も一般的な 2 つのタイプのモジュールは、アクションとトリガーです。 詳しくは、 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md).

1. 続行： [モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

アプリに接続するWorkfront Fusion モジュール ( [!DNL Workfront], [!DNL Salesforce]または [!DNL Jira)] 特集 [!UICONTROL 接続] フィールドに入力します。 ここで、このモジュールがアプリへの接続に使用する接続を指定できます。 ドロップダウンから既存の接続を選択するか、新しい接続を作成できます。

シナリオでアプリの接続を選択または作成すると、後のモジュールの設定時に別のモジュールを選択しない限り、そのアプリの他のモジュールは自動的に同じ接続を使用します。

詳しくは、 [接続について [!DNL Adobe Workfront Fusion] アプリまたはサービスに](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

内に接続を作成するには [!DNL Workfront Fusion] モジュール：

1. クリック **[!UICONTROL 追加]** 開く **[!UICONTROL 接続の作成]** ボックス
1. （オプション）デフォルトの **[!UICONTROL 接続名]**.
1. （条件付き）アプリに高度な接続設定 (ID、キー、 [!UICONTROL 秘密鍵]」に入力します。

   クリックが必要になる場合があります **[!UICONTROL 詳細設定を表示]** をクリックして、この種の情報を入力できるフィールドを表示します。

1. クリック **[!UICONTROL 続行]**.
1. 表示されるログインウィンドウで、アプリにログインするための資格情報を入力します（まだ入力していない場合）。
1. （条件付き） **[!UICONTROL 許可]** ボタンが表示され、コネクタが実行できるアクションを確認した後、ボタンをクリックしてアプリを [!DNL Workfront Fusion].
1. 続行： [モジュールの設定](#configure-the-module).


## モジュールの設定

1. 「接続」フィールドの下のフィールドで、モジュールの設定を指定し、 **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   これらの設定は、モジュールごとに異なります。 太字のタイトルは、必須の設定を示します。

   >[!TIP]
   >
   >シナリオの操作中は、モジュールをクリックすることで、いつでもこのボックスの設定を表示できます。
   >
   >
   >モジュールに黒い円が表示されている場合は、まだ設定が完了していません。 モジュールをクリックして開き、設定を続行します。
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. シナリオの最初のモジュールを追加する場合は、オプションを選択して、シナリオを実行するたびに開始する場所を指定します。

   ![](assets/choose-where-start-350x194.png)

1. セクションの手順を繰り返します。 [シナリオへのモジュールの追加](#add-a-module-in-a-scenario) および [モジュールの設定](#configure-the-module) をクリックして、他のモジュールをシナリオに追加します。

1. （オプション）モジュールまたはモジュールのグループをコピーして貼り付けます。

   詳しくは、 [Adobe Workfront Fusion でのモジュールまたはシナリオのコピー](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. 続行： [シナリオの設定と操作](#configure-and-work-with-your-scenario).

## シナリオの設定と操作

1. 次のいずれかの操作を行って、シナリオを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">シナリオを実行するタイミングと頻度を指定します</td> 
      <td> <p>時計アイコンをクリックします。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>詳しくは、 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">でのシナリオのスケジュール設定 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ルートの設定</td> 
      <td> <p>レンチアイコンをクリックします。 <img src="assets/wrench-icon.gif"> を 2 つのモジュールの間に挿入し、次のいずれかのオプションを使用します。 詳しくは、 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">のシナリオにフィルターを追加する [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL フィルターの設定 ]</strong>:シナリオの特定の時点で使用するバンドルを制御します。</li> 
        <li><strong>[!UICONTROL リンク解除 ]</strong>:ルートを削除します。</li> 
        <li><strong>[!UICONTROL ルーターの追加 ]</strong>:モジュール間にルータを追加します。 </li> 
        <li><strong>[!UICONTROL モジュールの追加 ]</strong>:モジュール間に新しいモジュールを追加します。</li> 
        <li><strong>[!UICONTROL メモを追加 ]</strong>:ルートにメモを追加します。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">シナリオの設定</td> 
      <td>[!UICONTROL シナリオ設定 ] アイコンをクリックします。 <img src="assets/gear-icon-settings.png"> これらの設定は主に上級ユーザー向けです。 詳しくは、 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">のシナリオ設定パネル [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">フロー制御の設定</td> 
      <td> <p>[!UICONTROL フロー制御 ] アイコンをクリックします。 <img src="assets/flow-control-icon.gif"> タスクを設定して、所定の回数を繰り返し、配列を一連のバンドルに変換し、複数のバンドルを 1 つのバンドルに結合できます。 詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">でのフロー制御 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">高度なツールを使用してシナリオを拡張する</td> 
      <td>次をクリック： [!DNL Tools] アイコン <img src="assets/tools-icon.gif"> トリガー、アクション、集約、変換サービスを作成できます。 詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">ツール</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーテキスト解析ツール</td> 
      <td>次をクリック： [!DNL Text parser] アイコン <img src="assets/text-parser-icon.gif">. HTMLコードから要素を取得し、検索パターンに一致する文字列要素を検索および抽出し、Web サイトから検索および置換し、「削除」を行うことができます。 詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">ツール</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. シナリオを操作するには、次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">シナリオの実行時に発生したイベントのログを表示します</td> 
      <td> <p>[!UICONTROL 編集を終了 ] 矢印をクリックします。 <img src="assets/exit-editing-arrow.png"> をクリックし、シナリオの詳細ページを表示します。 ログは、ウィンドウの下部または右下隅に表示されます。 このリストには、各フェーズに関する情報と、シナリオの実行中に発生したエラーが含まれます。</p> <p>次の手順で、 [!DNL scenario editor]、シナリオの詳細ページの任意の場所をクリックします。</p> <p>シナリオの詳細ページについて詳しくは、 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">シナリオの詳細 ( [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">最もよく使用するアプリやサービスへのアクセス</td> 
      <td> アイコンをクリックします。 <strong>[!UICONTROL お気に入り ]</strong> 」セクションを使用して、画面の下部に表示されます。 アプリやサービスをシナリオに追加すると、このセクションにアイコンが自動的に表示されます。 [!UICONTROL 追加 ] アイコン <img src="assets/add-icon.gif"> アプリやサービスをこの領域に手動で追加するには、次の手順に従います。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">データがシナリオをどのように流れるかを示すアニメーションを表示します</td> 
      <td>[!UICONTROL フローの説明を実行 ] アイコンをクリックします。 <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">モジュールのレイアウトを自動整列 </td> 
      <td>[!UICONTROL 自動整列 ] アイコンをクリックします。 <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">シナリオに関するメモを入力または表示します</td> 
      <td>[!UICONTROL メモ ] アイコンをクリックします。 <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">モジュールの削除</td> 
      <td>モジュールを右クリックし、 <strong>[!UICONTROL モジュールを削除 ]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. シナリオをテストして実行するには、 **[!UICONTROL 1 回実行]**.

   シナリオをアクティブ化する前に、シナリオが期待どおりに実行されることを確認することが重要です。 有効化されると、シナリオはスケジュールに従って実行されます。 すべてが期待どおりに動作しない場合は、 [でのエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. シナリオの編集が終了したら（または編集中にいつでも）、 [!UICONTROL 保存] ウィンドウ下部のアイコン ![](assets/save-icon.gif).

シナリオの有効化について詳しくは、 [でのシナリオのアクティブ化または非アクティブ化 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Workfront Fusion のシナリオのキーボードショートカット

シナリオの作成または編集時に、次のキーボードショートカットを使用できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>アクション</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 保存 ] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 1 回実行 ]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
