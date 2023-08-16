---
product-area: reporting
navigation-topic: other-blocks
title: レポートキャンバスでの Web コンテンツブロックの追加または編集
description: Web コンテンツブロックを使用すると、外部の Web サイトからの情報をレポート内に直接表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# レポートキャンバスでの Web コンテンツブロックの追加または編集

Web コンテンツブロックを使用すると、外部の Web サイトからの情報をレポート内に直接表示できます。

## 前提条件

開始する前に、レポートキャンバスベータ版に登録する必要があります。 詳しくは、 [レポートキャンバスベータ版：概要](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Web コンテンツブロックの追加または編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、**レポート**.
1. クリック **新しいレポート**.

   または

   既存のレポートに移動し、 **その他** アイコン ![](assets/more-icon-27x15.png) レポートのヘッダーで、 **編集**.

1. 画面の右側の、の下 **ブロックを追加**、次のいずれか：

   次の項目をドラッグ： **Web コンテンツ** アイコンをキャンバス上の目的の場所に直接配置します。

   または

   次をダブルクリックします。 **Web コンテンツ** アイコンをクリックして、キャンバスの上部にブロックを追加します。

   >[!TIP]
   >
   >ブロックを配置した後に、そのコーナーハンドルをドラッグして、ブロックのサイズを変更できます。

1. クリック **名称未設定の Web コンテンツ** ブロックヘッダーに、ブロックのタイトルを入力します。
1. 次をクリック： **編集** アイコン ![](assets/edit-icon.png) 」と入力します。

   ![](assets/web-content-block-header-350x76.png)

1. Adobe Analytics の **設定** 開いたパネルで、表示するページの完全な URL(「https://」を含む ) を **URL** フィールドに入力します。

   >[!NOTE]
   >
   >現在、表示できるのは、選択したドメインのサイトのみです。 現在使用可能なドメインは次のとおりです。
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   埋め込めない場合は、入力した URL の下に警告が表示されます。 次のような警告があります。

   | 警告名 | 理由 |
   |---|---|
   | 無効な URL | 入力された URL は有効なサイトを返しません。 |
   | プロバイダーサイトの制限 | 埋め込もうとしているサイトは許可されていません。 |

   {style="table-layout:auto"}

1. （オプション） **パスパラメーター** 切り替えて、使用可能なパスパラメータのリストを開きます。

   >[!WARNING]
   >
   >パスパラメーターは現在無効です。

1. クリック **埋め込み URL** 選択内容を保存し、レポートに戻ります。
