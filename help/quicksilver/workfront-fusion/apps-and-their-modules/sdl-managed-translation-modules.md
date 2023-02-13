---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: SDL Managed Translation モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合は、SDL Managed Translation アカウントを複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオに従って、 [!DNL SDL Managed Translation] を複数のサードパーティのアプリケーションおよびサービスにアカウントする。

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

## [!DNL SDL Managed Translation] モジュール

>[!NOTE]
>
>への呼び出しの操作タイムアウト [!DNL SDL Managed Translation] が **120 秒**.

### ファイル

#### [!UICONTROL 翻訳済みファイルをダウンロード]

このモジュールは、指定されたプロジェクトに含まれる単一の翻訳済みファイルのコンテンツを取得します。 要求されたファイルが Downland ステータスになっていない場合、ファイルのコンテンツがまだ完全に翻訳されていない可能性があります。 ファイルが「ダウンロード」ステータスで、正常に取得された場合は、必ず `Cancel or Complete File` メソッド。

#### [!UICONTROL ファイルのアップロード]

このモジュールでは、翻訳用または翻訳プロジェクトに含めるファイルを参照資料としてアップロードできます。 アップロードは multipart/form-data を使用して送信する必要があり、複数のファイルを含めることができます。 次を指定します。 `ProjectOptionId` を使用して、アップロードされたファイルを評価する必要があります。 これにより、アップロードする各ファイルが翻訳の候補として考えられるか、参照資料として処理する必要があるかが決まります。 アーカイブ (`zip `, `rar`, `7z`, `tar` ファイル ) アプリはアーカイブの内容を調べ、アーカイブ全体を翻訳できるかどうか、または翻訳可能なファイルと翻訳不可のファイルが混在しているかどうかを示します。

>[!NOTE]
>
>一度に複数のファイルをアップロードすることは、エラーの影響を大きくする可能性があるので、お勧めしません。

#### [!UICONTROL 参照ファイルを追加する]

このモジュールは、参照ファイルを追加します。

### プロジェクト

#### [!UICONTROL プロジェクトの作成]

このモジュールは、指定されたプロジェクトを作成します。

#### プロジェクトのキャンセルまたは完了

このモジュールは、指定されたプロジェクトをキャンセルまたは完了します。 プロジェクトがダウンロード待ちの場合、プロジェクトはワークフローの最終ステップを経て遷移し、最終的に完了に移ります。 プロジェクトが承認待ちの場合、または仕入先の選択がキャンセルされた場合。 プロジェクトが他のステータスの場合、リクエストは失敗します。

#### [!UICONTROL プロジェクト Zip をダウンロード]

このモジュールは、 `zip` 指定したプロジェクトの翻訳済みファイルのファイル。

#### [!UICONTROL プロジェクトを読む]

このモジュールは、指定されたプロジェクトを取得します。

#### [!UICONTROL ステータスでのプロジェクトの取得]

このモジュールは、指定された状態のすべての使用可能なプロジェクトを取得します。 このメソッドを使用すると、 `$top`, `$skip`、および `$orderby` クエリパラメーター。

#### [!UICONTROL プロジェクトリストを取得]

すべてのプロジェクトの単純なリストを取得し、各プロジェクトに関する一般情報を提供します。 このメソッドを使用すると、 `$top`, `$skip`、および `$orderby` クエリパラメーター。

#### [!UICONTROL プロジェクト作成オプションを検索]

このモジュールは、プロジェクト作成オプションを取得します。

### その他

#### [!UICONTROL API 呼び出しを実行する]

このモジュールは、許可された任意の API 呼び出しを実行します。
