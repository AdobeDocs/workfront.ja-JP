---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 予期しない結果を含む、自分が参加しているプロジェクトフィルター
description: この記事を読んで、予期しない結果を含む、自分が参加しているプロジェクトフィルターのトラブルシューティングを行ってください。
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 94%

---

# 予期しない結果を含む、自分が参加しているプロジェクトフィルター

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

[!UICONTROL **自分が参加しているプロジェクト**]&#x200B;フィルターには、これらのプロジェクトに割り当てられていない、または関連付けられていないので、予期しない結果が含まれています。

## ソリューション

[!UICONTROL **自分が参加しているプロジェクト**]&#x200B;フィルターには、「[!UICONTROL **入力者**]」または「[!UICONTROL **スポンサー ID**]」など、見逃しやすいフィールドや自動入力されるフィールドなど、「[!UICONTROL **プロジェクトの詳細**]」フィールドのいずれかにユーザーが含まれるプロジェクトが含まれます。不要な結果を削除するには、次の 2 つの解決策が考えられます。

1. フィルターに含まれる予期しない各プロジェクトの、[!UICONTROL **プロジェクトの詳細**]&#x200B;を確認し、すべてのフィールドから自分の名前を削除してください。

   または

1. [!UICONTROL **所有プロジェクト**]&#x200B;など、自分に特別に割り当てられたプロジェクトのみを含む類似のフィルターを使用してみてください。

でのフィルターの使用について詳しくは、 [!DNL Workfront]を参照してください。 [フィルターの概要](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
