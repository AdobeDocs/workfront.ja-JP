---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 基本シナリオへの Webhook の追加
description: Webhook は、インスタントトリガーとも呼ばれ、特定のスケジュールではなく、変更が行われるたびにトリガーを開始できる特定の種類のシナリオモジュールです。
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# の基本的なシナリオへの Webhook の追加 [!DNL Adobe Workfront Fusion]

Webhook は、インスタントトリガーとも呼ばれ、特定のスケジュールではなく、変更が行われるたびにトリガーを開始できる特定の種類のシナリオモジュールです。

この例では、特定のキューにリクエストが送信されたらすぐにシナリオを開始する Webhook を追加します。 次に、シナリオはこれらのリクエストをプロジェクトに変換します。

次の使用例は、で作成したシナリオを変更します [基本的なシナリオの作成](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 前提条件

に記載されているシナリオを作成する必要があります。 [基本的なシナリオの作成](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) この手順を実行する前に、

## Webhook の追加と設定

1. Convert object モジュールを開きます。
1. 「イシュー ID」フィールドで、黒の ID ブロックを削除します。 ブロックは、マッピング元のモジュールが使用できなくなったため、黒になります。
1. 最初のモジュール（イベントを監視）の下にある ID ブロックを選択して、2 番目のモジュールにマッピングします。
1. 「**OK**」をクリックします。

### Webhook モジュールの追加

1. シナリオエディターでシナリオを開きます。
1. 最初のモジュールを右クリックし、 **モジュールを削除**.

   モジュールが削除され、空白のプレースホルダーが残ります。

1. 空白のモジュールをクリックし、を選択します。 **Adobe Workfront** アプリのリストから。
1. を選択 **イベントを見る**.
1. クリック **追加** Webhook フィールドの隣です。
1. 「レコードタイプ」フィールドで、 **問題**&#x200B;そのため、モジュールでは問題の変更をトリガーします。
1. 「状態」フィールドで次を選択します **新しい状態**. これは、フィルターに使用される必須フィールドですが、この例では扱いません。
1. 「レコードの生成元」フィールドで、 **新しいレコードのみ**. これにより、イシューが更新や削除されたときではなく、イシューが追加されたときにシナリオがトリガーするようになります。
1. クリック **保存** モジュール設定を保存します。


