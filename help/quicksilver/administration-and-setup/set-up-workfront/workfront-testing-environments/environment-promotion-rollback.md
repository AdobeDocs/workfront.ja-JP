---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境プロモーションパッケージのロールバック
description: 環境プロモーション機能の目的は、設定関連オブジェクトを環境間で移動する機能を提供することです。 インストールしたプロモーションパッケージをターゲット環境からロールバックする方法を説明します。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 70f7e2a8-bb27-4546-afb7-53e0eec30bf1
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 15%

---

# 環境プロモーションパッケージのロールバック



パッケージをインストールしたら、ロールバックできます。 これにより、ターゲット環境でパッケージに加えられた変更が削除され、影響を受けたオブジェクトが以前の設定に戻ります。

プロモーションパッケージは、インストール後 24 時間以内にロールバックできます。 24 時間後は、そのインストールでロールバック機能は使用できなくなります。

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

* ロールバックする前に、環境プロモーションパッケージをインストールする必要があります。

  手順については、[&#x200B; 環境プロモーションパッケージのインストール &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md) を参照してください。


## 特定のパッケージデプロイメントをロールバックできるかどうかを判断します

特定のパッケージのデプロイメントをロールバックできるかどうかを知るには、次の点を考慮します。

* パッケージのインストールから 24 時間未満が経過している必要があります。
* ロールバックできるのは、最新のパッケージデプロイメントのみです。
* 失敗したデプロイメントはロールバックできます。
* ロールバックはロールバックできません。


## インストールした環境プロモーションパッケージのロールバック

1. パッケージがインストールされた環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 左側のナビゲーションで **環境のプロモーション** を選択します。
1. ロールバックするパッケージを選択して、「**デプロイメント**」をクリックします。
1. ロールバックするデプロイメント（インストール）の上にマウスポインターを置き、そのデプロイメントの行の右側に表示されたら「ロールバック」をクリックします。

   または

   ロールバックするデプロイメントをクリックし、画面の右上隅にある **パッケージをロールバック** をクリックします。

   >[!IMPORTANT]
   >
   >ロールバックする 24 時間以内にデプロイメントが実行されている必要があります。 24 時間以上前のインストールはロールバックできません。

1. （オプション） ロールバックプレビュー領域で、デプロイメントがロールバックされたときに発生する変更を表示します。
1. 画面の右上隅にある「**ロールバック**」をクリックします。
