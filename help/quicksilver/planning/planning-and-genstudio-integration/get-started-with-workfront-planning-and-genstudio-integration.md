---
title: Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ
description: GenStudio for Performance Marketing Workspace は、会社が両方の製品を購入すると、Adobe Workfront Planning で使用できるようになります。 この統合を使用してワークフローを効率化する方法に関する基本をいくつか説明します。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1475'
ht-degree: 6%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの統合の基本を学ぶ

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの両方を使用している組織では、多くの場合、キャンペーン、商品、ペルソナなどのマーケティング概念を、GenStudioがデフォルトでサポートしている概念よりも詳細に定義しています。

GenStudio for Performance MarketingとWorkfront Planning はネイティブで統合されています。 この統合により、Workfront Planning のユーザーはGenStudioで使用されるキャンペーン、製品、ペルソナ、アクティベーション、チャネルおよびリージョンを管理できるようになります。 また、Workfront Planning から既存のレコードタイプを参照するようにGenStudioを設定して、より接続された一貫性のあるマーケティングワークフローを作成することもできます。

GenStudio for Performance Marketing Workspace は、会社が両方の製品を購入すると、Adobe Workfront Planning で使用できるようになります。

## 統合のメリット

Workfront Planning とGenStudio for Performance Marketingの統合により、次のことができます。

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Workfront Planning でGenStudioワークスペースを表示します。
* GenStudioのキャンペーンを変更し、Workfront Planning で同じ情報をリアルタイムで更新します。
* Workfront Planning でキャンペーンを変更し、GenStudioで同じ情報をリアルタイムで更新します。
* 重複するデータ入力を避けます。
* 計画とアクティブ化の取り組み間の整合性を維持します。

## 統合要件

* WorkfrontとGenStudio for Performance Marketingは、同じ組織に対して有効にする必要があります。

  GenStudioについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

* 会社に複数のWorkfront インスタンスがある場合、Workfront Planning でGenStudioを使用できません。<!--this will change-->

