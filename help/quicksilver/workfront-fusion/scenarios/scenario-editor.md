---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: のシナリオエディター [!DNL Adobe] Workfront Fusion
description: シナリオエディターを使用すると、視覚的なインターフェイスでシナリオを作成および編集できます。
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 27db607fd0543b06a502032a9b6b0c88d4ecec41
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 1%

---

# のシナリオエディター [!DNL Adobe Workfront Fusion]

シナリオエディターを使用すると、視覚的なインターフェイスでシナリオを作成および編集できます。

![](assets/scenario-editor-350x228.jpg)

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## シナリオエディターを開きます。

1. クリック **[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックします。

1. シナリオを作成する場合は、「 **[!UICONTROL 新しいシナリオの作成]** をクリックします。

   または

   既存のシナリオを編集する場合は、シナリオをクリックします。

1. （条件付き）新しいシナリオを作成する場合、「 **[!UICONTROL 統合するサービス]**」で、シナリオで使用するアプリを選択し、 **[!UICONTROL 続行]**.

   または

   クリック **[!UICONTROL スキップ]** シナリオエディター内からアプリを選択する場合。

   表示されるシナリオエディターで、次の表に示す操作をすべて実行できます。 詳しくは、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. シナリオの編集が終了したら（または編集中に任意の時点で）、 [!UICONTROL 保存] アイコン ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >シナリオを保存すると、将来アクセスする必要が生じた場合に備えて、3 ドットメニューで新しいバージョンを使用できるようになります。 以前に保存したシナリオのバージョンは 60 日間のみ使用できます。

## 使用可能なシナリオエディターのアクション

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">最初のモジュールを追加</td>
     <td> <p>疑問符アイコンをクリックします。 <img src="assets/question-mark-full-size.png"></p> <p> 次に、開始するアプリまたはサービスを見つけてクリックします。 手順 2 で任意のアプリを選択した場合、簡単にアクセスできるよう、ここに表示されます ( および <strong>[!UICONTROL お気に入り ]</strong> 」セクションに表示されます )。</p> </td>
  </tr>
  <tr>
     <td role="rowheader">モジュールの追加</td>
     <td>モジュールの上にマウスポインターを置き、右側に表示されるプラスアイコンをクリックし、表示されるメニューで目的のモジュールをクリックします。</td>
  </tr>  
  <tr>   
     <td role="rowheader">シナリオを実行するタイミングと頻度を指定します</td>  
      <td> <p>時計アイコンをクリックします。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>詳しくは、 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">でのシナリオのスケジュール設定 [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">ルートの設定</td>   
     <td> <p>[!UICONTROL レンチ ] アイコンをクリックします。 <img src="assets/wrench-icon.gif"> を 2 つのモジュール間で切り替え、次のいずれかのオプションを使用します。</p>    
       <ul>
         <li><strong>[!UICONTROL フィルターの設定 ]</strong>:シナリオの特定の時点で使用するバンドルを制御します。 詳しくは、 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">のシナリオにフィルターを追加する [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL リンク解除 ]</strong>:ルートを削除します。</li>     
         <li><strong>[!UICONTROL ルーターの追加 ]</strong>:モジュール間にルータを追加します。 </li>     
         <li><strong>[!UICONTROL モジュールの追加 ]</strong>:モジュール間に新しいモジュールを追加します。</li>     
         <li><strong>[!UICONTROL メモを追加 ]</strong>:ルートにメモを追加します。</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">モジュールの削除</td>   
     <td>モジュールを右クリックし、 <strong>[!UICONTROL モジュールを削除 ]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">発生したイベントのログを表示します（シナリオ）</td>     
     <td> 
       <p>シナリオを実行します。 シナリオの実行が終了すると、ログが [!UICONTROL シナリオエディター ] の右下隅に表示されます。 </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>シナリオに応じて、ログには、各フェーズの困難性に関する情報や、シナリオの実行中に発生したエラーに関する情報が記録される場合があります。</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">シナリオの設定</td>   
     <td>[!UICONTROL シナリオ設定 ] アイコンをクリックします。 <img src="assets/gear-icon-settings.png"> これらの設定は主に上級ユーザー向けです。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">シナリオに関するメモを入力または表示します</td>   
     <td>[!UICONTROL メモ ] アイコンをクリックします。 <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">モジュールのレイアウトを自動整列 </td>   
     <td>[!UICONTROL 自動整列 ] アイコンをクリックします。 <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">データがシナリオをどのように流れるかを示すアニメーションを表示します</td>   <td>「[!UICONTROL フローの説明を実行」アイコンをクリックします。 <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">シナリオをコンピューターにブループリントとしてエクスポート</td>   
     <td>[!UICONTROL その他 ] メニューをクリックします。 <img src="assets/more-icon.png">をクリックし、「[!UICONTROL ブループリントを書き出し ]」をクリックします。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">コンピューターからシナリオのブループリントを読み込む</td>   
     <td>[!UICONTROL その他 ] メニューをクリックします。 <img src="assets/more-icon.png">をクリックし、「 [!UICONTROL ブループリントを読み込み」をクリックします。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">シナリオの以前のバージョンを復元します</td>   
     <td>この記事を参照してください <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">でのシナリオバージョンの復元 [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">[!UICONTROL フロー制御 ] の設定</td>   
     <td> <p>[!UICONTROL フロー制御 ] アイコンをクリックします。 <img src="assets/flow-control-icon.gif"> タスクを設定して、所定の回数を繰り返し、配列を一連のバンドルに変換し、複数のバンドルを 1 つのバンドルに結合できます。 詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">でのフロー制御 [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">高度なツールを使用してシナリオを拡張する</td>   
     <td>[!UICONTROL ツール ] アイコンをクリックします。 <img src="assets/tools-icon.gif"> トリガー、アクション、集約、変換サービスを作成できます。 詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">ツール</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">テキスト解析ツールの使用</td>   
     <td>[!UICONTROL テキストパーサー ] アイコンをクリックします。 <img src="assets/text-parser-icon.gif"> HTMLコードから要素を取得し、検索パターンに一致する文字列要素を検索および抽出し、Web サイトから検索および置換し、「削除」を行うことができます。 詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">ツール</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">最もよく使用するアプリやサービスへのアクセス</td>   
     <td> アイコンをクリックします。 <strong>[!UICONTROL お気に入り ]</strong> 」セクションを使用して、画面の下部に表示されます。 アプリやサービスをシナリオに追加すると、このセクションにアイコンが自動的に表示されます。 「追加」アイコン <img src="assets/add-icon.gif"> アプリやサービスをこの領域に手動で追加するには、次の手順に従います。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">シナリオのテスト実行</td>   
     <td>クリック <strong>[!UICONTROL 1 回実行 ]</strong> を使用して、シナリオをアクティブ化する前に、期待どおりに実行されることを確認します。 有効化されると、シナリオはスケジュールに従って実行されます。 すべてが期待どおりに実行されない場合は、エラー処理の方法について、エラー処理の節を参照してください。</td> 
   </tr> 
</tbody>
</table>
