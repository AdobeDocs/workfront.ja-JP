---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境プロモーションパッケージのロールバック
description: 環境プロモーション機能は、構成関連オブジェクトを環境から別の環境に移動する機能を提供することを目的としています。 インストール済みのプロモーションパッケージをターゲット環境からロールバックする方法について説明します。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
TQID: https://experienceleague.adobe.com/EPjuu-mWZH31cMvN-4tdzD8X-YFoW-DJ6YhfnJ0u06k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 389
ht-degree: 19%

---

# 環境プロモーションパッケージのロールバック



パッケージをインストールしたら、ロールバックできます。 これにより、パッケージがターゲット環境で行った変更が削除され、影響を受けるオブジェクトが以前の設定に戻されます。

プロモーションパッケージは、インストール後24時間以内にロールバックできます。 24時間後、そのインストールでロールバック機能は使用できなくなります。

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

* 環境プロモーションパッケージは、ロールバックする前にインストールする必要があります。

  手順については、[環境プロモーションパッケージのインストール ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)を参照してください。


## 特定のパッケージのデプロイメントをロールバックできるかどうかを確認します

特定のパッケージのデプロイメントをロールバックできるかどうかを確認するには、次の点を考慮してください。

* パッケージがインストールされてから24時間未満が経過している必要があります。
* ロールバックできるのは、最新のパッケージデプロイメントのみです。
* 失敗したデプロイメントはロールバックできます。
* ロールバックはロールバックできません。


## インストール済みの環境プロモーションパッケージのロールバック

1. パッケージがインストールされた環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 左側のナビゲーションで「**環境プロモーション**」を選択します。
1. ロールバックするパッケージを選択し、**デプロイメント**&#x200B;をクリックします。
1. ロールバックするデプロイメント（インストール）にカーソルを合わせ、デプロイメントの行の右側に表示されたら、「ロールバック」をクリックします。

   または

   ロールバックするデプロイメントをクリックし、画面の右上隅にある「**パッケージをロールバック**」をクリックします。

   >[!IMPORTANT]
   >
   >デプロイメントは、ロールバックする前に24時間未満で実行されている必要があります。 24時間以上経過したインストールはロールバックできません。

1. （オプション）ロールバックプレビュー領域で、デプロイメントがロールバックされたときに発生する変更を表示します。
1. 画面の右上隅にある「**ロールバック**」をクリックします。
