---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion リリースアクティビティ：2020 年 11 月 16 日の週'
description: このページでは、2020 年 11 月 17 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ：2020 年 11 月 16 日の週

このページでは、2020 年 11 月 17 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

## Jira Cloud Connector の更新

Jira Cloud コネクタの使用方法を拡張するために、3 つの新しいモジュールが追加されました。

* スプリントに問題を追加
* レコードのリスト
* レコードの検索

また、「Sprint」オブジェクトタイプをサポートするために、既存のモジュールも更新しました。 以前は、「Sprint」オブジェクトには、カスタム API 呼び出しモジュールからのみアクセスできました。

詳しくは、 [Jira Software モジュール](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## シナリオでのマッピングに実行 ID を使用できるようになりました

シナリオの実行 ID がマッピングパネルで使用できるようになりました。 この ID は、シナリオの特定の実行を表し、メタデータとして使用できます。 たとえば、実行 ID は、Fusion が作成するレコードと共に保存できるので、後でどの Fusion の実行がレコードを作成したかを判断できます。 実行 ID は、「一般関数」の下のマッピングパネルにあります。

シナリオの実行について詳しくは、 [Adobe Workfront Fusion のシナリオの実行、サイクル、フェーズ](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Workfront Fusion 2.0 シナリオのキーボードショートカット

シナリオの作成をより便利にするために、キーボードショートカットを追加しました。

* Ctrl/Cmd+Shift+Enter キー：シナリオを 1 回実行
* Ctrl/Cmd + Shift + S:シナリオの保存

Workfront Fusion 2.0 シナリオの構築について詳しくは、 [Adobe Workfront Fusion でシナリオを作成する](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Office 365 Excel コネクタの更新

Office 365 Excel コネクタの使用方法を拡張するために、新しいモジュールが追加されました。 次の操作が可能になりました。

* トリガーからワークブックへの変更からモジュールへの変更
* ワークブックの検索またはダウンロード
* ワークシート、ワークシート行、表、または表行のリスト
* テーブルまたはワークシート行を更新する
* テーブルまたはワークシート行を削除する
* テーブルのメタデータの取得
* カスタム API 呼び出しをおこなう

以前使用可能だったモジュールは、アプリ内にまだ存在します。

詳しくは、 [Microsoft Office 365 Excel モジュール](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## Workfrontアプリ接続で OAuth 2.0 を使用する

Workfrontコネクタを更新して OAuth 2.0 を使用するようにしました。この更新により、Workfrontアプリの接続を変更しやすくなりました。 例えば、接続に関する何か（パスワードなど）が変更された場合、シナリオで個々の接続を更新する必要がなくなりました。 また、OAuth2 には、セキュリティの向上やシングルサインオン (SSO) の使用など、その他の利点があります。

現時点では、既存の接続に変更を加える必要はありません。 ただし、OAuth 2.0 のメリットを活用する場合は、既存の接続を再認証できます。

詳しくは、 [Adobe Workfrontモジュール](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
