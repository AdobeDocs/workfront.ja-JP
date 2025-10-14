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
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 14%

---

# 環境間でのオブジェクトの比較

環境間でオブジェクトを比較して、環境プロモーションパッケージに必要なオブジェクトが含まれていることを確認できます。

比較する環境とオブジェクトのタイプを選択します。 Workfrontは、両方の環境で選択されたタイプのすべてのオブジェクトを比較し、オブジェクトの違いに関するデータを表示します。

## アクセス要件

以下が必要です。

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] プラン</strong>
   </td>
   <td> PrimeまたはUltimate（新規プランのみ）
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

環境間でオブジェクトを比較するには、組織がAdobeビジネスプラットフォーム上にある必要があります。

## オブジェクト比較の生成

1. オブジェクトを比較する環境に移動します。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 左側のナビゲーションで「**システム**」を選択し、「**環境のプロモーション**」を選択します。
1. 画面の右上隅付近にある **環境を比較** をクリックします。
1. 「**Source環境**」フィールドで、パッケージを作成する環境を選択します。 これは、オブジェクトをコピーする **コピー元の環境** す。
1. 「**ターゲット環境**」フィールドで、パッケージをインストールする環境を選択します。 これは、オブジェクトのコピー先 **環境** です。
1. **比較するオブジェクト** 領域で、環境間で比較するオブジェクト タイプを選択します。
1. 画面の右上隅付近にある「**比較を生成**」をクリックします。

   比較するオブジェクトの数とサイズによっては、比較の生成に時間がかかる場合があります。

## オブジェクトの比較を表示

比較の生成が完了すると、比較が表示されます。

このリストには、ソース環境に存在する選択したタイプのオブジェクト、それらのオブジェクトがターゲット環境に存在しないかどうか、および 2 つのオブジェクト間にフィールドの違いがあるかどうかが表示されます。

>[!BEGINSHADEBOX]

![&#x200B; 比較の例 &#x200B;](assets/environment-promotion-comparison.png)

この例では、次のようになります。

* 最初の行には、ターゲット環境には存在するがソース環境とは異なるオブジェクトが表示されます。
* 2 行目には、ターゲット環境に存在し、ソース環境と同じオブジェクトが表示されます。
* 3 行目には、ターゲット環境に存在しないオブジェクトが表示されます。

>[!ENDSHADEBOX]

特定のオブジェクトの違いを表示するには：

1. そのオブジェクトの行にある虫眼鏡アイコン ![&#x200B; 比較アイコン &#x200B;](assets/compare-icon.png) をクリックします。

   そのオブジェクトのすべてのフィールドを含むウィンドウが開きます。 違いは赤でマークされています。

## オブジェクト比較からのパッケージの作成

オブジェクト比較から直接パッケージを作成できます。

手順については、「環境プロモーションパッケージの作成または編集」の [&#x200B; オブジェクト比較からパッケージを作成する &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison) を参照してください。
