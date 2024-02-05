---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe]  Workfront Fusion のシナリオエディター'
description: シナリオエディターを使用すると、視覚的なインターフェイスでシナリオを作成および編集できます。
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 28ca9bab8d6a5aed395dc3297eb62912ebb506c7
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 97%

---

# [!DNL Adobe Workfront Fusion] のシナリオエディター

シナリオエディターを使用すると、視覚的なインターフェイスでシナリオを作成および編集できます。

![](assets/scenario-editor-350x228.jpg)

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## シナリオエディターを開きます。

1. 左側のパネルで&#x200B;**[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックします。

1. シナリオを作成する場合は、ページの右上隅にある「**[!UICONTROL 新しいシナリオを作成]**」をクリックします。

   または

   既存のシナリオを編集する場合は、シナリオをクリックします。

   表示されるシナリオエディターで、次の表に示す操作をすべて実行できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でシナリオを作成を参照してください。

1. シナリオの編集が終了したら（または編集中に任意の時点で）、[!UICONTROL 保存] アイコン ![](assets/save-icon.gif) をクリックします。

   >[!NOTE]
   >
   >シナリオを保存した後、将来アクセスする必要がある場合、「...」メニューから新しいバージョンを使用できます。以前に保存したシナリオのバージョンは 60 日間のみ使用できます。

## 使用可能なシナリオエディターのアクション

シナリオエディターでは、次のアクションを使用できます。

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">最初のモジュールを追加する</td>
     <td> <p>疑問符アイコンをクリックします。 <img src="assets/question-mark-full-size.png"></p> <p> 次に、開始するアプリまたはサービスを見つけてクリックします。手順 2 で任意のアプリを選択した場合、簡単にアクセスできるように、ここに（および画面下部の「<strong>[!UICONTROL Favorites]</strong>」セクションに）表示されます。</p> </td>
  </tr>
  <tr>
     <td role="rowheader">モジュールを追加する</td>
     <td>モジュールの上にポインタを合わせて、右側に表示されるプラスアイコンをクリックし、表示されるメニューで目的のモジュールをクリックします。</td>
  </tr>  
  <tr>   
     <td role="rowheader">シナリオを実行するタイミングと頻度を指定</td>  
      <td> <p>時計アイコンをクリックします。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>詳しくは、<a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオをスケジュールを参照してください。</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">ルートを設定</td>   
     <td> <p>2 つのモジュールの間にある [!UICONTROL wrench] アイコン <img src="assets/wrench-icon.gif"> をクリックして、次のいずれかのオプションを使用します。</p>    
       <ul>
         <li><strong>[!UICONTROL Set up a filter]</strong>：シナリオの特定の時点で使用されるバンドルを制御します。詳しくは、<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> のシナリオにフィルターを追加するを参照してください。</li>     
         <li><strong>[!UICONTROL Unlink]</strong>：ルートを削除します。</li>     
         <li><strong>[!UICONTROL Add a router]</strong>：モジュール間にルーターを追加します。 </li>     
         <li><strong>[!UICONTROL Add a module]</strong>：モジュール間に新規モジュールを追加します。</li>     
         <li><strong>[!UICONTROL Add a note]</strong>：ルートにメモを追加します。</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">モジュールを削除</td>   
     <td>モジュールを右クリックし、次に「<strong>[!UICONTROL Delete module]</strong>」をクリックします。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">シナリオで発生したイベントのログを表示する</td>     
     <td> 
       <p>シナリオを実行します。シナリオの実行が終了すると、ログが [!UICONTROL Scenario Editor] の右下隅に表示されます。 </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>シナリオに応じて、ログには各フェーズの難易度やシナリオの実行中に発生したエラーに関する情報が含まれる場合があります。</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">シナリオ設定を行います。</td>   
     <td>[!UICONTROL Scenario settings] アイコンをクリックします。<img src="assets/gear-icon-settings.png">これらの設定は主に上級ユーザー向けです。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">シナリオに関するメモを入力または表示</td>   
     <td>「[!UICONTROL Notes]」アイコンをクリックします。 <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">モジュールのレイアウトを自動整列 </td>   
     <td>「[!UICONTROL Auto-align]」アイコンをクリックします。 <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">シナリオ内のデータの流れを示すアニメーションを表示</td>   <td>「[!UICONTROL Explain flow]」アイコンをクリックします。 <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">シナリオをコンピューターにブループリントとして書き出す</td>   
     <td>[!UICONTROL More] メニュー <img src="assets/more-icon.png"> をクリックして、「[!UICONTROL Export Blueprint]」をクリックします。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">コンピューターからシナリオのブループリントを読み込む</td>   
     <td>[!UICONTROL More] メニュー <img src="assets/more-icon.png"> をクリックして、「[!UICONTROL Import Blueprint]」をクリックします。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">シナリオの以前のバージョンを復元する</td>   
     <td><a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオバージョンを復元の記事を参照してください。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">[!UICONTROL Flow Control] の設定を行う</td>   
     <td> <p>[!UICONTROL Flow Control] アイコンをクリックします。<img src="assets/flow-control-icon.gif">タスクを所定の回数繰り返すように設定したり、配列を一連のバンドルに変換したり、複数のバンドルを 1 つのバンドルに結合したりすることができます。詳しくは、<a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのフロー制御を参照してください。</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">高度なツールを使用してシナリオを拡張する</td>   
     <td>「[!UICONTROL Tools]」アイコンをクリックします。<img src="assets/tools-icon.gif">トリガー、アクション、集約、変換サービスを作成できます。詳しくは、<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">ツール</a>を参照してください。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">テキスト解析ツールを使用する</td>   
     <td>「[!UICONTROL Text parse]」アイコンをクリックします。<img src="assets/text-parser-icon.gif">HTML コードから要素の取得、検索パターンに一致する文字列要素の検索および抽出、テキストの検索および置換、web サイトからデータの「スクレイピング」を行うことができます。詳しくは、<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">ツール</a>を参照してください。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">最もよく使用するアプリやサービスにアクセス</td>   
     <td> 画面下部の「<strong>[!UICONTROL Favorites]</strong>」セクションにあるアイコンをクリックします。アプリやサービスをシナリオに追加すると、このセクションにアイコンが自動的に表示されます。追加アイコン <img src="assets/add-icon.gif"> をクリックすると、このエリアにアプリとサービスを手動で追加することもできます。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">シナリオのテスト実行を行う</td>   
     <td>「<strong>[!UICONTROL Run once]</strong>」をクリックして、シナリオをアクティブ化する前に、シナリオが期待どおりに実行されることを確認します。アクティブ化すると、シナリオはスケジュールに従って実行されます。すべてが期待どおりに実行されない場合は、エラー処理の方法について、エラー処理の節を参照してください。</td> 
   </tr> 
   <tr> 
     <td role="rowheader">開発ツールを使用したシナリオのデバッグ</td>   
     <td>詳しくは、 <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">でのシナリオのデバッグ [!DNL Adobe Workfront Fusion] 開発者ツール</a>.
</td> 
   </tr> 
</tbody>
</table>
