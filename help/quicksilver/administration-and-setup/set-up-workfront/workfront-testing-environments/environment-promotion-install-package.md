---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境のプロモーションパッケージのインストール
description: 環境プロモーション機能の目的は、設定関連オブジェクトを環境間で移動する機能を提供することです。 環境プロモーションパッケージをターゲット環境にインストールする方法を説明します。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 8%

---

# 環境のプロモーションパッケージのインストール

パッケージを作成したら、別の環境にインストールできます。

オブジェクトのコピー先となる環境にパッケージをインストールする必要があります **コピー先**。 例えば、カスタム更新サンドボックス環境でプロジェクトを設定し、実稼動環境に昇格する場合は、パッケージを実稼動環境にインストールする必要があります。

>[!IMPORTANT]
>
>環境の昇格のためにオブジェクトを設定している間にカスタム更新サンドボックスが更新されると、その設定は更新時に失われます。 未処理の環境プロモーションオブジェクトおよびパッケージがすべて正常に昇格されない限り、カスタム更新サンドボックスを更新しないことをお勧めします。

## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] プラン</strong>
   </td>
   <td> Prime または Ultimate （新規プランのみ）
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] ライセンス</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>アクセスレベル設定
   </td>
   <td>[!DNL Workfront] 管理者である必要があります。
   </td>
  </tr>
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

環境プロモーションパッケージは、インストールする前に作成する必要があります。

手順については、[ 環境プロモーションパッケージの作成または編集 ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md) を参照してください。

## インストールのパッケージステータス

実稼動環境にインストールするには、パッケージのステータスがアクティブである必要があります。

パッケージをテスト ステータスに移動し、別のサンドボックスにインストールしてパッケージをテストすることをお勧めします。  このテストが成功し、エラーが発生していない場合は、パッケージをアクティブに移動して、実稼動環境にインストールします。

パッケージのステータスを編集するには：

1. 環境プロモーションパッケージの作成と編集の記事の [ 既存のパッケージの編集またはアセンブリ ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) の説明に従って、パッケージを選択します。
1. **パッケージを編集** をクリックします。
1. **ステータス** をクリックします。
1. ドロップダウンリストから目的のステータスを選択します。

ステータスについて詳しくは、「Workfront環境間でのオブジェクトの移動の概要」の [ 環境のプロモーションステータス ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) を参照してください。

## パッケージのインストール

>[!NOTE]
>
>* パッケージをインストールするには、パッケージをインストールする環境にログインする必要があります。 これは、オブジェクトのコピー先 **環境** です。

1. パッケージをインストールする環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 左側のナビゲーションで「**システム**」を選択し、「**環境のプロモーション**」を選択します。
1. 表示されたリストからパッケージを選択します。
1. 衝突が発生したオブジェクトごとに、衝突を解決する方法を選択します。

   競合を解決するには、オブジェクト タイプの横にあるドロップダウン矢印をクリックし、実行するアクションを選択します。

   詳細については、この記事の [ 衝突 ](#collisions) を参照してください
1. パッケージを新しい環境にデプロイするには、画面の右上にある **デプロイ** をクリックします。

## 衝突

競合とは、インストールのターゲット環境にあるオブジェクトで、ソース環境からインストールされるオブジェクトのいずれかと一致するものです。 コリジョンは、ソース オブジェクトの名前と ID をターゲット環境内のオブジェクトと比較することで検出されます。 衝突は、ソース オブジェクトと以前にインストールされたオブジェクトのレコードを比較することによっても検出されます。

コリジョンが発生した場合、コリジョンの解決方法を選択できます。 衝突はオブジェクト レベルで解決されます。

各オブジェクト タイプの隣にあるドロップダウンをクリックすると、コリジョンを表示できます。 コリジョンはコリジョン カラムに表示されます。

>[!NOTE]
>
>検出されたコリジョンは、インストールでオーバーライドまたは使用するオブジェクトではない可能性があります。 検出された競合の検証を推奨し、インストールターゲットが正しいことを確認します。

競合を解決するには、[ 展開アクション ] 列でアクションを選択するか、既に表示されている既定のアクションを使用します。

* **新しい名前で作成**：ターゲット環境に新しいオブジェクトを作成します。 オブジェクトがターゲット環境に存在する場合は、新しい名前で新しいオブジェクトを作成できます。 ターゲット環境にオブジェクトが存在しない場合は、新しい名前、またはオブジェクトのパッケージ内にある名前でオブジェクトを作成できます。
* **既存のを使用**: パッケージ内のオブジェクトはインストールされておらず、ターゲット環境に既に存在するオブジェクトは変更されません。
* **上書き**: パッケージ内のオブジェクトは、ターゲット環境の既存のオブジェクトを置き換えます。

  衝突が検出されない場合でも、上書きするオブジェクトを選択することもできます。

  上書きが親オブジェクトと子オブジェクトにどのように影響するかについて詳しくは、この記事の [ 親オブジェクトと子オブジェクトの上書き ](#overwriting-parent-and-child-objects) を参照してください。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

デフォルト値は、オブジェクトがターゲット環境に存在しない場合は `Create new`、オブジェクトがターゲット環境に存在する場合は `Use existing` です。 「デフォルトのマッピングにリセット **をクリックすると、デフォルトのマッピングに戻すこ** ができます。

## 親オブジェクトと子オブジェクトの上書き

プロモーションパッケージ内の一部のオブジェクトには、子オブジェクトが含まれている場合があります。 例えば、プロジェクト（親）にはタスク（子）があります。 親オブジェクトを上書きする場合、子オブジェクトは次のように処理されます。

* パッケージとターゲットの両方に存在する子オブジェクトは、パッケージに一致するようにターゲットで更新されます。
* パッケージに存在するがターゲットには存在しない子オブジェクトが作成されます。
* ターゲットに存在するがパッケージには存在しない子オブジェクトは、変更されずに残ります。

この機能は、次の親オブジェクトと子オブジェクトに影響します。

| 親オブジェクト | 子オブジェクト |
|---|---|
| プロジェクト | Task<br>QueueDef （キュー定義） <br>RoutingRule |
| テンプレート | TemplateTask<br>QueueDef （キュー定義） <br>RoutingRule |
| パラメーター（カスタムフォームフィールド） | ParameterOption （カスタムフォームフィールドオプション） |
| CalendarInfo | CalendarSection |
| QueueDef （キュー定義） | QueueTopicGroup<br>QueueTopic |

