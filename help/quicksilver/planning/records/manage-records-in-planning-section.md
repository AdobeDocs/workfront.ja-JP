---
title: Adobe Workfront オブジェクトの計画セクションでのレコードの管理
description: 左側のパネルにあるWorkfront オブジェクトの「計画」セクションに、Adobe Workfront オブジェクトに接続されたWorkfront計画レコードを表示できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: e82cf1b586ea3b08f419802bd1e88c6567b61b95
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 9%

---


<!--add also Group and Company when they are available-->

# Workfront オブジェクトからのレコード接続の管理

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Workfrontの次の領域に、Workfrontの計画レコードと、Adobe Workfront オブジェクトに接続されたそれぞれのレコードを表示できます。

* Workfront オブジェクトの「プランニング」セクション：オブジェクトに接続されているすべてのレコードタイプと、接続されたそれぞれのレコードを表示します。
* <span class="preview">Planning 接続のカスタム フィールド：1 つのレコード タイプとそれぞれの接続されたレコードが表示されます。</span>

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

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
   <p>Workfront Planning で、ワークスペースへのアクセス権を表示して接続レコードを表示するか、またはContribute以上のワークスペースへのアクセス権を表示してレコードを接続または切断 </a> ます。 </p>  
   <p>システム管理者には、未作成のワークスペースを含むすべてのWorkfront Planning ワークスペースに対する権限があります</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontオブジェクトのプランニング・エリアまたはプランニング・セクションを表示するには、メイン・メニューのプランニング・エリアとプロジェクト、ポートフォリオおよびプログラムのプランニング・エリアを含むすべてのユーザー（Workfront管理者を含む）にレイアウト・テンプレートを割り当てる必要があります。 </p> 詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">Adobe計画のアクセスの概要 </a> を参照してください。 </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 計画セクションのレコードの管理

Workfront オブジェクトの「プランニング」セクションを使用すると、Workfront オブジェクトに接続されているすべてのレコードタイプとそれぞれのレコードを表示できます。
「計画」セクションは、次のWorkfront オブジェクトで使用できます。

* プロジェクト
* ポートフォリオ
* プログラム
<!--* Group
* Company-->

### Workfront オブジェクトのプランニング セクションに関する考慮事項

Workfront オブジェクトの「計画」セクションからWorkfront Planning レコードを表示する場合は、次の点に注意してください。

