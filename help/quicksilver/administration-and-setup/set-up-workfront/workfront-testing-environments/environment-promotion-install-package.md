---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境のプロモーションパッケージのインストール
description: 環境プロモーション機能は、構成関連オブジェクトを環境から別の環境に移動する機能を提供することを目的としています。 環境プロモーションパッケージをターゲット環境にインストールする方法を説明します。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
TQID: https://experienceleague.adobe.com/L6JxhFGfj-LHxRCZuVTxcrMlAx2YAH6wN72A2otyps0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 950
ht-degree: 8%

---

# 環境のプロモーションパッケージのインストール

パッケージを作成したら、別の環境にインストールできます。

オブジェクト **から**&#x200B;にコピーする環境にパッケージをインストールする必要があります。 例えば、カスタムリフレッシュサンドボックス環境でプロジェクトを設定し、実稼動環境にプロモートする場合、パッケージを実稼動環境にインストールする必要があります。

>[!IMPORTANT]
>
>* 環境プロモーション用にオブジェクトを設定している間にカスタムリフレッシュサンドボックスが更新されると、その設定はリフレッシュで失われます。 すべての未処理の環境プロモーションオブジェクトとパッケージが正常に昇格されない限り、カスタムリフレッシュサンドボックスを更新しないことをお勧めします。
>* パッケージのインストールの一環としてターゲット環境で作成されたオブジェクトは、**not**&#x200B;が元の環境のオブジェクトと同じIDを持ちます。 これは、オブジェクトの作成時にIDがシステムによって割り当てられるためです。

## アクセス要件

以下が必要です。

<table>
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
   <td> <p>PrimeまたはUltimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Workfront ライセンス </strong>
   </td>
   <td> <p>標準</p>&gt;
   </td>
  </tr>
   <tr>
   <td>アクセスレベル設定
   </td>
   <td><p>Workfront 管理者である必要があります。</p>
   </td>
  </tr>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

環境プロモーションパッケージは、インストールする前に作成する必要があります。

手順については、[環境プロモーションパッケージの作成または編集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)を参照してください。

## インストールのパッケージステータス

実稼動環境にインストールするには、パッケージがACTIVE ステータスである必要があります。

パッケージをテストステータスに移行し、別のサンドボックスにインストールしてパッケージをテストすることをお勧めします。  このテストが成功し、エラーがない場合は、パッケージをACTIVEに移動して実稼動環境にインストールします。

パッケージのステータスを編集するには：

1. 環境プロモーションパッケージの作成と編集の記事の[既存のパッケージの編集または組み立て](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package)で説明されているように、パッケージを選択します。
1. 「**パッケージを編集**」をクリックします。
1. **ステータス**&#x200B;をクリックします。
1. ドロップダウンメニューから目的のステータスを選択します。

ステータスについて詳しくは、「Workfront環境間でのオブジェクトの移動の概要」の「[環境プロモーションステータス ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses)」を参照してください。

## パッケージのインストール

>[!NOTE]
>
>* パッケージをインストールするには、パッケージをインストールする環境にログインする必要があります。 これは、オブジェクト **を**&#x200B;にコピーする環境です。

1. パッケージをインストールする環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 左側のナビゲーションで「**システム**」を選択し、「**環境プロモーション**」を選択します。
1. 表示されたリストからパッケージを選択します。
1. コリジョンを持つ各オブジェクトについて、コリジョンの解決方法を選択します。

   衝突を解決するには、オブジェクトタイプの横にあるドロップダウン矢印をクリックし、実行するアクションを選択します。

   詳しくは、この記事の[衝突](#collisions)を参照してください
1. 新しい環境にパッケージをデプロイするには、画面の右上にある「**デプロイ**」をクリックします。

## 衝突

コリジョンとは、インストールのターゲット環境にあるオブジェクトで、ソース環境からインストールされているオブジェクトの1つに一致するものです。 ソースオブジェクトの名前とIDをターゲット環境のオブジェクトと比較することで、衝突を検出します。 また、ソースオブジェクトと以前にインストールしたオブジェクトのレコードを比較して、衝突を検出することもできます。

衝突が発生した場合は、衝突の解決方法を選択できます。 衝突はオブジェクトレベルで解決されます。

各オブジェクトタイプの横にあるドロップダウンをクリックすると、衝突を表示できます。 コリジョンは、コリジョン列に表示されます。

>[!NOTE]
>
>検出された衝突は、上書きしたり、インストールで使用したりするオブジェクトではない可能性があります。 検出された衝突を検証して、インストールターゲットが正しいことを確認することをお勧めします。

衝突を解決するには、「デプロイメントアクション」列でアクションを選択するか、既に表示されているデフォルトアクションを使用します。

* **新しい名前で作成**: ターゲット環境に新しいオブジェクトを作成します。 オブジェクトがターゲット環境に存在する場合は、新しい名前の新しいオブジェクトを作成できます。 ターゲット環境にオブジェクトが存在しない場合は、新しい名前またはオブジェクトがパッケージに含まれる名前でオブジェクトを作成できます。
* **既存の**&#x200B;を使用：パッケージ内のオブジェクトはインストールされず、ターゲット環境に既に存在するオブジェクトは変更されません。
* **上書き**: パッケージ内のオブジェクトが、ターゲット環境の既存のオブジェクトに置き換わります。

  また、衝突が検出されない場合でも、上書きするオブジェクトを選択することもできます。

  上書きが親オブジェクトと子オブジェクトにどのような影響を与えるかについて詳しくは、この記事の[親オブジェクトと子オブジェクトの上書き](#overwriting-parent-and-child-objects)を参照してください。
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

オブジェクトがターゲット環境に存在しない場合は`Create new`、オブジェクトがターゲット環境に存在する場合は`Use existing`がデフォルト値です。 「**デフォルトのマッピングにリセット**」をクリックすると、デフォルトのマッピングに戻すことができます。

## 親オブジェクトと子オブジェクトの上書き

プロモーションパッケージ内の一部のオブジェクトには、子オブジェクトが含まれている場合があります。 例えば、プロジェクト（親）にタスク（子）があるとします。 親オブジェクトを上書きする場合、子オブジェクトは次のように処理されます。

* パッケージとターゲットの両方に存在する子オブジェクトは、パッケージに一致するようにターゲットで更新されます。
* パッケージに存在するが、ターゲットには存在しない子オブジェクトが作成されます。
* ターゲットに存在するがパッケージには存在しない子オブジェクトは変更されません。

この機能は、次の親子オブジェクトに影響します。

| 親オブジェクト | 子オブジェクト |
|---|---|
| プロジェクト | タスク <br>QueueDef （キュー定義） <br>RoutingRule |
| テンプレート | TemplateTask<br>QueueDef （キュー定義） <br>RoutingRule |
| パラメーター（カスタムフォームフィールド） | ParameterOption （カスタムフォームフィールドオプション） |
| CalendarInfo | CalendarSection |
| QueueDef （キュー定義） | QueueTopicGroup<br>QueueTopic |

