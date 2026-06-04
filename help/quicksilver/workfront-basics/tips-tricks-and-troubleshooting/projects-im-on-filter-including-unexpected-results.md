---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 予期しない結果を含む、自分が参加しているプロジェクトフィルター
description: この記事を読んで、予期しない結果を含む、自分が参加しているプロジェクトフィルターのトラブルシューティングを行ってください。
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 100%

---

# 予期しない結果を含む、自分が参加しているプロジェクトフィルター

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table>
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
   <td>任意</td>
  </tr>
  <tr>
   <td>Adobe Workfront ライセンス
   </td>
   <td><p>標準</p>
   <p>プラン</p>
   </td>
  </tr>
   <tr>
   <td>アクセスレベル設定
   </td>
   <td>[!DNL Workfront] 管理者である必要があります。
   </td>
  </tr>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 問題

[!UICONTROL **自分が参加しているプロジェクト**]&#x200B;フィルターには、これらのプロジェクトに割り当てられていない、または関連付けられていないので、予期しない結果が含まれています。

## ソリューション

[!UICONTROL **自分が参加しているプロジェクト**]&#x200B;フィルターには、「[!UICONTROL **入力者**]」または「[!UICONTROL **スポンサー ID**]」など、見逃しやすいフィールドや自動入力されるフィールドなど、「[!UICONTROL **プロジェクトの詳細**]」フィールドのいずれかにユーザーが含まれるプロジェクトが含まれます。 不要な結果を削除するには、次の 2 つの解決策が考えられます。

1. フィルターに含まれる予期しない各プロジェクトの、[!UICONTROL **プロジェクトの詳細**]&#x200B;を確認し、すべてのフィールドから自分の名前を削除してください。

   または

1. [!UICONTROL **所有プロジェクト**]&#x200B;など、自分に特別に割り当てられたプロジェクトのみを含む類似のフィルターを使用してみてください。

[!DNL Workfront] でのフィルターの使用について詳しくは、[フィルターの概要](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)を参照してください。
