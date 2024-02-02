---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive for Business モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Microsoft OneDrive for Business] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1087'
ht-degree: 100%

---

# [!DNL Microsoft OneDrive for Business] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Microsoft OneDrive for Business] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

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
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Adobe Workfront Fusion] の [!DNL Microsoft OneDrive for Business] を使用するには、[!DNL Microsoft] アカウントを必要とします。

[!DNL OneDrive for Business] アカウントの [!DNL Workfront Fusion] への接続について詳しくは、[Adobe  [!DNL Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

## [!DNL Microsoft OneDrive for Business] モジュールとそのフィールド

[!DNL Microsoft OneDrive for Business] モジュールの設定時に、[!DNL Workfront Fusion] に、以下のフィールドが表示されます。これらと共に、アプリやサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Microsoft OneDrive for Business] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

* [[!UICONTROL ファイルを監視]](#watch-files)
* [[!UICONTROL フォルダーを監視]](#watch-folders)

#### [!UICONTROL ファイルを監視]

このトリガーモジュールは、監視対象のフォルダーに新しいファイルが追加または更新されると、アクティブ化されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントの [!DNL Workfront Fusion] への接続について詳しくは、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事内の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスの [!DNL Workfront Fusion]</a> への接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>監視するドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> 監視するフォルダーを選択します。1 つのシナリオでは、監視できるフォルダーは 1 つだけです。</p> <p>ヒント：複数のフォルダーをトラックするには、各フォルダーに対して個別のシナリオを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL I want to watch]</p> </td> 
   <td> <p>新しいファイルとすべての変更を監視するか、新しいファイルのみを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned rows]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 サイクルの間に連携する結果の最大数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーを監視]

このトリガーモジュールは、監視対象のフォルダーに新しいフォルダーが追加されるとアクティブになります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオを作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">[!DNL Workfront Fusion]</a> にモジュールのアプリまたは web サービスを接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Drive ID]</p> </td> 
   <td> <p>監視するドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p> 監視するフォルダーを選択します。1 つのシナリオでは、監視できるフォルダーは 1 つだけです。</p> <p>ヒント：複数のフォルダーをトラックするには、各フォルダーに対して個別のシナリオを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL I want to watch]</p> </td> 
   <td> <p>新規フォルダーとすべての変更を監視するか、新規フォルダーのみを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned rows]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 サイクルの間に連携する結果の最大数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL ファイルをアップロード]](#upload-a-file)
* [[!UICONTROL ファイルを削除]](#delete-a-file)
* [[!UICONTROL ファイルを取得]](#get-a-file)
* [[!UICONTROL フォルダーを作成]](#create-a-folder)
* [[!UICONTROL フォルダーを削除]](#delete-a-folder)
* [[!UICONTROL 共有リンクを取得]](#get-a-sharing-link)

#### [!UICONTROL ファイルをアップロード]

このアクションモジュールは、指定されたフォルダーにバイナリまたはテキストファイルをアップロードします

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオを作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">[!DNL Workfront Fusion]</a> にモジュールのアプリまたは web サービスを接続を参照してください。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>ファイルのアップロード先のドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>ドライブ内のフォルダーを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL If the file with the same name exists]</td> 
   <td> <p> アップロードしようとしているファイルと同じ名前のファイルが既に存在する場合に実行する操作を選択します。</p> 
    <ul> 
     <li>[!UICONTROL Replace the existing file]</li> 
     <li>[!UICONTROL Rename the new file]</li> 
     <li>[!UICONTROL End with an error]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを削除]

このアクションモジュールは、指定されたファイルをごみ箱に移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオを作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">[!DNL Workfront Fusion]</a> にモジュールのアプリまたは web サービスを接続を参照してください。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>ファイルを削除するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>削除するファイルの ID を入力します。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを取得]

このアクションモジュールは、指定された ID を持つファイルを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオを作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">[!DNL Workfront Fusion]</a> にモジュールのアプリまたは web サービスを接続を参照してください。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>ファイルを取得するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td> <p>取得するファイルの ID を入力します。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーを作成]

指定された親フォルダー内にフォルダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Connection]</strong> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順について詳しくは、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でシナリオを作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Drive ID]</strong> </td> 
   <td> <p>新しいフォルダーを作成するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder]</strong> </td> 
   <td> <p>新しいフォルダーを作成するフォルダーを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Folder name]</strong> </td> 
   <td>新しいフォルダーの名前を入力またはマッピングします。</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーを削除]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順について詳しくは、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>ファイルを削除するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder ID]</td> 
   <td> <p>削除するフォルダーの ID を入力またはマッピングします。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有リンクを取得]

このモジュールは、指定されたファイルにアクセスするために共有できるリンクを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Drive ID]</td> 
   <td> <p>ファイルのアップロード先のドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>ファイル ID を使用してファイルを選択するか、ファイルパスを使用してファイルを選択するかを選択します。表示されるフィールドに、ファイル ID またはファイルパスを入力します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permission type]</p> </td> 
   <td> <p>リンクを受け取ったユーザーがファイルの読み取りと書き込みを行えるようにするか、読み取り専用にするかを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope]</td> 
   <td> <p> リンクを持つすべてのユーザーがファイルにアクセスできるようにするか、組織のメンバーのみがファイルにアクセスできるようにするかを選択します。</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
