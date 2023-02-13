---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、OneDrive を使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL OneDrive]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL OneDrive] モジュールの場合、 [!DNL Microsoft OneDrive] アカウント

## 接続 [!DNL OneDrive] ～へのサービス [!DNL Workfront Fusion]

接続方法 [!DNL OneDrive] アカウント [!UICONTROL Workfront Fusion]を参照してください。 [への接続の作成 [!UICONTROL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] モジュールとそのフィールド

設定時に [!DNL OneDrive] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL OneDrive] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [ファイル/フォルダー](#filefolder)
* [その他](#other)

### ファイル/フォルダー

* [[!UICONTROL 監視ファイル/フォルダ]](#watch-filesfolders)
* [[!UICONTROL ファイル/フォルダを検索]](#search-filesfolders)
* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL ファイルのダウンロード]](#download-a-file)
* [[!UICONTROL ファイルのアップロード]](#upload-a-file)
* [[!UICONTROL フォルダーの作成]](#create-a-folder)
* [[!UICONTROL 共有リンクを取得]](#get-a-share-link)
* [[!UICONTROL ファイル/フォルダの移動]](#move-a-filefolder)
* [[!UICONTROL ファイルのコピー]](#copy-a-file)
* [[!UICONTROL ファイル/フォルダの削除]](#delete-a-filefolder)

#### [!UICONTROL 監視ファイル/フォルダ]

このトリガーモジュールは、ファイルまたはフォルダーが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 監視ファイル/フォルダー ]</td> 
   <td> <p>ファイルまたはフォルダの監視方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 作成日時別 ]</b> </p> <p>新しいファイルまたはフォルダーを監視します。</p> </li> 
     <li> <p><b>[!UICONTROL 更新時刻別 ]</b> </p> <p>更新された既存のファイルまたはフォルダーを監視します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>監視する場所を選択してください：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>モジュールが監視するドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> <p>モジュールを監視するフォルダーに移動します。 クエリを入力して、返された結果をフィルターすることもできます。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 自分と共有</b> </p> <p>モジュールは、ドライブの所有者と共有されたファイルを監視します。</p> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>モジュールで監視するSharePoint Site を選択します。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>モジュールを監視するドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 項目タイプの選択 ]</td> 
   <td> <p>ファイル、フォルダ、またはその両方を監視するかどうかを選択します。</p> <p>注意：[!UICONTROL Shared With Me] ドライブ内のフォルダーを監視することはできません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL ファイル/フォルダを検索]

この検索モジュールは、設定した条件に基づいてファイルおよびフォルダを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>検索する場所を選択してください：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>モジュールで検索するドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> <p>モジュールで検索するフォルダーに移動します。 クエリを入力して、返された結果をフィルターすることもできます。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 自分と共有</b> </p> <p>このモジュールは、ドライブの所有者と共有されているファイルを検索します。</p> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] モジュールで検索するサイトです。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>モジュールで検索するドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 項目タイプの選択 ]</td> 
   <td> <p>ファイル、フォルダ、またはその両方を検索するかどうかを選択します。</p> <p>注意：[!UICONTROL Shared With Me] ドライブ内のフォルダーは検索できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの取得]

このアクションモジュールは、指定されたファイルのメタデータを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter （ファイル ID およびファイルパス）]</td> 
   <td>ファイルをファイル ID で識別するか、ファイルパスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID を入力 ] / [!UICONTROL ファイルパス ]</td> 
   <td> <p>[ ファイル ID] または [ ファイルパス ] を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>検索する場所を選択してください：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>取得するファイルが含まれているドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>取得するファイルが含まれているSharePoint Site を選択します。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>取得するファイルが含まれているドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>取得するファイルが含まれているドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ] / [!UICONTROL ファイル ID] / [!UICONTROL ファイルパス ]</td> 
   <td> <p>[!UICONTROL Enter Manually] を選択した場合は、取得するファイルのファイル ID またはパスを入力またはマッピングします。</p> <p>[!UICONTROL リストから選択 ] を選択した場合、取得するファイルを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのダウンロード]

