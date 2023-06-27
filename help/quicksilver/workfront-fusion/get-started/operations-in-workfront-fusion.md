---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion の運用
description: Adobe Workfront Fusion の操作は、モジュールによって実行されるタスクです。 追跡のために、モジュールが成功したアクションはすべて操作になります。
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# の操作 [!DNL Adobe Workfront Fusion]

の操作 [!DNL Adobe Workfront Fusion] は、モジュールによって実行されるタスクです。 追跡のために、モジュールが成功したアクションはすべて操作になります。

## 操作数をカウントする際の考慮事項

* 一般に、成功したアクションステップの実行は、操作と見なされます。

* シナリオの最初のモジュールは 1 回だけ実行され、バンドルを返さない場合でも、常に 1 回の操作としてカウントされます。

* 残りのモジュールが実行される回数は、処理する必要のあるバンドルの数によって異なります。  1 つのバンドルに対するモジュールの 1 回の実行は 1 回の操作です。 例外は集約モジュールで、処理されるバンドルのセットごとに 1 回の操作としてカウントされます。

* 操作は [!UICONTROL 確定] シナリオ実行のステージ。

* 以下が該当します。 **not** 操作としてカウント：

   * 任意のフィルター手順。

   * エラーまたは停止するアクション。

   * ルートのルールが満たされなかったために実行されないルート（フォールバックや無効なルートなど）。

   * フィルターがデータを許可していないか、エラーが原因でシナリオが停止したために、実行しないアクション。

## 操作の制限

組織には月次の操作制限が設定されている場合があります。 これは、 [!DNL Workfront] 組織が購入したプランを作成します。 この [!UICONTROL Ultimate] [!DNL Workfront] プランは無制限の操作を提供します。

組織が毎月の制限を設けている場合は、制限に近づくと通知が届きます。 もし限界を越えれば [!DNL Workfront] が組織に連絡して、計画がニーズを満たしていることを確認します。

## 過去 30 日間に実行された操作数を表示

実行された操作の数を示すグラフが表示されます。 これらのグラフは、次の場所で利用できます。

* **組織ダッシュボード**:組織全体で使用される操作
* **チームダッシュボード**:このチームが所有するシナリオで使用される操作 ([!DNL Adobe Experience Cloud] のみ )
* **シナリオの詳細ページ**:このシナリオで使用される操作 ([!DNL Adobe Experience Cloud] のみ )

