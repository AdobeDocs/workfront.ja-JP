---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境プロモーションパッケージのインストール
description: 環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 ターゲット環境に環境プロモーションパッケージをインストールする方法を説明します。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 610469811a937fde70a938af829b156e69cca391
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 9%

---

# 環境プロモーションパッケージのインストール


1. パッケージをインストールする環境に移動します。 これは、オブジェクトをコピーする環境です **から**.
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 選択 **システム** 左側のナビゲーションで、「 **環境の昇格**.
1. 表示されたリストからパッケージを選択します。
1. パッケージをインストールするには、 **インストール** をクリックします。
1. パッケージ内の各オブジェクトを、ターゲット環境内の対応するオブジェクトにマッピングします。

   詳しくは、 [マッピング](#mapping) この記事では、


## マッピング

各オブジェクトタイプは、左側のナビゲーションとカードに表示されます。 カードには、そのタイプのオブジェクトと、それらのオブジェクトがターゲット環境に存在するかどうかが表示されます。 これらのオブジェクトがターゲット環境にどのように移動するかを決定できます。

* 新規作成：ターゲット環境に新しいオブジェクトを作成します。 ターゲット環境にオブジェクトが存在する場合は、新しい名前で新しいオブジェクトを作成できます。 ターゲット環境に存在しない場合は、新しい名前でオブジェクトを作成するか、パッケージに含まれるオブジェクトの名前でオブジェクトを作成できます。
* 既存を使用：パッケージ内のオブジェクトがインストールされておらず、ターゲット環境に既に存在するオブジェクトは変更されていません。
* 既存を上書き： （現在は使用できません）ターゲット環境内の既存のオブジェクトに代わる、パッケージ内のオブジェクト。
* 使用しない：パッケージ内のオブジェクトがターゲット環境にインストールされていません。 [ 使用しない ] を選択すると、この選択が他のオブジェクトやフィールドに与える影響を詳細に示すエラーメッセージが表示されます。

デフォルト値は次のとおりです。 `Create new` オブジェクトがターゲット環境に存在しない場合、また `Use existing` （対象の環境にオブジェクトが存在する場合）。 デフォルトのマッピングに戻すには、 **デフォルトのマッピングにリセット**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