このアクションモジュールは、指定したファイルをダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter （ファイル ID およびファイルパス）]</td> 
   <td>ファイルをファイル ID で識別するか、ファイルパスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ファイル ID /ファイルパスを入力</td> 
   <td> <p>[ ファイル ID] または [ ファイルパス ] を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>ダウンロードするファイルを含む場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>ダウンロードするファイルが含まれるドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>ダウンロードするファイルが含まれているSharePoint Site を選択します。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>ダウンロードするファイルが含まれているドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>ダウンロードするファイルが含まれているドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ] / [!UICONTROL ファイル ID] / [!UICONTROL ファイルパス ]</td>
   <td> <p>[!UICONTROL Enter Manually] を選択した場合は、ダウンロードするファイルのファイル ID またはパスを入力またはマッピングします。</p> <p>[!UICONTROL リストから選択 ] を選択した場合、ダウンロードするファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROLPDFに変換 ]</td> 
   <td> <p>このオプションを有効にすると、ファイルがPDFファイルに変換されます。 次のファイルタイプから変換できます。</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>鍋</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、指定されたフォルダーにファイルをアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">（フォルダーの場所 ID とパス）を入力</td> 
   <td>ターゲットフォルダーを ID で識別するか、パスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>ファイルをアップロードする場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>取得するファイルが含まれているドライブを選択します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] ファイルをアップロードするフォルダーを含むサイト。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>ファイルをアップロードするフォルダを含むドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルをアップロードするフォルダーを含むドライブを選択します。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 同じ名前のファイルが存在する場合 ]</td> 
   <td>同じ名前のファイルが既に存在する場合の続行方法を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ]</td> 
   <td>アップロードしたファイルに説明を追加します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの作成]

このアクションモジュールは、指定されたドライブに新しいフォルダを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>フォルダーを作成する場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>フォルダを作成するドライブを選択します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] フォルダーを作成するサイトです。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>フォルダを作成するドライブを所有するグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>フォルダを作成するドライブを選択します。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>新しいフォルダをサブフォルダにする場合は、サブフォルダにするフォルダに移動します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新規フォルダー名 ]</td> 
   <td> <p>新しいフォルダの名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 同じ名前のフォルダが存在する場合 ]</td> 
   <td>同じ名前のファイルが既に存在する場合の続行方法を選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有リンクを取得]

このアクションモジュールは、指定されたファイルの共有リンクを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter （ファイル ID およびファイルパス）]</td> 
   <td>ファイルをファイル ID で識別するか、ファイルパスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID を入力 ] / [!UICONTROL ファイルパス ]</td> 
   <td> <p>[ ファイル ID] または [ ファイルパス ] を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>共有リンクを取得する場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>共有リンクを取得するファイルが含まれるドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>共有リンクを取得するファイルが含まれているSharePointサイトを選択します。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>共有リンクを取得するファイルが含まれるドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>共有リンクを取得するファイルが含まれるドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ] / [!UICONTROL ファイル ID] / [!UICONTROL ファイルパス ]</td> 
   <td> <p>[!UICONTROL Enter Manually] を選択した場合は、共有リンクを取得するファイルのファイル ID またはパスを入力またはマッピングします。</p> <p>リストから「[!UICONTROL 選択 ]」を選択した場合、共有リンクを取得するファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 権限のタイプ ]</td> 
   <td> <p>リンクを持つユーザーがファイルの読み取りと書き込みを行えるようにするか、読み取り専用にするかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スコープ ]</td> 
   <td>リンクを持つすべてのユーザーがファイルを使用できるようにするか、リンクを持つ組織のメンバーのみがファイルを使用できるようにするかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダの移動]

