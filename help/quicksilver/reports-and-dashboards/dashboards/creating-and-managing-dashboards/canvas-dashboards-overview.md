---
title: キャンバスダッシュボードの概要
description: レポートキャンバスのビジュアライゼーションと従来のレポートを統合し、新しいレイアウトオプションを備えたキャンバスダッシュボードを作成できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b02ca181-e3c3-41e9-ab45-b1b606909127
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 92%

---

# キャンバスダッシュボードの概要

<!-- This page is hidden as it is outdated, delete once full Canvas Dashboard docs are live-->
<!-- Audited: 12/2023 -->

現在、ダッシュボード向けに開発中の機能であるキャンバスダッシュボードは、Workfront で効果的なダッシュボードを構築するための新しいオプションを提供します。キャンバスダッシュボードを使用すると、レポートキャンバスのビジュアライゼーションを既存のレポートに簡単に含めることができ、柔軟性が向上し、新しいレイアウトオプションが提供されます。

この機能は開発中で、まだ次の機能をサポートしていません。
* 外部ページ
* カレンダー統合
* プロンプトレポート
* レイアウトテンプレートを使用した配布

キャンバスダッシュボードに追加された機能の完全なリストについては、[キャンバスダッシュボード：リリースアクティビティ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md)を参照してください

## キャンバスダッシュボードへのアクセス

既存のダッシュボードのランディングページの左パネルにある新しい「キャンバスダッシュボード」オプションを有効にして、キャンバスダッシュボードにアクセスできます。このメニューオプションは、デフォルトでオフになっており、アクセスを有効にするオンに切り替える必要があります。メニューオプションを有効にし、そのオプションに移動する方法について詳しくは、以下の手順を参照してください。

### ダッシュボードの左パネルにキャンバスダッシュボードを追加

>[!IMPORTANT]
>
>レイアウトテンプレートのキャンバスダッシュボード項目を切り替えるには、少なくともレポートとダッシュボードの表示権限が必要です。

1. [レイアウトテンプレートの作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)の説明に従って、キャンバスダッシュボードを有効にするレイアウトテンプレートの作業を開始します。

1. 「**ユーザーの表示項目のカスタマイ**」ドロップダウンメニューをクリックして、「**ダッシュボード**&#x200B;をクリックします。

1. 下に表示される **左側のパネル** リストで、**キャンバスダッシュボード ![ の横にある ](assets/delete-secondary-nav-item.png) セカンダリナビゲーション項目を削除** アイコンをクリックします。 アイコンが ![ セカンダリナビゲーション項目を追加 ](assets/add-secondary-nav-item.png) に変わり、ダッシュボードの左側のパネルに表示されることを示します。

1. ウィンドウの下部にある「**保存**」をクリックします。

### キャンバスダッシュボードを開く

1. レイアウトテンプレートで「キャンバスダッシュボード」オプションが有効になっていることを確認します。手順については、上記の&#x200B;**ダッシュボードの左パネルにキャンバスダッシュボードを追加**&#x200B;を参照してください。

1. 「メインメニュー」アイコン ![ 「メインメニュー」アイコン ](assets/main-menu-icon.png) をクリックし、「**ダッシュボード**」をクリックします。

1. 左側のパネルで、「**キャンバスダッシュボード**」をクリックします。

## キャンバスダッシュボードの使用

### 新しいキャンバスダッシュボードを作成

1. 上記の&#x200B;**キャンバスダッシュボードを開く**&#x200B;の説明に従って、キャンバスダッシュボードを開きます。

1. 「**+ 新しいダッシュボード**」をクリックします。

1. 左上隅の「**名称未設定**」をクリックして、ダッシュボードの名前を入力します。

1. 右上隅の「**完了**」をクリックして新しいダッシュボードを保存するか、以下の&#x200B;**キャンバスダッシュボードにレポートを追加**&#x200B;の説明に従ってウィジェットの追加を開始します。

### キャンバスダッシュボードにレポートを追加

1. 上記の&#x200B;**キャンバスダッシュボードを開く**&#x200B;の説明に従って、キャンバスダッシュボードを開きます。

1. ダッシュボードのリストから、レポートを追加するダッシュボードをクリックします。

1. 右上隅にある「**ウィジェットを管理**」をクリックし、「**ウィジェットを追加**」をクリックします。

1. 追加するレポートウィジェットのタイプの上にポインタを合わせて、表示されるチェックボックスをクリックします。

1. 追加するすべてのウィジェットを選択したら、右上隅にある「**追加**」をクリックします。

1. 選択したウィジェットがダッシュボードに表示されます。ウィジェットの中央にある「**設定**」をクリックして、表示するレポートを選択します。

1. 「**レポートを検索**」フィールドに、表示するレポートの名前の入力を開始します。リストにレポートが表示されたら、名前の横にある「**リストレポート**」または「**グラフレポート**」アイコンをクリックすると、そのレポートの情報が選択した形式で表示されます。

>[!WARNING]
>
> 現在、同一レポートの情報を表示する複数のウィジェットを追加することができますが、ダッシュボードのパフォーマンスに影響を与える可能性があるので、各レポートは 1 回だけ表示することをお勧めします。

### キャンバスダッシュボードでウィジェットを編集

1. 上記の&#x200B;**キャンバスダッシュボードを開く**&#x200B;の説明に従って、キャンバスダッシュボードを開きます。

1. ダッシュボードのリストから、編集するダッシュボードをクリックします。

1. （オプション）ウィジェットのサイズを変更するには、ウィジェットの左下隅にある「**サイズ変更**」アイコンをドラッグ＆ドロップして、希望のサイズに変更します。

1. （オプション）ウィジェットの位置を変更するには、ウィジェットの境界の空白をクリックし、ダッシュボード上の目的の位置までドラッグします。
