---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 基本シナリオへの Webhook の追加
description: Webhook は、インスタントトリガーとも呼ばれ、特定のスケジュールではなく、変更が行われるたびにトリガーを開始できる特定の種類のシナリオモジュールです。
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] の基本シナリオへの Webhook の追加

Webhook は、インスタントトリガーとも呼ばれ、特定のスケジュールではなく、変更が行われるたびにトリガーを開始できる特定の種類のシナリオモジュールです。

この例では、特定のキューにリクエストが送信されたらすぐにシナリオを開始する Webhook を追加します。 次に、シナリオはこれらのリクエストをプロジェクトに変換します。

この例では、[ 基本シナリオの作成 ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) で作成したシナリオを変更します。

## 前提条件

この手順を実行する前に、[ 基本シナリオの作成 ](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) で説明されているシナリオを作成する必要があります。

## Webhook の追加と設定

1. Convert object モジュールを開きます。
1. 「イシュー ID」フィールドで、黒の ID ブロックを削除します。 ブロックは、マッピング元のモジュールが使用できなくなったため、黒になります。
1. 最初のモジュール（イベントを監視）の下にある ID ブロックを選択して、2 番目のモジュールにマッピングします。
1. 「**OK**」をクリックします。

### Webhook モジュールの追加

1. シナリオエディターでシナリオを開きます。
1. 最初のモジュールを右クリックし、「**モジュールを削除**」を選択します。

   モジュールが削除され、空白のプレースホルダーが残ります。

1. 空のモジュールをクリックし、アプリのリストから **0}Adobe Workfront} を選択します。**
1. **イベントをウォッチ** を選択します。
1. Webhook フィールドの横にある「**追加**」をクリックします。
1. 「レコードタイプ」フィールドで「**イシュー**」を選択すると、イシューの変更がトリガーされるようになります。
1. 「状態」フィールドで「**新しい状態**」を選択します。 これは、フィルターに使用される必須フィールドですが、この例では扱いません。
1. 「レコード生成元」フィールドで、「**新しいレコードのみ**」を選択します。 これにより、イシューが更新や削除されたときではなく、イシューが追加されたときにシナリオがトリガーするようになります。
1. 「**保存**」をクリックして、モジュール設定を保存します。
