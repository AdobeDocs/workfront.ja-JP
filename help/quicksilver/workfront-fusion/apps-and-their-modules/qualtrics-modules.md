---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Qualtrics モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Qualtrics を使用するワークフローを自動化でき、さらにそれを複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Qualtrics モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Qualtrics]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Qualtrics] モジュールの場合、 [!UICONTROL Qualtrics] アカウント

## 接続中 [!DNL Qualtrics] から [!DNL Workfront Fusion]

次に、 [!DNL Qualtrics] 内部から直接アカウントを取得する [!UICONTROL Qualtrics] モジュール。

1. 任意の [!UICONTROL Qualtrics] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 接続名 ]</p> </td> 
      <td> <p>新しい接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL データセンター ID] </td> 
      <td>形式を使用 <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API キー ]</td> 
      <td>API キーを見つけるには、 [!DNL Qualtrics] ドキュメント。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Qualtrics] モジュールとそのフィールド

では、以下のモジュールを使用できます。 [!DNL Qualtrics] コネクタ：

* [!UICONTROL 新しい調査の回答を見る]
* [!UICONTROL ディレクトリ連絡先の作成]
* [!UICONTROL ディレクトリ連絡先の削除]
* [!UICONTROL ディレクトリ連絡先の取得]
* [!UICONTROL ディレクトリ連絡先の更新]
* [!UICONTROL SMS を使用した新しい調査配布の作成]
* [!UICONTROL 電子メールでの調査の配布]
* [!UICONTROL API 呼び出しを実行する]
* [!UICONTROL ディレクトリ連絡先のリスト]
