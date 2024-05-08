---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 基本シナリオへのフィルターの追加
description: フィルターを使用すると、特定の条件が満たされた場合にのみシナリオを進行させることができます。
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 5%

---

# の基本的なシナリオへのフィルターの追加 [!DNL Adobe Workfront Fusion]

フィルターを使用すると、特定の条件が満たされた場合にのみシナリオを進行させることができます。

この例では、リクエストが特定のリクエストキューに送信された場合にのみリクエストから新しいプロジェクトを作成できるようにするフィルターをシナリオに追加します。

次の使用例は、で作成したシナリオを変更します [基本的なシナリオの作成](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront トリガーモジュールには、特定の条件が満たされた場合にのみシナリオを開始できるフィルターが含まれます。 ただし、between-module フィルターはモジュール以外およびWorkfront以外のすべてのユースケースで使用されるので、トリガー間でフィルターを使用する方法を学ぶことが重要です。 この例では、モジュール内フィルターで満たされる可能性のある機能に対して、モジュール間フィルターを使用しています。

## 前提条件

に記載されているシナリオを作成する必要があります。 [基本的なシナリオの作成](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) この手順を実行する前に、

## フィルターの追加

### フィルターの追加準備

1. 最初のシナリオを開きます。
1. が含まれる **出力** エリア、選択 `Project`.
これで、次のようになります `ID`, `Name`、および `Project` を選択しました。
1. 「OK」をクリックして、モジュール設定を保存します。
1. Workfrontを開きます。
1. Workfrontで、Fusion シナリオが使用するリクエストキューを表すプロジェクトを見つけます。

   このプロジェクトは、Fusion 接続が設定されているのと同じWorkfront アカウントにある必要があります。

1. URL 内のプロジェクト ID をメモします。

   例：https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### フィルターの追加と設定

1. シナリオエディターでシナリオを開きます。
1. レンチアイコンをクリックします。 ![レンチアイコン](assets/wrench-icon.png) 最初のモジュールと 2 番目のモジュールの間にあるを選択します。 **フィルターの設定**.
1. 「ラベル」フィールドに、「リクエストキューのフィルター」などのこのフィルターのラベルを入力します。
1. が含まれる **条件** 領域の上部フィールドで、 `projectID` 最初のモジュールから。

   ![プロジェクト ID をマッピング](assets/map-proj-id.png)
1. を残す **条件** 次と等しい演算子。
1. の下部のフィールドに **条件** 領域で、メモしたプロジェクト ID を内のプロジェクト URL から貼り付けます。 [フィルターの追加準備](#prepare-to-add-the-filter).
1. クリック **OK** フィルター設定を保存します。

### テストしてアクティブ化

1. Fusion が接続しているWorkfront環境に移動し、フィルターで指定したプロジェクトにイシューを追加します。 別の問題を別のプロジェクトに追加します。
1. シナリオエディターの左下隅にある「**[!UICONTROL 1 回実行]**」をクリックします。
1. 出力を調べて、シナリオが期待どおりに実行されたことを確認します。

   両方のイシューが最初のシナリオの出力に表示されますが、2 番目のシナリオへの入力として表示されるのは、指定されたプロジェクトのイシューのみです。
1. シナリオが期待どおりに動作していることを確認したら、 **スケジュール** 画面の左下にあるを切り替えて **日付：**.

   これにより、シナリオがアクティブになります。
1. 対象： [!DNL Workfront Fusion]を選択し、 **[!UICONTROL 保存]** 左下隅付近にあるシナリオの進捗を保存します。

   >[!IMPORTANT]
   >
   >シナリオを改良、テストするたびに保存するようにしてください。

## リソース

* フィルターについて詳しくは、 [シナリオへのフィルターの追加](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

