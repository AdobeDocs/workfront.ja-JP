---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: プルーフビューアーでプルーフを比較
description: 2 つのプルーフの比較結果を並べて表示できます。これらは、同じプルーフの 2 つのバージョンである場合も、まったく別個の 2 つのプルーフである場合もあります。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: ht
source-wordcount: '976'
ht-degree: 100%

---

# プルーフビューアーでプルーフを比較

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

2 つのプルーフの比較結果を並べて表示できます。これらは、同じプルーフの 2 つのバージョンである場合も、まったく別個の 2 つのプルーフである場合もあります。

## プルーフバージョンを比較 {#compare-proof-versions}

1. 比較する複数のバージョンを持つプルーフを開きます。
1. 表示されるプルーフビューアの左上隅で、プルーフの名前をクリックします。次に、表示されるバージョンリストで、開いて比較するバージョンの横にある&#x200B;**比較**&#x200B;アイコンをクリックします。

   ![](assets/compare-proofs-choose-version-350x115.jpg)

   プルーフは横に並べて表示され、より新しいバージョンが左側に表示されます。

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. [比較ツールの使用](#use-the-compare-tools)に進みます。

## 個別のプルーフの比較 {#compare-separate-proofs}

2 つの別個のプルーフを比較できます。

* [ [!DNL Workfront] 内の別個のプルーフを比較](#compare-separate-proofs-in-workfront)
* [ [!DNL Workfront Proof] 内の別個のプルーフを比較](#compare-separate-proofs-in-workfront-proof)

### [!DNL Workfront] 内の別個のプルーフを比較 {#compare-separate-proofs-in-workfront}

[!DNL Workfront] 内のドキュメントリストに含まれる別個のプルーフを比較する方法については、[プルーフの比較](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md)記事で[2 つの異なるプルーフの比較](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list)の節を参照してください。

### [!DNL Workfront Proof] 内の別個のプルーフを比較 {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>比較するプルーフは、同じフォルダー内に存在するか、フォルダー構造内の同じ階層レベルに存在する必要があります。フォルダーを使用して比較対象のプルーフをグループ化する方法について詳しくは、[プルーフビューアでの複数のプルーフの操作](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)を参照してください。

1. 比較するプルーフのいずれかをプルーフビューアで開きます。
1. **[!UICONTROL 比較モード]**&#x200B;アイコンをクリックします。

   ![proof_compare_icon.png](assets/proof-compare-icon.png)\
   表示エリアが半分に分割され、プルーフビューアの左側と右側の両方にプルーフが表示されます。

   ![Compare_proofs-versions.png](assets/compare-proofs-versions-350x180.png)

1. 左右どちらかのプルーフの上にある[!UICONTROL フォルダー]アイコンをクリックして、同じフォルダー内の他のプルーフを一覧表示します。

   ![Folder_icons_when_comparing_in_proofing_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. 現在プルーフビューアで開いているプルーフと比較するプルーフの名前をリストでクリックします。

   ![Comparing_proofs-list_of_proofs_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   両方のプルーフが表示されます。

1. [比較ツールの使用](#use-the-compare-tools)に進みます。

## 比較ツールの使用 {#use-the-compare-tools}

プルーフビューアには、プルーフを効果的かつ効率的に比較するための様々なツールが用意されています。

* [プルーフの自動比較](#auto-compare-proofs)
* [オーバーレイでのプルーフの比較](#compare-proofs-in-an-overlay)
* [同時ナビゲーション比較](#simultaneous-navigation-comparison)

### プルーフの自動比較 {#auto-compare-proofs}

自動比較では、2 つの静的プルーフまたはビデオプルーフをピクセルごとに比較します。相違点が検出されると、左側のプルーフで赤くハイライト表示されます。

インタラクティブプルーフを比較する場合は、自動比較は使用できません。

2 つのプルーフを自動比較するには、次の手順に従います。

1. 次のいずれかの方法でプルーフの比較を開始します。

   * 同じプルーフの 2 つのバージョンを比較する（この記事の[プルーフバージョンを比較](#compare-proof-versions)を参照）
   * 2 つの別個のプルーフを比較する（この記事の[別個のプルーフの比較](#compare-separate-proofs)を参照）

1. **[!UICONTROL 自動比較]**&#x200B;アイコンをクリックします。

   ![proof_autocompare_icon.png](assets/proof-autocompare-icon-31x32.png)

   2 つのプルーフに相違点があると、左側のプルーフで赤くハイライト表示されます。

1. （オプション）**[!UICONTROL 切り替え]**&#x200B;アイコンをクリックすると、アクティブな側が変わって、右側のプルーフに相違点が表示されるようになります。デフォルトでは、相違点は左側のプルーフに表示されます。

   ![proof_autocompare_changeactive.png](assets/proof-autocompare-changeactive.png)

1. （オプション）**[!UICONTROL カラー]**&#x200B;アイコンをクリックすると、相違点のハイライト表示に使用するカラーと不透明度を変更できます。

   ![proof_compare_color.png](assets/proof-compare-color.png)

### オーバーレイでのプルーフの比較 {#compare-proofs-in-an-overlay}

オーバーレイ比較を使用すると、2 つの静的プルーフを 1 つのプルーフとして表示すると同時に、プルーフの中央下に縦の区切り線を表示して、2 つの静的プルーフの相違点を表示できます。縦の区切り線をまたいでプルーフをパンすると、相違点が表示されます。

>[!NOTE]
>
>ビデオプルーフやインタラクティブプルーフを比較する場合は、オーバーレイ比較は使用できません。

オーバーレイ比較を有効にするには、次の手順に従います。

1. 次のいずれかの方法でプルーフの比較を開始します。

   * 同じプルーフの 2 つのバージョンを比較する（この記事の[プルーフバージョンの比較](#compare-proof-versions)を参照）。
   * 2 つの異なるプルーフを比較する（この記事の[別個のプルーフの比較](#compare-separate-proofs)を参照）

1. **[!UICONTROL オーバーレイ]**&#x200B;アイコンをクリックします。

   ![proof_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   2 つのプルーフは、プルーフの中央下に縦の区切り線が付いた 1 つのプルーフとして表示されます。

1. 次のいずれかの操作を行います。

   * 縦の区切り線をまたいでプルーフをパンします。パンしている間は、縦区切りの左側に左側のプルーフが表示され、右側に右側のプルーフが表示されます。
   * 縦の区切り線を左右に移動します。縦の区切り線を移動するにつれて、区切り線の左側に左側のプルーフが表示され、右側に右側のプルーフが表示されます。

### 同時ナビゲーション比較 {#simultaneous-navigation-comparison}

プルーフの比較時には、同時ナビゲーションがデフォルトで有効になっています。これは、静的プルーフどうしを比較する場合またはビデオプルーフどうしを比較する場合に使用できます。静的プルーフとビデオプルーフを比較する場合は使用できません。

**静的プルーフ：** 静的プルーフに対して有効にすると、同時ナビゲーションにより、パンまたはスクロール時に 2 つのプルーフのズームレベルと位置がロックされます。プルーフに複数のページが含まれ、同時ナビゲーションが有効な場合は、一方のプルーフでページを変更すると、もう一方のプルーフでもページが変更されます。

**ビデオプルーフ：** ビデオプルーフに対して有効にすると、2 つのプルーフのタイムラインの時間差が同時ナビゲーションで記憶されます。

まだ有効になっていない場合に同時ナビゲーションを有効にするには、次の手順に従います。

1. 次のいずれかの方法でプルーフの比較を開始します。

   * 同じプルーフの 2 つのバージョンを比較する（この記事の[プルーフバージョンの比較](#compare-proof-versions)を参照）。
   * 2 つの別個のプルーフを比較する（この記事の[別個のプルーフの比較](#compare-separate-proofs)を参照）

1. **[!UICONTROL 同時ナビゲーション]**&#x200B;アイコンをクリックします。

   ![proof_compare_simulante_icon.png](assets/proof-compare-simultaneous-icon.png)

1. （オプション）**[!UICONTROL リセット]**&#x200B;アイコンをクリックすれば、いつでもズームレベルと位置をリセット（静的プルーフの場合）したり、タイムラインをリセット（ビデオプルーフの場合）したりできます。

   ![proof_compare_simulante_reset.png](assets/proof-compare-simultaneous-reset.png)

## 比較モードの終了

1. 表示を終了するプルーフを閉じるには、プルーフの左上隅にある「x」アイコンをクリックします。

   ![proof_compare_exit.png](assets/proof-compare-exit-350x163.png)

   閉じないプルーフは、プルーフビューアで開いたままになります。
