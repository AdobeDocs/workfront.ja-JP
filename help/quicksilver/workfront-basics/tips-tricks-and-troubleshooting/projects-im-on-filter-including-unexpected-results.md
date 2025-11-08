---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 予期しない結果を含む、自分が参加しているプロジェクトフィルター
description: この記事を読んで、予期しない結果を含む、自分が参加しているプロジェクトフィルターのトラブルシューティングを行ってください。
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 90%

---

# 予期しない結果を含む、自分が参加しているプロジェクトフィルター

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table>
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
   <td> <p>PrimeまたはUltimate</p>
    <p>ワークフロー Ultimate</p>
   </td>
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

[!UICONTROL **自分が参加しているプロジェクト**]&#x200B;フィルターには、「[!UICONTROL **入力者**]」または「[!UICONTROL **スポンサー ID**]」など、見逃しやすいフィールドや自動入力されるフィールドなど、「[!UICONTROL **プロジェクトの詳細**]」フィールドのいずれかにユーザーが含まれるプロジェクトが含まれます。不要な結果を削除するには、次の 2 つの解決策が考えられます。

1. フィルターに含まれる予期しない各プロジェクトの、[!UICONTROL **プロジェクトの詳細**]&#x200B;を確認し、すべてのフィールドから自分の名前を削除してください。

   または

1. [!UICONTROL **所有プロジェクト**]&#x200B;など、自分に特別に割り当てられたプロジェクトのみを含む類似のフィルターを使用してみてください。

[!DNL Workfront] でのフィルターの使用について詳しくは、[フィルターの概要](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)を参照してください。
