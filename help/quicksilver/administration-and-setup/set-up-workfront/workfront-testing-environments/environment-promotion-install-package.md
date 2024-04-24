---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境プロモーションパッケージのインストール
description: 環境プロモーション機能の目的は、設定関連オブジェクトを環境間で移動する機能を提供することです。 環境プロモーションパッケージをターゲット環境にインストールする方法を説明します。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: bd27f98191637a3efd11c732890be0091feca89c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 6%

---

# 環境プロモーションパッケージのインストール

>[!NOTE]
>
>パッケージをインストールするには、パッケージをインストールする環境にログインする必要があります。 これは、オブジェクトをコピーする環境です **対象：**.

1. パッケージをインストールする環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. を選択 **システム** 左側のナビゲーションで、を選択します。 **環境促進**.
1. 表示されたリストからパッケージを選択します。
1. 衝突が発生したオブジェクトごとに、衝突を解決する方法を選択します。

   競合を解決するには、オブジェクトタイプの横にあるドロップダウン矢印をクリックし、実行するアクションを選択します。

   詳しくは、を参照してください [衝突](#collisions) この記事の
1. 新しい環境にパッケージをデプロイするには、をクリックします。 **デプロイ** 画面の右上に表示されます。

## 衝突

競合は、インストールパッケージの一部であるオブジェクトが、ターゲット環境に既に存在するオブジェクトと同じ名前を持つ場合に発生します。 これが発生すると、コリジョンの解決方法を選択できます。 衝突はオブジェクト レベルで解決されます。

各オブジェクトタイプの横にあるドロップダウンをクリックすると、衝突を表示できます。 コリジョンはコリジョン カラムに表示されます。

競合を解決するには、[ 展開アクション ] 列でアクションを選択するか、既に表示されている既定のアクションを使用します。

* **新しい名前で作成**：ターゲット環境で新しいオブジェクトを作成します。 オブジェクトがターゲット環境に存在する場合は、新しい名前で新しいオブジェクトを作成できます。 ターゲット環境にオブジェクトが存在しない場合は、新しい名前、またはオブジェクトのパッケージ内にある名前でオブジェクトを作成できます。
* **既存のものを使用**：パッケージ内のオブジェクトはインストールされておらず、ターゲット環境に既に存在しているオブジェクトは変更されません。
* **上書き**：パッケージ内のオブジェクトは、ターゲット環境の既存のオブジェクトを置き換えます。

  衝突が検出されない場合でも、上書きするオブジェクトを選択することもできます。

  上書きが親オブジェクトと子オブジェクトに与える影響について詳しくは、を参照してください。 [親オブジェクトと子オブジェクトの上書き](#overwriting-parent-and-child-objects) この記事の内容です。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

デフォルト値： `Create new` オブジェクトがターゲット環境に存在しない場合、および `Use existing` オブジェクトがターゲット環境に存在する場合。 をクリックすると、デフォルトのマッピングに戻すことができます。 **デフォルトのマッピングにリセット**.

## 親オブジェクトと子オブジェクトの上書き

プロモーションパッケージ内の一部のオブジェクトには、子オブジェクトが含まれている場合があります。 例えば、プロジェクト（親）にはタスク（子）があります。 親オブジェクトを上書きする場合、子オブジェクトは次のように処理されます。

* パッケージとターゲットの両方に存在する子オブジェクトは、パッケージに一致するようにターゲットで更新されます。
* パッケージに存在するがターゲットには存在しない子オブジェクトが作成されます。
* ターゲットに存在するがパッケージには存在しない子オブジェクトは、変更されずに残ります。

この機能は、次の親オブジェクトと子オブジェクトに影響します。

| 親オブジェクト | 子オブジェクト |
|---|---|
| プロジェクト | タスク<br>QueueDef （キュー定義）<br>RoutingRule |
| テンプレート | TemplateTask<br>QueueDef （キュー定義）<br>RoutingRule |
| パラメーター（カスタムフォームフィールド） | ParameterOption （カスタムフォームフィールドオプション） |
| CalendarInfo | CalendarSection |
| QueueDef （キュー定義） | QueueTopicGroup<br>QueueTopic |