このアクションモジュールは、ファイルまたはフォルダを新しいフォルダの場所に移動します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter （ファイル ID およびファイルパス）]</td> 
   <td>ファイルをファイル ID で識別するか、ファイルパスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID /ファイルパスを入力 ]</td> 
   <td> <p>[ ファイル ID] または [ ファイルパス ] を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>移動するファイルまたはフォルダを含む場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>移動するファイルまたはフォルダが含まれるドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] 移動するファイルまたはフォルダを含むサイト。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>移動するファイルまたはフォルダが含まれるドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>移動するファイルまたはフォルダを含むドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル/フォルダー ] を選択</td> 
   <td>ファイルを移動するか、フォルダを移動するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL ファイル ] / [!UICONTROL ファイル ID] / [!UICONTROL ファイルパス ]</p> <p role="rowheader">[!UICONTROL フォルダー ] / [!UICONTROL フォルダー ID] / [!UICONTROL フォルダーパス ]</p> </td> 
   <td> <p>[!UICONTROL Enter Manually] を選択した場合は、移動するファイルまたはフォルダーの ID またはパスを入力またはマッピングします。</p> <p>リストから [!UICONTROL 選択 ] を選択した場合、移動するファイルまたはフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しいフォルダーの場所を入力 ]</td> 
   <td> <p>ファイルまたはフォルダの移動先を入力する方法を選択してください：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>ファイルまたはフォルダーを移動する場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>ファイルまたはフォルダを移動するドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] ファイルまたはフォルダーを移動するサイト。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>ファイルまたはフォルダを移動するドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルまたはフォルダの移動先のフォルダが含まれるドライブを選択またはマップします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> <p>このオプションを空白のままにした場合、同じ [!DNL OneDrive].</p> <p>[!UICONTROL マイドライブ ] から [!UICONTROL サイトのドライブ ] または [!UICONTROL グループのドライブ ] にファイルやフォルダを移動できます。 </p> <p>ファイルを [!UICONTROL Site's Drive] から同じ Site 内の同じドライブにのみ移動できます。</p> <p>ファイルを [!UICONTROL グループのドライブ ] から移動できるのは、同じグループ内の同じドライブだけです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>ファイルまたはフォルダを移動するフォルダを入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのコピー]

このアクションモジュールは、新しいフォルダーの場所にファイルをコピーします

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter （ファイル ID およびファイルパス）]</td> 
   <td>ファイルをファイル ID で識別するか、ファイルパスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID を入力 ] / [!UICONTROL ファイルパス ]</td> 
   <td> <p>[ ファイル ID] または [ ファイルパス ] を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>コピーするファイルを含む場所を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>コピーするファイルまたはフォルダを含むドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>移動するファイルが含まれているSharePointサイトを選択します。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>コピーするファイルが含まれるドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>コピーするファイルを含むドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL ファイル ] / [!UICONTROL ファイル ID] / [!UICONTROL ファイルパス ]</p> </td> 
   <td> <p>[!UICONTROL Enter Manually] を選択した場合は、コピーするファイルの ID またはパスを入力またはマッピングします。</p> <p>リストから [!UICONTROL 選択 ] を選択した場合、コピーするファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しいフォルダーの場所を入力 ]</td> 
   <td> <p>ファイルをコピーする場所を入力する方法を選択するか、次の操作を行います。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なフォルダーのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しい OneDrive の場所 ]</td> 
   <td> <p>フィルタをコピーする場所を選択します。 このオプションは、リストから新しいフォルダーの場所を選択した場合に使用できます。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>ファイルをコピーするドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] ファイルをコピーするサイト。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>ファイルをコピーするドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルのコピー先のフォルダを含むドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> <p>このオプションを指定しない場合、ファイルまたはフォルダーは同じ [!UICONTROL OneDrive] 内でのみコピーできます。</p> <p>[!UICONTROL マイドライブ ] から [!UICONTROL サイトのドライブ ] または [!UICONTROL グループのドライブ ] にファイルおよびフォルダーをコピーできます。 </p> <p>ファイルを [!UICONTROL サイトのドライブ ] からコピーできるのは、同じサイトの同じドライブだけです。</p> <p>ファイルを [!UICONTROL グループのドライブ ] からコピーできるのは、同じグループ内の同じドライブだけです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>コピーまたはフォルダーを移動するフォルダーを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新しくコピーされたファイル名 ]</td> 
   <td> <p>ファイルの新しいコピーの名前を入力またはマッピングします。 元のファイル名を変更しない場合は、この値を空白のままにすることができます。</p> <p>名前にはファイル拡張子を含める必要があります。 例:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダの削除]

