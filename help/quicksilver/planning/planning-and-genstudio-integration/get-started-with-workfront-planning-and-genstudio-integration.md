---
title: Workfront計画とGenStudio for Performance Marketingの統合の基本を学ぶ
description: GenStudio for Performance Marketing Workspaceは、Adobe Workfront Planningで両方の製品を購入した場合に使用できます。 この統合を使用してワークフローを合理化する方法の基本を説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Dzo6SD-mf-89koGS55sYT8gSk7z1U7aEyrg1MzSEHGY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 2402
ht-degree: 3%

---

<!--
Better metadata, at publishing:
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


# Adobe Workfront Planning と Adobe GenStudio for Performance Marketing の統合の基本を学ぶ

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

多くの場合、Adobe Workfront PlanningとAdobe GenStudio for Performance Marketingの両方を使用している企業は、GenStudioがデフォルトでサポートしている内容よりも、キャンペーン、製品、アクティベーション、ペルソナなどのマーケティングコンセプトをより詳細に定義しています。

GenStudio for Performance MarketingとWorkfront Planningはネイティブで統合されています。 この統合により、Workfront Planningのユーザーは、GenStudioで使用されるキャンペーン、製品、ペルソナ、アクティベーション、チャネル、リージョンを管理できます。 また、Adobe GenStudioを設定して、Workfront Planningの既存のレコードタイプを参照できるようにすることで、より連続性のある一貫性のあるマーケティングワークフローを構築できます。

GenStudio for Performance Marketing Workspaceは、Adobe Workfront Planningで両方の製品を購入した場合に使用できます。

## 統合の利点

Workfront PlanningとGenStudio for Performance Marketingの統合により、次のことが可能になります。

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Workfront PlanningのGenStudio Workspaceを表示します。
* GenStudio for Performance Marketingでキャンペーン、製品、ペルソナ、リージョン、アクティベーションを変更し、Workfront Planningで同じ情報をリアルタイムで更新できます。
* Workfront Planningでキャンペーン、製品、ペルソナ、アクティベーションを変更し、GenStudio for Performance Marketingで同じ情報をリアルタイムに更新できます。
* 重複したデータ入力を避ける：
* 計画とアクティベーションの取り組み全体で整合性を維持。
* GenStudio Brandsとその情報を、Workfront Planning レコードに接続します。
* キャンペーン、製品、ペルソナ、リージョン、チャネルに関するGenStudio情報を、PlanningのGenStudio Workspaceでこれらのレコードタイプに接続する際に、AEM Assetsおよびコンテンツフラグメントに同期します。

## 統合要件

Workfront PlanningとGenStudio for Performance Marketingの統合を実現するには、次の要件を満たす必要があります。

* WorkfrontとGenStudio for Performance Marketingは、同じ組織で有効にする必要があります。

  GenStudioについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home)を参照してください。

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

<!--
No longer needed to specify:
* Your Workfront instance is part of the Adobe Unified Experience, including using the Identity Management System (IMS). 

    For information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
-->

* Workfront PlanningとGenStudio for Performance Marketingの両方を使用するユーザーは、IMS組織内の1つのWorkfront インスタンスにのみ属する必要があります。

  Workfrontのみのユーザーは、GenStudio for Performance Marketing ユーザーでない場合でも、GenStudio ワークスペースを表示できます。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## アクセス要件

次の表に、Adobe GenStudio for Performance MarketingでAdobe Workfront Planningを使用するためのアクセス要件と権限要件を示します。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよびプランニングパッケージ</p> <p>任意のワークフローとプランニングパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
   </td> 
   <tr> 
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketingのユーザーロール</p></td> 
   <td><p><ul><li>キャンペーン、商品、ペルソナにアクセスするためのGenStudioのユーザーロール</li>
   <li>GenStudio System Managerからアクティベーションにアクセス <!--and Events--></li></ul>
   詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> ユーザーの役割と権限</a>を参照してください。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  
   <p>Workfront Planningでは、次の操作を行います。 </p>
   <ul>
   <li><p>GenStudio ワークスペースへの権限を管理して、新しいフィールドまたはレコードタイプをGenStudio ワークスペースに追加します</p></li>
   <li><p>GenStudio ワークスペースにアクセス権を付与して、GenStudio ワークスペース内のレコードを追加、更新、削除します</p> </li>  
   </ul>
   <p>Workfront PlanningのGenStudio WorkspaceからGenStudio for Performance Marketing レコードタイプまたはフィールドを削除することはできません</p>
   <p>Adobe GenStudio for Performance Marketingで： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketingのすべての権限</p></li>
   <li><p> Adobe GenStudio for Performance Marketingで権限を作成して項目を作成する</p></li></ul>
   </td>  