* Workfront インスタンスは、Identity Management System （IMS）の使用を含む、Adobe統合エクスペリエンスの一部です。

  詳しくは、[WorkfrontのAdobe統合エクスペリエンス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。

* Planning とGenStudioの両方を使用するユーザーは、IMS 組織内の 1 つのWorkfrontインスタンスにのみ属できます。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## アクセス要件

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のAdobe Workfront ワークフローパッケージ</p>
<p>任意のAdobe Workfront Planning パッケージ</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio パッケージ</p></td> 
   <td> 
<p>???GEN STUDIO には、これをサポートするパッケージがありま？??。</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p> 標準</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio ライセンス</p></td> 
   <td><p> ???GEN STUDIO には、これをサポートする特定のライセンスが必要で？??。</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>  
   <p>GenStudioの設定：???GENS に必要なアクセスレベルは？??</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクトの権限*</p></td> 
   <td>  
   <p>Workfrontの計画では、次の操作を行います。 </p>
   <ul>
   <li><p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p> </li> 
   <li><p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p></li>
   </ul>
   <p>Adobe GenStudio for Performance Marketingで： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketingのすべての権限</p></li>
   <li><p> Adobe GenStudio for Performance Marketingでアイテムを作成する権限を作成する</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。
*Adobe GenStudio for Performance Marketingについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。


## Workfront Planning とGenStudioの統合の概要

以下の節では、以下について説明します。

* GenStudioからWorkfront Planning の情報を更新する機能
* Workfront Planning からGenStudio情報を更新する機能
* Workfront Planning のGenStudio Workspace で管理できる内容と管理できない内容に関する制限。

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront Planning のGenStudio ワークスペース

* お客様の組織に複数のWorkfront インスタンスがある場合、GenStudio Workspace は、お使いのWorkfront インスタンスからは表示されません。<!-- this might change-->
* GenStudio Workspace には、GenStudioから読み込まれていることを示す視覚的なインジケーターが表示されます。 詳しくは、[Adobe Workfront Planning でのGenStudio Workspace の管理 ](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md) を参照してください。
* GenStudioとWorkfront Planning の両方のアクセス権を持つすべてのユーザーは、Workfront Planning のGenStudio Workspace も参照できます。
* Workfront Planning ユーザーがWorkfrontからGenStudio Workspace を表示して使用するには、Adobe Identity Management System （IMS）を通じて管理される必要があります。

  Workfrontのみのユーザーには、Workfrontで使用可能な場合でも、GenStudio workspace は表示されません。

  詳しくは、[WorkfrontのAdobe統合エクスペリエンス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。


### レコードタイプ

* GenStudio レコードタイプに関する情報（外観など）は、Workfront Planning から編集できます。
* GenStudio レコードタイプは、Planning で他のユーザーと共有できます。
* レコードタイプは、GenStudio Workspace の Planning から作成できます。 これらのレコードタイプは、Planning でのみ残ります。 GenStudioには表示されません。
* GenStudioと同期されたレコードタイプには、GenStudioからレコードタイプが読み込まれていることを示す視覚的なインジケーターがWorkfront Planning に表示されます。

### レコード

GenStudioとWorkfront Planning の両方に表示されるGenStudio レコードタイプに属するレコードの場合、次のことが可能です。

* GenStudio内のレコードを追加または削除すると、Workfront Planning に表示される（または削除される）ことができます。
* Workfront Planning でレコードを追加または削除すると、GenStudioに表示される（または削除される）ようになります。
* Workfront Planning またはGenStudioからレコードを削除すると、それらのレコードはWorkfront Planning の最近削除されたレコード・ビンに 30 日間配置されます。 GenStudioには、最近削除された bin がありません。
* 最近削除された bin からレコードを復元すると、Workfront Planning とGenStudioに戻ります。
* Workfront Planning からレコードを追加するには、次の方法があります。

   * 新規レコードボタンを使用して、任意のビューからゼロから手動で
   * CSV または Excel ファイルを使用してインポートする
   * 手動、インライン、テーブルビュー
   * 手動で、タイムラインまたはカレンダー表示 <!--ensure the calendar is released when this releases--> ージで直接移動

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* Workfront Planning から有効化レコードを作成または削除することはできません。
* Workfront Planning の表示可能な任意のフィールドで、GenStudio Workspace 内のすべてのレコードに関するレコード情報を Planning 内で編集できます。

  詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### フィールド

* レコードフィールドは、GenStudioから読み込まれます。 Workfront Planning からGenStudioのフィールド設定を編集できます。
* Gen Studio の管理アクセス権がある場合は、Workfront Planning でGenStudio レコードタイプのフィールドを作成できます。
* Planning でGenStudioレコード・タイプのフィールドを作成すると、次の領域から表示されます：
   * 計画ビュー
   * 計画レコードの詳細ページ
   * GenStudio レコードの詳細ページ

  >[!TIP]
  >
  >Workfront Planning で作成されたフィールドは、GenStudioのリスト表示には表示されません。

* Planning のGenStudioレコード・タイプのテーブル・ビューでフィールドを非表示にできます。
* Workfront Planning からGenStudioからインポートされたフィールドは削除できません。
* Workfront Planning から、Workfront Planning で作成されたGenStudioレコードタイプのフィールドを削除できます。

### 作成者フィールドと承認者フィールド

* Workfront Planning 内のWorkfront Planning のレコード タイプに対して、[ 作成者 ] フィールドと [ 承認者 ] フィールドをGenStudio Planning から追加できます。
* チャネルおよび地域レコードタイプに表示されるレコードには、作成者ユーザーとして「システム」と表示されます。 これらのレコードは、Workfront Planning でGenStudio Workspace を作成すると、自動的に作成されます。
* Workfront Planning でワークスペースが使用可能になった後にGenStudioで作成されたレコードには、作成者フィールドにレコードを作成した IMS ユーザーの名前が表示されます。ユーザーがWorkfront ユーザーでなくて、GenStudioでレコードを作成した場合でも同様です。
* 「承認者」フィールドには、Workfront Planning でGenStudio レコードタイプのレコードを作成するためにリクエストフォームが送信された際に、承認者の名前が表示されます。

### ビュー

* GenStudio レコードタイプのビューを作成できます。

  詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

* GenStudio レコードタイプのビューを共有することは、Planning レコードタイプのビューを共有することと同じです。
* GenStudioでは、複数のビューを作成できません。

### 接続

* Workfront Planning では、GenStudioレコード・タイプと他のレコードまたはオブジェクト・タイプを次のように関連付けることができます。

   * 2 つのGenStudio レコードタイプ
   * 同じワークスペースからのGenStudio レコードタイプと Planning レコードタイプ
   * 別の作業領域から接続するようにレコード・タイプが構成されている場合、別の作業領域からのGenStudioレコード・タイプおよび計画レコード・タイプ。
   * GenStudio レコードタイプとWorkfront オブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム、会社、グループ）
   * GenStudio レコードタイプとAEM Assets オブジェクトタイプ。

### リクエストフォームと自動化

* リクエストフォームは、Workfront Planning のGenStudio レコードタイプに追加できます。
* Workfront Planning で、GenStudio レコードタイプの自動化を設定できます。

### プレビュー環境

* 実稼動環境からアクセスできるGenStudio Workspace は、プレビュー環境でも表示されます。
* プレビュー環境にあるWorkfront Planning のGenStudio Workspace で、この記事に記載されているすべてのアクティビティを実行できますが、これらの変更内容はGenStudioに転送されません。
実稼動環境で項目に加えた変更のみが、Workfront Planning とGenStudioの間で同期されます。
GenStudioにはプレビュー環境がありません。