このアクションモジュールは、選択したファイルを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter （ファイル/フォルダー ID およびパス）]</td> 
   <td>ファイルをファイル ID で識別するか、ファイルパスで識別するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル/フォルダー ID を入力/ファイル/フォルダーパスを入力 ]</td> 
   <td> <p>[ ファイル ID] または [ ファイルパス ] を入力する方法を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 手動で入力 ]</b> </p> <p>ID またはパスを直接入力する場合、または以前のモジュールからマッピングする場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL リストから選択 ]</b> </p> <p>使用可能なファイルまたはパスのリストから選択する場合は、このオプションを選択します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL [!DNL OneDrive] location]</td> 
   <td> <p>検索する場所を選択してください：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL マイドライブ ]</b> </p> <p>モジュールがドライブ ID を入力できるようにするかどうかを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL はい ]</b> </p> <p>削除するファイルまたはフォルダが含まれるドライブの ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL いいえ ]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL サイトのドライブ ]</b> </p> <p>を選択します。 [!DNL SharePoint] 削除するファイルまたはフォルダを含むサイト。 利用可能なサイトは、サイトに続くサインインしたユーザーです。</p> </li> 
     <li> <p><b>[!UICONTROL グループのドライブ ]</b> </p> <p>削除するファイルまたはフォルダが含まれるドライブのグループを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドライブ ID]</td> 
   <td> <p>削除するファイルまたはフォルダを含むドライブを選択またはマッピングします。 [!UICONTROL Enable to Enter a Drive ID] フィールドで [!UICONTROL No] を選択した場合、このフィールドは使用できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル/フォルダー ] を選択</td> 
   <td>ファイルを削除するか、フォルダを削除するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ] / [!UICONTROL ファイル ID] / [!UICONTROL ファイルパス ]</td>
   <td> <p>[!UICONTROL Enter Manually] を選択した場合は、削除するファイルのファイル ID またはパスを入力またはマッピングします。</p> <p>リストから [!UICONTROL 選択 ] を選択した場合、削除するファイルを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

#### [!UICONTROL API 呼び出しを実行する]

このモジュールは、カスタム API 呼び出しを実行します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL OneDrive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://graph.microsoft.com</code>. 例:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は、認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## ファイルをアップロードまたは更新できない場合

ファイルのアップロードまたは更新が失敗した場合は、次のような問題が発生する可能性があります。

* アップロードされたファイルが大きすぎて、ファイルサイズの上限を超えています [!DNL OneDrive] プランまたはすべての [!DNL OneDrive] アカウントのストレージクォータ。 より多くのストレージ領域を取得するには、次の場所から既存のファイルを削除します： [!DNL OneDrive] または、 [!DNL OneDrive] アカウント
* OneDrive では、同じ名前の 2 つのファイルを 1 つのフォルダにアップロードできません。 アップロード先のフォルダに、アップロード先のファイルと同じ名前のファイルが含まれている場合、シナリオの実行はエラーで終了します。 解決策は、アップロードするファイルの名前を変更するだけです。 ファイルを更新する場合は、 [!UICONTROL ファイルの更新] アクション。
* 以前に選択したフォルダー（ファイルのアップロード先）は存在しません。 シナリオが停止し、ターゲットフォルダーを再度選択する必要があります。
