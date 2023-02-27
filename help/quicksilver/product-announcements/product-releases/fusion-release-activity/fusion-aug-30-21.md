---
title: Workfront Fusion リリースアクティビティ：&nbsp;2021 年 8 月 30 日の週
description: Workfront Fusion リリースアクティビティ：&nbsp;2021 年 8 月 30 日の週
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ：2021 年 8 月 30 日の週

このページでは、2021 年 8 月 30 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

## Workfront/イベント監視モジュールをトリガーするイベントのフィルタリング

1. Workfront/イベント監視モジュールをトリガーするイベント用のカスタムフィルターを設定する

   不要なシナリオの実行数を減らすために、 Workfront /レコード監視モジュールを更新し、イベントのフィルタリングを有効にしました。 これで、Webhook を作成する際にフィルターを設定できます。 これにより、イベントが特定の条件を満たす場合にのみ、トリガーが発生します。

   イベントフィルターは、現在、次の操作を提供しています。

   * 次と等しい：トリガー：イベントがフィルターの条件と一致する場合にのみ、シナリオをフィルターします。 例えば、イベントが特定のプロジェクトで発生した場合にのみシナリオをトリガーするフィルターを設定できます。
   * 等しくない：トリガーイベントがフィルターの条件に一致しない場合にのみ、シナリオをイベントします。 例えば、でイベントが発生した場合にステータスが「クローズ」にならない場合にのみ、シナリオをトリガーするフィルターを作成できます。

   以前は、監視レコードモジュールはすべてのレコードを取得していました。 ユーザーは、シナリオの後半でフィルターを設定することでのみ、フィルタリングできました。

   イベントのフィルタリングを活用するには、Watch イベントモジュールで新しい Webhook を作成します。 現在、この機能を含めるために既存の Web フックを編集することはできません。 既存のシナリオに対して、イベントフィルターを使用して新しい Web フックを作成することを強くお勧めします。

1. 現在の接続でトリガーされたイベントを除外します。

   Web フックをWorkfront / Watch イベントモジュール用に簡単に設定できるように、最も一般的なイベントフィルターが追加されました。 これで、Webhook には、Watch イベントモジュール用に指定された接続を使用して、モジュールによる変更を除外するオプションが用意されました。 つまり、このフィルターを有効にすると、その接続に関連付けられたWorkfrontユーザーが行った変更では、シナリオをトリガーできなくなります。

   以前は、このフィルターは使用できませんでした。 したがって、Workfrontモジュールでおこなった変更を、これらのモジュールを含むトリガーシナリオに対して容易に行うことができ、シナリオが無限ループで自らをトリガーさせる可能性があります。

Workfront/イベントを監視モジュールのイベントフィルターについて詳しくは、 [Adobe Workfrontモジュール](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

