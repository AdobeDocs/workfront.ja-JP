---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Qualtrics モジュール
description: ' [!DNL Adobe Workfront Fusion] シナリオでは、Qualtrics を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '313'
ht-degree: 100%

---

# Qualtrics モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Qualtrics] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプやアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## 前提条件

[!DNL Qualtrics] モジュールを使用するには、[!UICONTROL Qualtrics] アカウントが必要です。

## [!DNL Qualtrics] と [!DNL Workfront Fusion] の接続

[!DNL Qualtrics] アカウントへの接続を、[!UICONTROL Qualtrics] モジュール内から直接作成できます。

1. 任意の [!UICONTROL Qualtrics] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>新しい接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data Center ID] </td> 
      <td><code>&lt;Data Center ID>.qualtrics.com</code> の形式を使用します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>API キーを見つけるには、[!DNL Qualtrics] ドキュメントを参照してください。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。

## [!DNL Qualtrics] モジュールとそのフィールド

[!DNL Qualtrics] コネクターでは、以下のモジュールを使用できます。

* [!UICONTROL 新しい調査の回答を見る]
* [!UICONTROL ディレクトリ連絡先の作成]
* [!UICONTROL ディレクトリ連絡先の削除]
* [!UICONTROL ディレクトリ連絡先の取得]
* [!UICONTROL ディレクトリ連絡先の更新]
* [!UICONTROL SMS を使用した新しい調査配布の作成]
* [!UICONTROL メールでの調査配布]
* [!UICONTROL API 呼び出し]
* [!UICONTROL ディレクトリ連絡先をリスト]
