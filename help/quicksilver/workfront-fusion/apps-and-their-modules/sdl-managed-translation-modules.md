---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: SDL Managed Translation モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、SDL Managed Translation アカウントをサードパーティの複数のアプリケーションとサービスに接続できます。'
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '529'
ht-degree: 100%

---

# [!DNL SDL Managed Translation] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL SDL Managed Translation] アカウントを複数のサードパーティのアプリケーションとサービスに接続できます。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront]プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL SDL Managed Translation] モジュール

>[!NOTE]
>
>[!DNL SDL Managed Translation] の呼び出し操作のタイムアウトは **120 秒**&#x200B;です。

### ファイル

#### [!UICONTROL 翻訳済みファイルをダウンロード]

このモジュールは、指定されたプロジェクトに含まれる、1 つの翻訳済みファイルの内容を取得します。要求されたファイルがダウンロードのステータスになっていない場合、ファイルの内容がまだ完全に翻訳されていない可能性があります。ファイルがダウンロードのステータスであり、そのファイルを正常に取得した場合は、必ず `Cancel or Complete File` メソッドを使用してファイルを完了としてマークしてください。

#### [!UICONTROL ファイルをアップロード]

このモジュールでは、翻訳用のファイル、または翻訳プロジェクトに含めるファイルを参照資料としてアップロードできます。アップロードは multipart/form-data を使用して送信する必要があり、ファイルを複数含めることができます。アップロードされたファイルの評価に使用する `ProjectOptionId` を指定します。これにより、アップロードする各ファイルが翻訳の候補として考えられるか、参照資料として処理する必要があるかが決まります。アーカイブ（`zip `、`rar`、`7z`、`tar` ファイル）の場合、アプリはアーカイブの内容を調べ、アーカイブ全体を翻訳できるかどうか、または翻訳可能なファイルと翻訳不可のファイルが混在しているかどうかを示します。

>[!NOTE]
>
>一度に複数のファイルをアップロードすることは、エラーの影響を大きくする可能性があるので、お勧めしません。

#### [!UICONTROL 参照ファイルを追加]

このモジュールは、参照ファイルを追加します。

### プロジェクト

#### [!UICONTROL プロジェクトの作成]

このモジュールは、指定されたプロジェクトを作成します。

#### プロジェクトをキャンセルまたは完了

このモジュールは、指定されたプロジェクトをキャンセルまたは完了します。プロジェクトがダウンロード待ちの場合、プロジェクトはワークフローの最終ステップを経て遷移し、最終的に完了に移ります。プロジェクトが承認待ちの場合、またはベンダーの選択がキャンセルされた場合。プロジェクトがその他のステータスの場合、リクエストは失敗します。

#### [!UICONTROL プロジェクト Zip をダウンロード]

このモジュールは、指定されたプロジェクトの翻訳済みファイルの `zip` ファイルを取得します。

#### [!UICONTROL プロジェクトの読み取り]

このモジュールは、指定されたプロジェクトを取得します。

#### [!UICONTROL 特定ステータスのプロジェクトの取得]

このモジュールは、指定されたステータスにあるすべての使用可能なプロジェクトを取得します。このメソッドでは、`$top`、`$skip` および `$orderby` のクエリパラメーターを指定することで、結果をページ分割することができます。

#### [!UICONTROL プロジェクトリストの取得]

すべてのプロジェクトの単純なリストを取得し、各プロジェクトに関する一般情報を提供します。このメソッドでは、`$top`、`$skip` および `$orderby` のクエリパラメーターを指定することで、結果をページ分割することができます。

#### [!UICONTROL プロジェクト作成オプションの検索]

このモジュールは、プロジェクト作成オプションを取得します。

### その他

#### [!UICONTROL API 呼び出しの実行]

このモジュールは、許可された任意の API 呼び出しを実行します。
