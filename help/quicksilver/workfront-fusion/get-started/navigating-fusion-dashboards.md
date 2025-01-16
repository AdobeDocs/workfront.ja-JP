---
product-area: workfront-navigation
product-previous: workfront-fusion
navigation-topic: workfront-fusion-2-0
title: Workfront Fusion でのダッシュボードの操作
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 8%

---

# Workfront Fusion でのダッシュボードの操作

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [Adobe Workfront Fusion に移動 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/navigate-workfront-fusion/navigate-workfront-fusion.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

Workfront Fusion にログインすると、組織のダッシュボードに移動します。 ここから、左側のナビゲーションの領域をクリックして、Fusion の様々な領域に移動できます。

左側のナビゲーションパネルが表示されない場合は、画面の左上隅にあるメインメニューアイコン ![ メインメニュー ](assets/main-menu-icon-left-nav.png) をクリックします。

| アイコン | エリア | 説明 |
|---|---|---|
| ![ 組織の概要アイコン ](assets/org-overview-icon.png) | 組織の概要 | ここでは、Fusion 組織に関する情報を確認できます。 この組織のシナリオで実行された操作の数と、アクティブなシナリオのリストを表示できます。 また、この組織のチーム、ユーザー、環境のリストを表示することもできます。 |
| ![ チームの概要アイコン ](assets/team-overview-icon.png) | チームの概要 | ここでは、このチームのシナリオで実行された操作の数やアクティブなシナリオのリストなど、Fusion チームに関する情報を確認できます。 また、このチームのユーザーを表示および管理したり、このチームの通知オプションを設定したりできます。 チームを表示する際に、このページの上部にあるドロップダウンから別のチームを選択できます。 |
| ![ シナリオアイコン ](assets/scenarios-icon.png) | シナリオ | Fusion のシナリオは、自動ワークフローを表します。 例えば、あるシナリオでは、受信するWorkfront リクエストを監視してプロジェクトにコンバージョンし、別のシナリオでは、画像を生成してドキュメントプロバイダーにアップロードし、Workfrontに承認タスクを追加するといった処理を行います。 Fusion での作業のほとんどは、シナリオの設定と管理です。 「シナリオ」領域では、チームのシナリオのリストを表示および整理し、表示または変更する個々のシナリオを選択できます。 |
| ![ テンプレートアイコン ](assets/fusion-template-icon.png) | テンプレート | テンプレートは、独自のユースケース用に設定できる事前定義済みシナリオです。 ここでは、Workfront Fusion が提供する公開シナリオと、チームが作成したテンプレートを確認できます。 |
| ![ 接続アイコン ](assets/connections-icon.png) | 接続 | 接続には、Fusion が他のアプリケーションとやり取りするためのログイン資格情報と権限が含まれます。 特定のアプリケーション用の特定の資格情報セットと権限セットを持つ接続を作成し、その接続をシナリオで使用します。 その後、シナリオは、これらの資格情報と権限を持つユーザーが使用できるレコードやその他のデータにアクセスし、変更できます。 1 つのアプリケーションに対して複数の接続を作成し、複数のシナリオで接続を使用できます。 「接続」領域では、チームによって設定された接続のリストを表示および管理できます。 |
| ![webhook アイコン ](assets/webhooks-icon.png) | Web フック | Webhook は、アプリケーションの変更を監視し、その変更に基づいてシナリオを開始します。 例えば、特定のWorkfront プロジェクトに問題が送信された際にシナリオを開始するように Webhook を設定できます。 Webhook エリアには、チームで設定された Webhook のリストと、それらが使用されているシナリオが表示されます。 |
| ![ キーアイコン ](assets/keys-icon.png) | キー | 公開鍵と秘密鍵は、データの暗号化と復号化に使用されます。公開鍵は配布でき、公開鍵を持つすべてのユーザーがデータを暗号化できますが、復号化できるのは秘密鍵のみです。同様に、同様に、秘密鍵を持つユーザーは、公開鍵を持つ誰もが復号化できるデータを暗号化できます。キーエリアでは、チームが所有するキーを表示および管理できます。 |
| ![ データストアアイコン ](assets/datastores-icon.png) | データストア | データストアは、シナリオの外部に存在する小さなデータベースです。 データストアを使用すると、シナリオ間またはシナリオの別々の実行間でデータを転送できます。 データストア エリアでは、チームが所有するデータストアを表示および管理できます。 |
| ![ データ構造アイコン ](assets/datastructures-icon.png) | データ構造 | データ構造は、Fusion に転送されるデータの形式を記述し、JSON、XML、CSV などの形式をシリアル化したり解析したりするために一般的に使用されます。 データ構造では、チームが所有するデータ構造を表示および管理できます。 |

>[!NOTE]
>
>「チーム」セクションのすべての領域で、ページ上部付近のチーム名をクリックし、ドロップダウンから新しいチームを選択することで、別のチームの項目を表示できます。
>
>![ チームドロップダウン ](assets/team-dropdown.png)


<!--
If you are an administrator, the following sections are available (Find out if these are visible, and if so, what they mean.)
Native apps | 
Apps | 
Organizations | 
All scenarios | 
All users |
-->