* Workfront Planning レコードタイプは、まずWorkfront オブジェクトタイプに接続する必要があります。

  詳しくは、次の記事を参照してください。

   * [レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [レコードの接続](/help/quicksilver/planning/records/connect-records.md)
* Workfrontオブジェクトに関連付けられたレコードがない場合でも、Workfrontオブジェクトから「プランニング」セクションを表示できます。

### 計画セクションからのレコード接続の管理

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. Workfront プロジェクト、ポートフォリオ、またはプログラムに接続されているレコードタイプのカードをクリックします。
1. テーブル ビューまたはレコードの詳細ページから、Workfront オブジェクトに接続されている [ 接続済みレコード ] フィールドに移動します。 詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
1. 「接続されたレコード」フィールドでWorkfront オブジェクトの名前をクリックします。
Workfrontでオブジェクトのページが開きます。

   >[!NOTE]
   >
   >  Planning レコードに既に接続されているWorkfront オブジェクトがわかっている場合は、Workfront オブジェクトから Planning セクションに移動できます。

1. 左側のパネルで「**計画**」をクリックします。

   >[!NOTE]
   >
   >   Workfrontまたはグループの管理者は、Workfrontのプロジェクト、ポートフォリオまたはプログラムに表示される前に、計画セクションをレイアウトテンプレートに追加する必要があります。

   「計画」セクションには、次の情報が表示されます。

   * 接続されたレコードは、次の情報を含む個々のカードに表示されます。
      * レコードの名前
      * レコードのサムネール
      * Workfront Planning に表示される、接続されたレコードフィールドの名前。
   * レコードは、それぞれのワークスペースとレコードタイプの下に表示されます。

   ![](assets/planning-section-on-project.png)

1. （省略可能） [**すべての接続を表示**] をクリックすると、接続されたすべてのレコードの種類（接続されていないレコードを含む）が表示されます。 既定では、レコードが接続されていないレコード タイプは表示されません。
1. レコードカードをクリックすると、レコードに関する詳細情報が表示されます。 レコードのプレビューボックスが表示されます。
1. （オプション）レコードのプレビューボックスのフィールドの変更を開始します。 変更内容は自動的に保存されます。
1. （オプション）プレビューボックスの右上隅に ![](assets/open-details-in-a-new-tab-icon.png) る **新しいタブで開く** アイコンをクリックして、レコードの詳細ページを開きます。 Workfront Planning にレコードの詳細ページが開きます。
1. （オプション）レコードカードの上にマウスポインターを置き、「レコードを切断」アイコン（**-**）をクリックしてから「**切断**」をクリックします。
次のことが発生します。
   * レコードがWorkfront オブジェクトに接続されなくなりました。
   * Workfront オブジェクトも、Workfront Planning からレコードの接続されたフィールドから削除されます。
   * 計画レコードに接続されているWorkfront参照フィールドの値も削除されます。
1. 「**接続**」をクリックすると、接続されたレコードタイプのその他のレコードを接続できます。 詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

   次のことが発生します。

   * レコードは直ちにWorkfront オブジェクトに接続され、計画セクションに表示されます。
   * Workfront オブジェクトが、Workfront計画レコードの接続されたフィールドに追加されます。
   * 計画レコードに接続されたWorkfront参照フィールドの値は、Workfront Planning に入力されます。

<div class="preview">

## Planning 接続フィールド タイプのレコードの管理

Workfront オブジェクトに対して Planning 接続のカスタムフィールドを使用すると、1 つのレコードタイプと、Workfront オブジェクトに接続されたそれぞれのレコードを表示できます。

Planning 接続のカスタム・フィールドを作成するときに、Workfrontオブジェクトに表示する Planning レコード・タイプを制御できます。

* 「計画接続」フィールドには、接続が確立された後、および次のWorkfront オブジェクトのフォームにフィールドが添付されている場合に、計画レコードが表示されます。

   * プロジェクト
   * ポートフォリオ
   * プログラム
   * グループ
   * 会社

詳しくは、[ フォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

### Planning 接続フィールド・タイプに関する考慮事項

Workfrontオブジェクトの「Planning 接続」フィールドからWorkfront Planning レコードを表示する場合は、次の点に注意してください。

* 1 つの Planning 接続フィールドに関連付けることができるレコード・タイプは 1 つだけです。
* 正しいアクセス権がある場合は、Planning 接続カスタムフィールドを含むカスタムフォームを、Workfront Planning から接続できるWorkfront オブジェクトに添付する必要があります。
* Workfront Planning レコードタイプは、まずWorkfront オブジェクトタイプに接続する必要があります。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* Workfront オブジェクトの Planning 接続フィールドに対するレコードの接続または切断は、Workfront Planning 接続を持つことができるオブジェクトに対してのみ行うことができます。
* Workfront オブジェクトの Planning 接続フィールドにレコードを接続または接続解除するには、Workfront Planning のワークスペースのContribute権限が必要です。
* Workfrontオブジェクトを一括編集する場合は、Planning 接続フィールドを編集できません。

### 計画接続フィールドタイプからのレコード接続の管理

1. Workfront Planning レコード タイプに接続されている次のオブジェクト タイプのいずれかに移動します：

   * プロジェクト
   * ポートフォリオ
   * プログラム
   * 会社
   * グループ

1. 左側のパネルで **&lt; オブジェクト /詳細** をクリックします。
1. （条件付き）選択したオブジェクトに対して 1 つ以上の Planning 接続フィールドを持つカスタムフォームを追加します（存在しない場合）。

   >[!NOTE]
   >
   >オブジェクトに追加する前に、Workfrontまたはグループ管理者が最初にフォームを作成し、そのフォームに Planning 接続フィールドを追加する必要があります。


1. フィールド内をクリックして接続レコードを追加し、フィールド内の下向き矢印をクリックして、リストからレコードを選択します。

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >フィールドの設定時に選択したオブジェクト以外のWorkfront オブジェクトに関連付けられている Planning 接続フィールドにレコードを追加することはできません。
   >
   >例えば、プロジェクトのカスタムフォームからPortfolio用に作成された Planning 連携フィールドにレコードを追加することはできません。
   >
   >フィールドのオブジェクトと選択したオブジェクトが一致しない場合があります。
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. リストの外側をクリックして閉じます。

   次のことが発生します。

   * レコードは直ちにWorkfront オブジェクトに接続され、Planning 接続フィールドとWorkfront オブジェクトの Planning セクションに表示されます。
   * Workfront オブジェクトが、Workfront計画レコードの接続されたフィールドに追加されます。
   * 計画レコードに接続されたWorkfront参照フィールドの値は、Workfront Planning に入力されます。
1. （オプション）「Planning 接続」フィールドのレコード名をクリックして、Workfront Planning で開きます。
Workfront Planning で「レコードの詳細」タブが開きます。
レコードに関する情報を確認するか、レコードタイプページに移動できます。

1. （オプション）Workfrontのカスタムフォームで、レコードの ![](assets/remove-icon.png) にある **削除** アイコンをクリックして、Planning 接続フィールドから削除し、Workfront オブジェクトから切断します。
Workfront オブジェクトは計画レコードから切断され、Workfrontからのルックアップ情報はレコードから削除されます。

</div>