</tbody> 
</table>

Adobe Workfront計画アクセスについて詳しくは、[Adobe Workfront計画アクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。

Adobe GenStudio for Performance Marketingについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home)を参照してください。

<!--
Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****and Events****</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>
-->

## Workfront計画とGenStudio for Performance Marketing統合機能の概要

組織が保有するWorkfront インスタンスの数に応じて、PlanningのGenStudio ワークスペースに対する次の権限が自動的に付与されます。

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Workfrontの1つのインスタンス</p></td> 
   <td> 
<p>GenStudio Workspaceは、Workfront Planningのインスタンスに表示されます</p>
<p>Workfront管理者を含むすべてのユーザーは、デフォルトでPlanningのGenStudio WorkspaceにContribute アクセスできます</p>
<p>Workfront管理者は、GenStudio Workspaceの管理権限を誰にでも変更および付与できます</p>
</td> </tr>
   <tr> 
<td> 
   <p> Workfrontの複数のインスタンス数</p> </td> 
   <td> 
   <p>Workfront Planningを使用したWorkfrontのインスタンスが複数ある場合のシナリオを以下に示します。</p>
   <ul><li>Adobe GenStudio for Performance Marketingを購入する時点で複数のWorkfront インスタンスが存在する場合、すべてのWorkfront インスタンスからGenStudio ワークスペースが表示されます。</li>
   <li>元のインスタンスが既にAdobe GenStudio for Performance Marketingと統合された後にWorkfront インスタンスを追加する場合、GenStudio ワークスペースは元のWorkfront インスタンスからのみ表示されます。 Workfrontのその他のインスタンスをAdobe GenStudioに接続する方法については、アカウント担当者にお問い合わせください。 </li></ul>    
</td> 
  </tr>
   </tbody> 
</table>

<!--
Old for the second row in the table:

<p>The GenStudio workspace is visible from all Workfront instances</p>
<p>All users with access to GenStudio for Performance Marketing and Workfront Planning have Contribute permissions on the GenStudio in Planning by default</p> 
<p>Workfront administrators cannot grant Manage permissions to the GenStudio workspace to anyone</p>
-->

