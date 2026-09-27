---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境間でのオブジェクトの比較
description: 環境間でオブジェクトを比較して、環境プロモーションパッケージに必要なオブジェクトが含まれていることを確認できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 085b0f04-5a9c-49b9-86d7-2363731ee067
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 14%
---
# 環境間でのオブジェクトの比較

環境間でオブジェクトを比較して、環境プロモーションパッケージに必要なオブジェクトが含まれていることを確認できます。

比較する環境とオブジェクトのタイプを選択します。 Workfrontは、両方の環境で選択したタイプのすべてのオブジェクトを比較し、オブジェクトの違いに関するデータを表示します。

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

環境間でオブジェクトを比較するには、Adobe Business Platformを使用している必要があります。

## オブジェクト比較の生成

1. オブジェクトを比較する環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 左側のナビゲーションで「**システム**」を選択し、「**環境プロモーション**」を選択します。
1. 画面の右上隅付近にある「**環境を比較**」をクリックします。
1. **Source environment** フィールドで、パッケージを作成する環境を選択します。 これは、オブジェクト **を**&#x200B;からコピーする環境です。
1. **Target環境** フィールドで、パッケージをインストールする環境を選択します。 これは、オブジェクト **を**&#x200B;にコピーする環境です。
1. **比較するオブジェクト**&#x200B;領域で、環境間で比較するオブジェクトタイプを選択します。
1. 画面の右上隅付近にある「**比較を生成**」をクリックします。

   比較オブジェクトの数とサイズによっては、比較の生成に時間がかかる場合があります。

## オブジェクトの比較を表示

比較の生成が完了すると、比較が表示されます。

リストには、ソース環境に存在する選択したタイプのオブジェクト、それらのオブジェクトがターゲット環境に存在しないかどうか、およびそれらの間にフィールドの違いがあるかどうかが含まれます。

>[!BEGINSHADEBOX]

![比較例](assets/environment-promotion-comparison.png)

この例では、次のようになります。

* 最初の行は、ターゲット環境に存在するオブジェクトを示していますが、ソース環境とは異なります。
* 2行目は、ターゲット環境に存在し、ソース環境と同じオブジェクトを示します。
* 3行目には、ターゲット環境に存在しないオブジェクトが表示されます。

>[!ENDSHADEBOX]

特定のオブジェクトの違いを表示するには：

1. そのオブジェクトの行の虫眼鏡アイコン ![比較アイコン &#x200B;](assets/compare-icon.png)をクリックします。

   ウィンドウが開き、そのオブジェクトのすべてのフィールドが表示されます。 違いは赤で示されます。

## オブジェクトの比較からパッケージを作成する

オブジェクトの比較から直接パッケージを作成できます。

手順については、環境プロモーションパッケージの作成または編集の記事の「[&#x200B; オブジェクト比較からパッケージを作成する](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison)」を参照してください。
