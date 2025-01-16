---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 基本シナリオへのフィルターの追加
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 4%

---

# [!DNL Adobe Workfront Fusion] の基本シナリオへのフィルターの追加

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ 基本シナリオへのフィルターの追加 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-filter-basic-scenario.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

フィルターを使用すると、特定の条件が満たされた場合にのみシナリオを進行させることができます。

この例では、リクエストが特定のリクエストキューに送信された場合にのみリクエストから新しいプロジェクトを作成できるようにするフィルターをシナリオに追加します。

この例では、[ 基本シナリオの作成 ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) で作成したシナリオを変更します。

>[!NOTE]
>
>Workfront トリガーモジュールには、特定の条件が満たされた場合にのみシナリオを開始できるフィルターが含まれます。 ただし、between-module フィルターはモジュール以外およびWorkfront以外のすべてのユースケースで使用されるので、トリガー間でフィルターを使用する方法を学ぶことが重要です。 この例では、モジュール内フィルターで満たされる可能性のある機能に対して、モジュール間フィルターを使用しています。

## 前提条件

この手順を実行する前に、[ 基本シナリオの作成 ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) で説明されているシナリオを作成する必要があります。

## フィルターの追加

### フィルターの追加準備

1. 最初のシナリオを開きます。
1. **出力** 領域で、「`Project`」を選択します。
これで、`ID`、`Name`、`Project` が選択されました。
1. 「OK」をクリックして、モジュール設定を保存します。
1. Workfrontを開きます。
1. Workfrontで、Fusion シナリオが使用するリクエストキューを表すプロジェクトを見つけます。

   このプロジェクトは、Fusion 接続が設定されているのと同じWorkfront アカウントにある必要があります。

1. URL 内のプロジェクト ID をメモします。

   例：https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### フィルターの追加と設定

1. シナリオエディターでシナリオを開きます。
1. 1 つ目のモジュールと 2 つ目のモジュールの間にあるレンチアイコン ![ レンチアイコン ](assets/wrench-icon.png) をクリックし、「**フィルターを設定** を選択します。
1. 「ラベル」フィールドに、「リクエストキューのフィルター」などのこのフィルターのラベルを入力します。
1. **条件** 領域の上部フィールドで、最初のモジュールから `projectID` をマッピングします。

   ![ プロジェクト ID をマップ ](assets/map-proj-id.png)
1. **条件** 演算子は「次と等しい」のままにします。
1. 「**条件**」領域の下部フィールドに、「[ フィルターを追加する準備 ](#prepare-to-add-the-filter)」のプロジェクト URL からメモしたプロジェクト ID を貼り付けます。
1. **OK** をクリックして、フィルター設定を保存します。

### テストしてアクティブ化

1. Fusion が接続しているWorkfront環境に移動し、フィルターで指定したプロジェクトにイシューを追加します。 別の問題を別のプロジェクトに追加します。
1. シナリオエディターの左下隅にある「**[!UICONTROL 1 回実行]**」をクリックします。
1. 出力を調べて、シナリオが期待どおりに実行されたことを確認します。

   両方のイシューが最初のシナリオの出力に表示されますが、2 番目のシナリオへの入力として表示されるのは、指定されたプロジェクトのイシューのみです。
1. シナリオが期待どおりに動作していることを確認したら、画面の左下にある **スケジュール** トグルをクリックして **オン** にします。

   これにより、シナリオがアクティブになります。
1. [!DNL Workfront Fusion] では、左下隅付近の **[!UICONTROL 保存]** をクリックして、シナリオの進捗を保存します。

   >[!IMPORTANT]
   >
   >シナリオを改良、テストするたびに保存するようにしてください。

## リソース

* フィルターについて詳しくは、[ シナリオへのフィルターの追加 ](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md) を参照してください。
