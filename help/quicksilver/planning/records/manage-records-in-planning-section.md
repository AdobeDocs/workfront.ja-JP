---
title: Adobe Workfront オブジェクトの計画セクションでのレコードの管理
description: 左側のパネルでは、Adobe Workfront オブジェクトの「計画」セクションで、Workfront オブジェクトに接続されているレコードを表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 11%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->

<!-- opening the Details preview and page is not possible yet - hid those steps, but add them when released-->


# Adobe Workfront オブジェクトの計画セクションでのレコードの管理

{{planning-important-intro}}

左側のパネルでは、Adobe Workfront オブジェクトの「計画」セクションで、Workfront オブジェクトに接続されているレコードを表示できます。

「計画」セクションは、次のWorkfront オブジェクトで使用できます。

* プロジェクト
* ポートフォリオ
* プログラム
<!--* Group
* Company-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 契約</p></td>
   <td>
<p>Workfront Planning の早期アクセス段階に登録されている必要があります </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>新規：標準</p>
   または
   <p>現在：プラン</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>プロジェクト、プログラム、Portfolioへの表示以上のアクセス</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>Workfrontで、プロジェクト、ポートフォリオまたはプログラムに対する表示以上の権限</a> </p> 
   <p>Workfront Planning で、Contribute以上の作業領域への権限</a> </p>  
   <p>システム管理者には、未作成のワークスペースを含むすべてのWorkfront Planning ワークスペースに対する権限があります</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、メインメニューのプランニング エリアと左側のパネルのプランニング セクションをレイアウトテンプレートに追加する必要があります。 詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## Workfront オブジェクトのプランニング セクションに関する考慮事項

* まず、レコードタイプをWorkfront オブジェクトタイプに関連付け、レコードをWorkfront オブジェクトに関連付けて、Workfrontで表示できるようにする必要があります。

  詳しくは、次の記事を参照してください。

   * [レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [レコードの接続](/help/quicksilver/planning/records/connect-records.md)
* Workfront オブジェクトにはレコードが関連付けられていない場合でも、Workfront オブジェクトの「プランニング」セクションを表示できます。
* 1 つ以上のレコードがWorkfront オブジェクトに接続されている場合は、「計画」セクションのWorkfrontのWorkfront オブジェクトに計画レコードを関連付けることができます。

## 計画セクションのレコードの管理

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. Workfront プロジェクト、ポートフォリオ、またはプログラムに接続されているレコードタイプのカードをクリックします。
1. テーブル ビューまたはレコードの詳細ページから、Workfront オブジェクトに接続されている [ 接続済みレコード ] フィールドに移動します。 詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
1. 「接続されたレコード」フィールドでWorkfront オブジェクトの名前をクリックします。
Workfront Planning にオブジェクトのページが開きます。
1. クリック **ソースに移動**&#x200B;をクリックします。

   Workfrontでオブジェクトのページが開きます。
1. クリック **計画** 左側のパネルで次の操作を行います。

   >[!NOTE]
   >
   >   Workfront のプロジェクト、ポートフォリオ、またはプログラムに表示する前に、Workfront管理者またはグループ管理者がレイアウトテンプレートに「プランニング」セクションを追加する必要があります。

   「計画」セクションには、次の情報が表示されます。

   * 接続されたレコードは、次の情報を含む個々のカードに表示されます。
      * レコードの名前
      * レコードのサムネール
      * Workfront Planning に表示される、接続されたレコードフィールドの名前。
   * レコードは、それぞれのワークスペースの下に表示されます。

   ![](assets/planning-section-on-project.png)

1. レコードカードをクリックすると、レコードに関する詳細情報が表示されます。 レコードのプレビューボックスが表示されます。
1. （オプション）レコードのプレビューボックスのフィールドの変更を開始します。 変更内容は自動的に保存されます。
1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) プレビューボックスの右上隅でをクリックして、レコードの詳細ページを開きます。 Workfront Planning にレコードの詳細ページが開きます。
1. レコードカードの上にマウスポインターを置き、レコードを切断アイコンをクリックします **-**&#x200B;を選択し、 **連携解除**.
次のことが発生します。
   * レコードがWorkfront オブジェクトに接続されなくなりました。
   * Workfront オブジェクトも、Workfront Planning からレコードの接続されたフィールドから削除されます。
   * 計画レコードに接続されているWorkfront参照フィールドの値も削除されます。
1. クリック **接続** より多くのレコードを接続します。

   >[!NOTE]
   >
   >   「接続」ボタンは、Contributeの権限を持つワークスペースに対してのみ表示されます。 <!--they might replace this with one button at the top of the page. Rephrase-->

1. 接続するレコードをクリックします。 次のことが発生します。

   * レコードは直ちにWorkfront オブジェクトに接続され、計画セクションに表示されます。
   * Workfront オブジェクトが、Workfront計画レコードの接続されたフィールドに追加されます。
   * 計画レコードに接続されたWorkfront参照フィールドの値は、Workfront Planning に入力されます。

<!--add more steps here for what happens after clicking Connect-->
