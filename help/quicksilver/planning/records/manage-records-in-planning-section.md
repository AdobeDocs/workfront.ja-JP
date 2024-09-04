---
title: Adobe Workfront オブジェクトの計画セクションでのレコードの管理
description: 左側のパネルにあるWorkfront オブジェクトの「計画」セクションに、Adobe Workfront オブジェクトに接続されたWorkfront計画レコードを表示できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 10%

---


<!--add also Group and Company when they are available-->

# Adobe Workfront オブジェクトの計画セクションでのレコードの管理

{{planning-important-intro}}

左側のパネルにあるWorkfront オブジェクトの「計画」セクションに、Adobe Workfront オブジェクトに接続されたWorkfront計画レコードを表示できます。

「計画」セクションは、次のWorkfront オブジェクトで使用できます。

* プロジェクト
* ポートフォリオ
* プログラム
<!--* Group
* Company-->

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

Workfront Planning にアクセスするには、次のものが必要です：

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
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfrontの計画<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
<p>次のいずれかのWorkfront プラン：</p>
<ul><li>選択</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront計画*</p></td>
   <td>
<p>任意</p>
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>プロジェクト、プログラム、Portfolioへの表示以上のアクセス</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>Workfrontで、プロジェクト、ポートフォリオまたはプログラムに対する表示以上の権限 </a> </p> 
   <p>Workfront Planning で、Contribute以上の作業領域への権限 </a> </p>  
   <p>システム管理者には、未作成のワークスペースを含むすべてのWorkfront Planning ワークスペースに対する権限があります</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューの計画領域と、プロジェクト、ポートフォリオおよびプログラムの計画領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> 詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md"> アクセスの概要 </a> を参照してください。 </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront オブジェクトのプランニング セクションに関する考慮事項

* Workfront Planning レコードタイプは、Workfront オブジェクトタイプに接続されている必要があります。

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
Workfrontにオブジェクトのページが開きます。

1. 左側のパネルで「**計画**」をクリックします。

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

1. （省略可能） [**すべての接続を表示**] をクリックすると、接続されたすべてのレコードの種類（接続されていないレコードを含む）が表示されます。 既定では、レコードが接続されていないレコード タイプは表示されません。
1. レコードカードをクリックすると、レコードに関する詳細情報が表示されます。 レコードのプレビューボックスが表示されます。
1. （オプション）レコードのプレビューボックスのフィールドの変更を開始します。 変更内容は自動的に保存されます。
1. （オプション）プレビューボックスの右上隅に ![](assets/open-details-in-a-new-tab-icon.png) る **新しいタブで開く** アイコンをクリックして、レコードの詳細ページを開きます。 Workfront Planning にレコードの詳細ページが開きます。
1. レコードカードにポインタを合わせ、「レコードを切断」アイコン（**-**）をクリックしてから、「**切断**」をクリックします。
次のことが発生します。
   * レコードがWorkfront オブジェクトに接続されなくなりました。
   * Workfront オブジェクトも、Workfront Planning からレコードの接続されたフィールドから削除されます。
   * 計画レコードに接続されているWorkfront参照フィールドの値も削除されます。
1. 「**接続**」をクリックすると、接続されたレコードタイプのその他のレコードを接続できます。 詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

   次のことが発生します。

   * レコードは直ちにWorkfront オブジェクトに接続され、計画セクションに表示されます。
   * Workfront オブジェクトが、Workfront計画レコードの接続されたフィールドに追加されます。
   * 計画レコードに接続されたWorkfront参照フィールドの値は、Workfront Planning に入力されます。


