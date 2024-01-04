---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 予期しない結果を含む、フィルター処理中のプロジェクト
description: この記事を読んで、予期しない結果を含む I'm On フィルタのトラブルシューティングを行ってください。
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# [ 現在のプロジェクト ] フィルターに予期しない結果が含まれています

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL システム管理者 ]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

The [!UICONTROL **自分がいるプロジェクト**] これらのプロジェクトに割り当てられていない、または関連付けられていないので、フィルターには予期しない結果が含まれます。

## 解決策

The [!UICONTROL **自分がいるプロジェクト**] フィルターには、任意の [!UICONTROL **プロジェクトの詳細**] フィールド（例えば、簡単に見逃すか、自動的に入力されるフィールドを含む） [!UICONTROL **入力者**] または [!UICONTROL **スポンサー ID**]. 不要な結果を削除するには、次の 2 つの解決策が考えられます。

1. 次を確認します。 [!UICONTROL **プロジェクトの詳細**] フィルターに含まれる予期しない各プロジェクトに対して、お客様の名前をすべてのフィールドから削除します。

   または

1. 次のような類似のフィルターを使用してみてください。 [!UICONTROL **自分が所有するプロジェクト**]：ユーザーに特別に割り当てられたプロジェクトのみが含まれます。

でのフィルターの使用について詳しくは、 [!DNL Workfront]を参照してください。 [フィルターの概要](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
