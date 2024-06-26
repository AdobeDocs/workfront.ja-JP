---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境のプロモーションパッケージの作成または編集
description: 環境プロモーション機能の目的は、設定関連オブジェクトを環境間で移動する機能を提供することです。 環境プロモーションパッケージを作成して、別の環境にインストールする方法を説明します。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 17%

---

# 環境のプロモーションパッケージの作成または編集

オブジェクトをコピーする環境にパッケージを作成する必要があります **から**. 例えば、カスタム更新サンドボックス環境でプロジェクトを設定し、実稼動環境に昇格する場合は、カスタム更新サンドボックス環境でパッケージを作成する必要があります。

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

この表にある情報についての詳細は、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## パッケージを作成

1. パッケージを作成する環境に移動します。 これは、オブジェクトをコピーする環境です **から**.
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. を選択 **システム** 左側のナビゲーションで、を選択します。 **環境促進**.
1. クリック **パッケージを作成**.

   「新規プロモーションパッケージ」 ページが開きます。

1. が含まれる **パッケージ名** フィールドに、パッケージの名前を入力します。
1. が含まれる **説明** このパッケージの説明を入力します。
1. パッケージにオブジェクトを追加するには、以下をクリックします **オブジェクトを追加** 左側のナビゲーションで、追加するオブジェクトのタイプを選択します。
1. リストから 1 つ以上のオブジェクトを選択するか、検索バーに名前を入力して、リストに表示されたらオブジェクトを選択します。 リストで複数のオブジェクトを選択できます。
1. クリック **追加（X オブジェクト）** 選択したオブジェクトをパッケージに追加します。

   >[!INFO]
   >
   >**例**
   >
   >プロジェクトに追加するプロジェクトを 3 つ選択した場合は、とボタンに表示されます **3 つのプロジェクトを追加**.

   追加したオブジェクトは、ページの右側の「パッケージコンテンツ」領域に表示されます。

1. 別のタイプのオブジェクトを追加するには、手順 7 ～ 9 を繰り返します。
1. （オプション）パッケージからオブジェクトを削除するには、「パッケージコンテンツ」領域のオブジェクトにポインタを合わせて、オブジェクトの横にある「X」をクリックします。
1. 必要なオブジェクトをすべてパッケージに追加したら、 **保存して閉じる** パッケージを組み立てずに保存します。

   または

   クリック **保存とアセンブリ** パッケージを保存してアセンブリします。

   >[!NOTE]
   >
   >* パッケージに 5 文字以上の名前と、1 つ以上のオブジェクトが追加されている場合は、「保存して閉じる」ボタンと「保存してアセンブリ」ボタンを使用できます。
   >* テストまたはアクティブなど、インストール可能な状態のパッケージはアセンブリできません。

## 既存のパッケージの編集またはアセンブリ

1. パッケージを作成する環境に移動します。 これは、オブジェクトをコピーする環境です **から**.
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. を選択 **システム** 左側のナビゲーションで、を選択します。 **環境促進**.
1. 表示されたリストからパッケージを選択します。
1. （条件付き）無効なパッケージを表示するには、 **廃止されたパッケージを表示** オプション。
1. （オプション）すべてのオブジェクトとそのサブオブジェクトを含むコンテンツを表示するには、内のオブジェクト タイプの横にあるドロップダウン矢印をクリックします **目次** セクション。
1. （オプション）このパッケージの以前のインストールおよびインストール試行を表示するには、 **デプロイメント**.
1. （オプション）パッケージを編集するには、 **パッケージを編集** 画面の右上に表示されます。
1. パッケージをインストールするには、 **インストール** 画面の右上に表示されます。

   パッケージのインストール手順については、 [環境プロモーションパッケージのインストール](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
