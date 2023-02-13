---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: シナリオ，パフォーマンス
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion パフォーマンスガードレール
description: Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] パフォーマンスガードレール

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] にはが必要です [!DNL Adobe Workfront Fusion] に加えてライセンス [!DNL Adobe Workfront license].

作業の自動化には迅速な処理が必要なため、 [!DNL Adobe Workfront Fusion] は、高いパフォーマンスを実現するように設計されています。 長時間実行するシナリオは、作業のペースを遅くする可能性があるので、アドビでは、 [!DNL Workfront Fusion] 実行時間、データサイズ、その他のシナリオパラメーターを制限する、パフォーマンスを保つガードレールを使用します。 [!DNL Workfront Fusion] デザイナーは、これらのガードレールを認識し、デザインの慣行に組み込む必要があります。

## シナリオ

* デフォルトのシナリオ実行タイムアウトは、 **40 分**. 実行がこのタイムアウトに達したら、 [!DNL Workfront Fusion] シナリオに応じて、次のサイクルまたは操作の後に、シナリオの実行を中断します。 これにより、40 分の制限に達した直後にシナリオが強制的に停止します
* シナリオのブループリントの最大サイズは次のとおりです **5 MB**&#x200B;シナリオのサイズは以下にすることをお勧めします。 **3 MB**.

   多数のフィールドを持つデータを作成または更新するアプリモジュールは、非常に大きなブループリントを引き起こす可能性があります。

   * を使用する場合、 [!DNL Workfront] アプリの場合は、作成または更新の使用例に必要なフィールドのみを選択してください。
   * 他のアプリを使用する場合は、カスタム API モジュールを使用して、多数のフィールドを持つ任意のレコードタイプを操作します。

* シナリオ内のモジュール数に上限はありませんが、150 を超えるモジュールを持つシナリオは、のパフォーマンスに悪影響を与えます [!DNL Workfront Fusion] システム。 このため、150 を超えるモジュールを使用したシナリオを作成することはお勧めしません。

## 操作

* 通常、デフォルトの操作タイムアウトは **40 秒**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## ファイル

* Fusion のファイルの総処理容量は次のとおりです。 **1 GB**. この制限は、合計メモリコストに基づいています。 すべての運営がそのコストに寄与します。 400 MB の 1 つのファイルをダウンロードしてアップロードした場合、ファイル容量の合計コストは 800 MB になります。

## サーバーのメモリ使用量

* 1 回の実行でのサーバーのメモリ使用量は次の値に制限されます。 **1 GB**.

   大きなファイルや複雑なモジュールなど、多くの要因は、予測や制御が困難な方法でサーバーのメモリ使用量に影響を与える可能性があります。 このため、シナリオが他のすべてのパフォーマンスガードレールに従っている場合でも、シナリオの実行が 1 GB のメモリ制限を超える可能性があります。 メモリ制限を超えると、実行が失敗します。

## ウェブフック

* ペイロードのデフォルトの最大サイズは次のとおりです。 **5 MB**.
* ウェブフックは次に制限されています： **1 秒あたり 100 リクエスト**. この制限に達すると、Workfront Fusion は 429 ([!UICONTROL リクエストが多すぎます]) ステータス。
* [!DNL Workfront Fusion] は、30 日間、webhook ペイロードを保存します。 受信後 30 日を超える Webhook ペイロードへのアクセスにより、「[!UICONTROL ストレージからファイルを読み取れませんでした。]&quot;
* 次のいずれかに該当する場合、Webhook は自動的に非アクティブ化されます。

   * Webhook は 5 日以上どのシナリオにも接続されていません
   * Webhook は、非アクティブなシナリオ（30 日以上非アクティブであったシナリオ）でのみ使用されます。

* 非アクティブ化された Web フックは、シナリオに接続されておらず、30 日以上非アクティブ状態にある場合、自動的に削除され、登録解除されます。
