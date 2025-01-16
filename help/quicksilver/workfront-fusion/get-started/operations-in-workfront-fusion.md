---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion の操作
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 80%

---

# [!DNL Adobe Workfront Fusion] での操作



>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ 運営 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/operations-in-workfront-fusion.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

[!DNL Adobe Workfront Fusion] の操作は、モジュールによって実行されるタスクです。トラッキングの目的上、モジュールによって実行された成功アクションは操作とみなします。

## 操作数をカウントする際の考慮事項

* 一般的に、成功したアクションの手順の実行はすべて操作とみなします。

* シナリオの最初のモジュールは 1 回だけ実行され、バンドルを返さない場合でも、常に 1 回の操作としてカウントされます。

* 残りのモジュールが実行される回数は、処理する必要のあるバンドルの数によって異なります。1 つのバンドルに対するモジュールの 1 回の実行は、1 回の操作です。例外はアグリゲータモジュールで、処理されるバンドルのセットごとに 1 回の操作としてカウントされます。

* 操作は、シナリオ実行の[!UICONTROL 最終化]ステージでカウントされます。

* 次は、操作としてカウント&#x200B;**されません**。

   * 任意のフィルター手順。

   * エラーまたは停止するアクション。

   * フォールバックや無効なルートなどの、ルートのルールが満たされなかったために実行されないルート。

   * フィルターがデータを許可していないか、エラーが原因でシナリオが停止したために、実行されないアクション。

## 操作の制限

組織には月間の操作制限が設定されている場合があります。これは、組織が購入した [!DNL Workfront] プランに基づいています。[!UICONTROL Ultimate] [!DNL Workfront] プランは無制限の操作を提供します。

組織が月間の制限を設けている場合は、制限に近づくと通知が届きます。制限を越えた場合、[!DNL Workfront] は組織に連絡して、プランがニーズを満たしていることを確認します。

## 過去 30 日間に実行された操作数を表示

実行された操作の数を示すグラフが表示されます。これらのグラフは、次の場所で利用できます。

* **組織ダッシュボード**：組織全体で使用される操作
* **チームダッシュボード**：このチームが所有するシナリオで使用される操作（[!DNL Adobe Experience Cloud] のみ）
* **シナリオの詳細ページ**：このシナリオで使用される操作（[!DNL Adobe Experience Cloud] のみ）
