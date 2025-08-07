---
title: Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ
description: GenStudio for Performance Marketing Workspace は、会社が両方の製品を購入すると、Adobe Workfront Planning で使用できるようになります。 この統合を使用してワークフローを効率化する方法に関する基本をいくつか説明します。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 36cd1c23dfb6e01dc1016a6a12ae47e4f9172d20
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 8%

---

# Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ

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

Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの両方を使用している組織では、多くの場合、キャンペーン、商品、ペルソナなどのマーケティング概念を、GenStudioがデフォルトでサポートしている概念よりも詳細に定義しています。

GenStudio for Performance MarketingとWorkfront Planning はネイティブで統合されています。 この統合により、Workfront Planning のユーザーはGenStudioで使用されるキャンペーン、製品、ペルソナ、アクティベーション、チャネルおよびリージョンを管理できるようになります。 また、Workfront Planning から既存のレコードタイプを参照するようにGenStudioを設定して、より接続された一貫性のあるマーケティングワークフローを作成することもできます。

この統合により、データ入力の重複を回避し、計画とアクティブ化の取り組み間の整合性を維持し、レコードのマーケティングシステムをサポートできます。

GenStudio for Performance Marketing Workspace は、会社が両方の製品を購入すると、Adobe Workfront Planning で使用できるようになります。

Workfront Planning とGenStudio for Performance Marketingの統合により、次のことができます。

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Workfront Planning でGenStudioワークスペースを表示します。
* GenStudioのキャンペーンを変更し、Workfront Planning で同じ情報をリアルタイムで更新します。
* Workfront Planning でキャンペーンを変更し、GenStudioで同じ情報をリアルタイムで更新します。

## 統合要件

* WorkfrontとGenStudio for Performance Marketingは、同じ組織に対して有効にする必要があります。

  GenStudioについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

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
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
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
   <td><p> システム管理者</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


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

* レコードタイプ情報（外観など）は、Workfront Planning のGenStudioから編集できます。
* GenStudio レコードタイプは、Planning で他のユーザーと共有できます。 <!--checking with Ani H.-->
* レコードタイプは、GenStudio Workspace の Planning から作成できます。<!-- checking with Ani where these show up in GenS-->
* GenStudioと同期されるレコードタイプには、そのレコードタイプがGenStudioから読み込まれていることを示す視覚的なインジケーターが表示されます。

### レコード

* GenStudio内のレコードを追加または削除すると、Workfront Planning に表示される（または削除される）ことができます。
Workfront Planning でレコードを追加または削除すると、GenStudioに表示される（または削除される）ようになります。
* Workfront Planning からレコードを追加するには、次の方法があります。

   * 新規レコードボタンを使用して、任意のビューからゼロから手動で
   * CSV または Excel ファイルを使用してインポートする
   * 手動、インライン、テーブルビュー
   * 手動で、タイムラインビューで直接移動

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* Workfront Planning から有効化レコードを作成または削除することはできません。
* Workfront Planning の表示可能な任意のフィールドで、GenStudio Workspace 内のすべてのレコードに関するレコード情報を Planning 内で編集できます。

  詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### フィールド

* レコードフィールドは、GenStudioから読み込まれます。 Workfront Planning でフィールド設定を編集できます。
* Gen Studio の管理アクセス権がある場合は、Workfront Planning でGenStudio レコードタイプのフィールドをさらに作成できます。
* Planning でGenStudioレコード・タイプのフィールドを作成すると、次の領域から表示されます：
   * 計画ビュー
   * 計画レコードの詳細ページ
   * GenStudio レコードの詳細ページ

  >[!TIP]
  >
  >Workfront Planning で作成されたフィールドは、GenStudioのリスト表示には表示されません。

* Planning のGenStudioレコードタイプのテーブル表示でフィールドを非表示にすることはできますが、Workfront Planning からフィールドを削除することはできません。


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### ビュー

* GenStudio レコードタイプのビューを作成できます。

  詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

* GenStudio レコードタイプのビューは、Planning レコードタイプのビューと同じように共有できます。

### 接続

* Workfront Planning では、GenStudioレコード・タイプと他のレコードまたはオブジェクト・タイプを次のように関連付けることができます。

   * 2 つのGenStudio レコードタイプと
   * 同じワークスペースからのGenStudio レコードタイプと Planning レコードタイプ
   * 別の作業領域から接続するようにレコード・タイプが構成されている場合、別の作業領域からのGenStudioレコード・タイプおよび計画レコード・タイプ。
   * GenStudio レコードタイプとWorkfront オブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム、会社、グループ）