Workfront Planningの権限について詳しくは、[Adobe Workfront Planningでの共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

以下の節では、次の点について説明します。

* GenStudio for Performance MarketingからWorkfront計画情報を更新する機能
* Workfront PlanningからGenStudio for Performance Marketing情報を更新する機能
* Workfront PlanningのGenStudio Workspaceで管理できる機能と管理できない機能に関する制限。

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront PlanningのGenStudio Workspaceは

* GenStudio ワークスペースは、Workfront計画に視覚的なインジケーターを表示して、GenStudio for Performance Marketing ワークスペースを表すものとして識別します。

  計画中の![GenStudio カード &#x200B;](assets/genstudio-card-with-tag-highlighted.png)

  詳しくは、[Adobe Workfront PlanningでのGenStudio Workspaceの管理](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)を参照してください。
* GenStudio Workspaceは、Workfront Planningで作成されたときにWorkfrontにアクセスできるすべてのGenStudio ユーザーと自動的に共有されます。
* PlanningのGenStudio Workspaceのワークスペースマネージャーとして、次のことができます。

   * PlanningでGenStudio ワークスペースを更新します（名前、説明、アイコン）
   * セクションを作成
   * レコードタイプを追加
   * 他のユーザーとの共有

     >[!NOTE]
     >
     >* GenStudio Workspaceは、GenStudio アカウントを持たない他のユーザーと共有できます。 組織のIdentity Management システム（IMS）で使用可能なユーザーにのみ共有できます。
     >* GenStudio ユーザーをGenStudio ワークスペースまたはそのレコードタイプの共有から削除することはできません。

  <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* PlanningのGenStudio Workspaceに対するContribute権限がある場合、Workfront PlanningからWorkspaceを変更することはできません。

### GenStudio ワークスペースのレコードタイプ

* GenStudio for Performance MarketingとPlanningの両方に表示されるレコードタイプには、Workfront PlanningのGenStudio インジケーターがあります。

  ![Workfront計画のGenStudio レコードタイプ カード &#x200B;](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* GenStudio ワークスペースのレコードタイプは、プランニングでワークスペースを作成するときにWorkfrontにもアクセスできるすべてのGenStudio ユーザーと自動的に共有されます。
* PlanningのGenStudio Workspaceに対する管理権限がある場合は、Workfront Planningから次の操作を実行できます。
   * GenStudioのレコードタイプ情報（外観、詳細設定）を編集します。
   * GenStudioのレコードタイプを他のユーザーと共有します。 GenStudio レコードタイプの共有からGenStudio ユーザーを削除することはできません。
   * レコードタイプの作成： これらのレコードタイプは、Workfront Planningにのみ残ります。 GenStudioには表示されません。
   * GenStudio ワークスペースのレコードタイプを有効にして、他のワークスペースから接続します。
   * GenStudio ワークスペースのレコードタイプを有効にして、他のワークスペースに追加できます。
* PlanningのGenStudio Workspaceに対するContribute権限がある場合、PlanningからGenStudio レコードタイプを変更することはできません。

### GenStudio ワークスペースのレコード

* すべてのGenStudio レコードは、プランニングでワークスペースを作成するときにWorkfrontにアクセスできるすべてのGenStudio ユーザーと自動的に共有されます。
* GenStudio for Performance MarketingからGenStudio レコードを編集すると、変更内容はWorkfrontのすべてのインスタンスのGenStudio ワークスペースに表示されます。
* Workfront PlanningのGenStudio ワークスペースからアクティベーションレコードを作成または削除することはできません。
* PlanningのGenStudio Workspaceに対する管理権限またはコントリビュート権限がある場合は、Workfront Planningから次の操作を実行できます。
   * レコードを追加または削除すると、レコードはGenStudio for Performance Marketingで表示されます（または削除されます）。

     Workfront計画またはGenStudio for Performance Marketingから削除されたレコードは、30日間、「最近削除されたWorkfront計画」ビンに配置されます。 GenStudio for Performance Marketingには、「最近削除されたビン」がありません。
   * 最近削除したビンからレコードを復元します。 削除されたレコードを復元すると、Workfront PlanningおよびGenStudio for Performance Marketingに戻されます。
   * 次の方法でレコードを追加します。

      * 新規レコードボタンを使用して、任意のビューから手動で最初から
      * テーブルビューでCSVまたはExcel ファイルを使用してインポートすることで
      * Workfront Planningの任意のビューでの手動
      * Workfrontのレコードタイプのリクエストフォームにリクエストを送信します。

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* Workfront Planningから、GenStudio Workspaceのすべてのレコードに関するレコード情報を編集できます。

  詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

### GenStudio ワークスペースのレコードタイプフィールド

レコードタイプフィールドは、デフォルトでGenStudio for Performance MarketingからWorkfront Planningに読み込まれます。

また、PlanningからGenStudio Workspaceで、レコードタイプのPlanning フィールドを作成することもできます。

GenStudioのレコードタイプフィールドについては、次の点を考慮してください。

* PlanningのGenStudio Workspaceに対する管理権限がある場合は、Workfront Planningから次の操作を実行できます。

   * GenStudioのフィールド設定を編集します。
   * GenStudio レコードタイプのフィールドを作成します。

     PlanningでGenStudio レコードタイプのフィールドを作成すると、次の領域から表示されます。

      * Workfront計画ビュー
      * Workfront計画レコードの詳細ページ
      * GenStudio レコードの詳細ページ

     >[!TIP]
     >
     >Workfront Planningで作成されたフィールドは、GenStudio リストには表示されません。

   * Workfront PlanningのGenStudio レコードタイプのテーブルビューでフィールドを非表示にします。
   * GenStudioで作成されたフィールドをWorkfront Planningから削除することはできません。

* PlanningのGenStudio Workspaceに対するContribute権限がある場合：

   * Workfront PlanningのGenStudio ワークスペースでは、フィールド設定の編集、フィールドの削除または追加はできません。
   * Workfront Planningのテーブルビューでは、フィールドを非表示にできます。

#### 作成者と承認者のフィールド

* Workfront PlanningのGenStudio レコードタイプに対して、「作成者」フィールドと「承認者」フィールドをWorkfront Planningから追加できます。
* チャネルおよび地域レコードタイプに表示されるレコードには、ユーザーが作成した「システム」が表示されます。 これらのレコードは、GenStudio ワークスペースをWorkfront Planningで作成するときに自動的に作成されます。
* ワークスペースがWorkfront Planningで使用できるようになった後にGenStudioで作成されたレコードは、ユーザーがGenStudioでレコードを作成し、Workfront ユーザーではない場合でも、「作成者」フィールドにレコードを作成したIMS ユーザーの名前が表示されます。
* 「承認者」フィールドには、Workfront PlanningのGenStudio レコードタイプでレコードを作成するためにリクエストフォームが送信されたときに、承認者の名前が表示されます。
* 作成者フィールドと承認者フィールドは、GenStudio for Performance Marketingのレコードの詳細に表示されます。 リストビューには表示されません。

### GenStudio ワークスペースでのビューの記録

>[!NOTE]
>
>GenStudio レコードタイプは、GenStudio for Performance Marketing リストビューから読み込まれたデフォルトのテーブルビューに表示されます。
>
>GenStudio for Performance Marketingからデフォルトで読み込まれた元のテーブルビューは削除できません。

* GenStudio for Performance Marketingでは複数のビューを作成することはできません。

* PlanningのGenStudio Workspaceに対する管理権限がある場合は、Workfront Planningから次の操作を実行できます。

   * GenStudio レコードタイプのビューを作成します。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * GenStudioのレコードタイプからカスタムビューの名前を変更、共有、書き出し、複製または削除します。

* PlanningのGenStudio Workspaceに対するContribute権限がある場合は、Workfront Planningから次の操作を実行できます。

   * GenStudio レコードタイプのビューを作成します。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * GenStudioのレコードタイプからカスタムビューの名前を変更、書き出し、複製または削除します。

     Workfront PlanningのGenStudio ワークスペースからビューを共有することはできません

### GenStudio ワークスペースのレコード接続

GenStudio ワークスペースに対する管理権限がある場合、レコードタイプ間の接続を作成できます。

Workfront Planningでは、GenStudioのレコードタイプと、その他のレコードタイプまたはオブジェクトタイプとの間に次のつながりを作成できます。

* 2種類のGenStudio レコードタイプ
* 同じワークスペースのGenStudio レコードタイプとプランニングレコードタイプ
* 別のワークスペースから接続するようにレコードタイプが設定されている場合は、GenStudio レコードタイプと別のワークスペースのプランニングレコードタイプ。
* GenStudio レコードタイプとWorkfront オブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム、企業、グループ）。
* GenStudio レコードタイプとAEM オブジェクトタイプ（Assetsまたはコンテンツフラグメント）。 Adobe Experience ManagerがAEM オブジェクトにアクセスするには、Workfront PlanningのライセンスとAdobe GenStudio for Performance Marketingのライセンスに加えて、ライセンスが必要です。
* GenStudioレコードタイプとGenStudio Brands。 ブランド接続は、デフォルトで製品およびペルソナのレコードタイプに追加されます。

### GenStudio Workspace レコードとAEM オブジェクト間のメタデータの同期

AEM オブジェクトタイプ（アセットおよびコンテンツフラグメント）がGenStudio ワークスペースからGenStudio レコードタイプに接続されている場合、次の情報はGenStudio レコードとAEM オブジェクト間で同期されます。

* AEM アセットとコンテンツフラグメントの情報は、レコードタイプが接続されたときに追加されたルックアップフィールドのGenStudio ワークスペースに表示されます。
* GenStudio レコード情報は、「Campaign」タブのAEM アセットまたは「メタデータ」タブのコンテンツフラグメントにAEM レコード情報が表示されます。

  詳しくは、[Adobe Workfront PlanningでのGenStudio Workspaceの管理](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)を参照してください。

### GenStudio レコードタイプのリクエストフォームと自動化

* Workfront PlanningのGenStudio レコードタイプにリクエストフォームを追加できます。 GenStudio Workspace レコードタイプに関連付けられたリクエストフォームに、Planning接続フィールドを追加できます。

  詳しくは、[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)でのリクエストフォームの作成と管理を参照してください。
* Workfront Planningでは、GenStudio レコードタイプの自動処理を設定できます。

  詳しくは、[Adobe Workfront Planningの自動処理の設定](/help/quicksilver/planning/records/configure-automations-to-create-records.md)を参照してください。

### Workfront Planning ワークスペースからGenStudioブランドへの接続

Workfront PlanningとAdobe GenStudioの間に統合がある場合、Workfront Planningの任意のワークスペースの任意のレコードタイプからGenStudio BrandsにPlanning レコードタイプを接続できます。

次の点に注意してください。

* ブランドは、デフォルトで次のGenStudio Workspace レコードタイプに接続されます。

   * 製品
   * ペルソナ

* ブランドは、他のすべてのGenStudio Workspace レコードタイプ、または管理権限を持つすべての他のワークスペースのレコードタイプに手動で接続できます。

* ブランドをPlanningまたはGenStudio レコードタイプに接続した後、レコードタイプに関連付けられたリクエストフォームにブランド接続フィールドを追加できます。

## プレビュー環境

* 実稼動環境からアクセス可能なGenStudio ワークスペースも、同じWorkfront インスタンスのプレビュー環境に表示されます。
* この記事で説明するすべてのアクティビティは、Workfront PlanningのGenStudio Workspaceでプレビュー環境で実行できますが、これらの変更はGenStudioからは表示されません。

  実稼動環境の項目に加えた変更のみが、Workfront PlanningとGenStudio間で同期されます。

  GenStudioにはプレビュー環境がありません。

