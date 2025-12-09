---
title: Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ
description: GenStudio for Performance Marketing Workspace は、会社が両方の製品を購入すると、Adobe Workfront Planning で使用できるようになります。 この統合を使用してワークフローを効率化する方法に関する基本をいくつか説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '2063'
ht-degree: 1%

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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの両方を使用している組織では、多くの場合、キャンペーン、製品、アクティベーション、ペルソナなどのマーケティング概念を、GenStudioがデフォルトでサポートしている概念よりも詳細に定義しています。

GenStudio for Performance MarketingとWorkfront Planning はネイティブで統合されています。 この統合により、Workfront Planning のユーザーはGenStudioで使用されるキャンペーン、製品、ペルソナ、アクティベーション、チャネルおよびリージョンを管理できるようになります。 また、Workfront Planning から既存のレコードタイプを参照するようにGenStudioを設定して、より接続された一貫性のあるマーケティングワークフローを作成することもできます。

GenStudio for Performance Marketing Workspace は、会社が両方の製品を購入すると、Adobe Workfront Planning で使用できるようになります。

## 統合のメリット

Workfront Planning とGenStudio for Performance Marketingの統合により、次のことができます。

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Workfront Planning でGenStudioワークスペースを表示します。
* GenStudio for Performance Marketingでキャンペーン、商品、ペルソナ、アクティベーションを変更し、Workfront Planning で同じ情報をリアルタイムに更新します。
* Workfront Planning でキャンペーン、商品、ペルソナ、およびアクティベーションを変更し、GenStudio for Performance Marketingで同じ情報をリアルタイムで更新します。
* 重複するデータ入力を避けます。
* 計画とアクティブ化の取り組み間の整合性を維持します。
* GenStudio Brands とその情報をWorkfront Planning レコードに接続します。

## 統合要件

Workfront Planning とGenStudio for Performance Marketingの統合が存在するには、次の要件を満たす必要があります。

* WorkfrontとGenStudio for Performance Marketingは、同じ組織に対して有効にする必要があります。

  GenStudioについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Workfront インスタンスは、Identity Management System （IMS）の使用など、Adobe統合エクスペリエンスの一部です。

  詳しくは、[WorkfrontのAdobe統合エクスペリエンス &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。

* Workfront Planning とGenStudio for Performance Marketingの両方を使用するユーザーは、IMS 組織内の 1 つのWorkfront インスタンスにのみ属している必要があります。

  Workfrontのみのユーザーは、GenStudio for Performance Marketing ユーザーでなくても、GenStudio Workspace を表示できます。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## アクセス要件

次の表に、Adobe GenStudio for Performance MarketingでAdobe Workfront Planning を使用するためのアクセス要件と権限要件を示します。

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
<p>任意のWorkfrontと任意の Planning パッケージ</p> <p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
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
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing ユーザーの役割</p></td> 
   <td><p><ul><li>キャンペーン、製品およびペルソナにアクセスするためのGenStudio ユーザーロール</li>
   <li>アクティベーションにアクセスするための GenSudio System Manager <!--and Events--></li></ul>
   詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> ユーザーの役割と権限 </a> を参照してください。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  
   <p>Workfrontの計画では、次の操作を行います。 </p>
   <ul>
   <li><p>GenStudio Workspace に新しいフィールドまたはレコードタイプを追加するためのGenStudio Workspace に対する権限を管理します</p></li>
   <li><p>GenStudio Workspace に対するレコードの追加、更新、削除の権限の投稿GenStudio Workspace</p> </li>  
   </ul>
   <p>Workfront Planning のGenStudio Workspace からGenStudio for Performance Marketing レコードタイプまたはフィールドを削除することはできません</p>
   <p>Adobe GenStudio for Performance Marketingで： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketingのすべての権限</p></li>
   <li><p> Adobe GenStudio for Performance Marketingでアイテムを作成する権限を作成する</p></li></ul>
   </td>  
</tbody> 
</table>

Adobe Workfront Planning へのアクセスについて詳しくは、[Adobe Workfront Planning へのアクセスの概要 &#x200B;](/help/quicksilver/planning/access/access-overview.md) を参照してください。

Adobe GenStudio for Performance Marketingについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

<!--Old:
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
</table> -->

## Workfront Planning とGenStudio for Performance Marketingの統合機能の概要

組織のWorkfront インスタンスの数に応じて、Planning のGenStudio Workspace に対して自動的に次の権限が付与されます。

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Workfrontの 1 つのインスタンス</p></td> 
   <td> 
<p>GenStudio Workspace は、Workfront Planning のインスタンスに表示されます</p>
<p>Workfront管理者を含むすべてのユーザーは、デフォルトで Planning のGenStudio Workspace への投稿アクセス権を持っています</p>
<p>Workfront管理者は、GenStudio Workspace の管理権限を変更して任意のユーザーに付与できます</p>
</td> </tr>
   <tr> 
<td> 
   <p> Workfrontの複数のインスタンス</p> </td> 
   <td> 
   <p>Workfront Planning を使用するWorkfrontのインスタンスが複数ある場合のシナリオを次に示します。</p>
   <ul><li>Adobe GenStudio for Performance Marketingの購入時に会社にWorkfrontの複数のインスタンスがある場合、GenStudio Workspace はすべてのWorkfront インスタンスから表示されます。</li>
   <li>元のインスタンスがWorkfrontと統合されてから会社がAdobe GenStudio for Performance Marketing インスタンスをさらに追加した場合、GenStudio Workspace は元のWorkfront インスタンスからのみ表示されます。 Workfrontの追加のインスタンスをAdobe GenStudioに接続する方法については、アカウント担当者にお問い合わせください。 </li></ul>    
</td> 
  </tr>
   </tbody> 
</table>

<!--Old for the second row in the table:

<p>The GenStudio workspace is visible from all Workfront instances</p>
<p>All users with access to GenStudio for Performance Marketing and Workfront Planning have Contribute permissions on the GenStudio in Planning by default</p> 
<p>Workfront administrators cannot grant Manage permissions to the GenStudio workspace to anyone</p>-->

Workfront Planning の権限については、[Adobe Workfront Planning での共有権限の概要 &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md) を参照してください。

以下の節では、以下について説明します。

* GenStudio for Performance MarketingからWorkfront Planning の情報を更新する機能
* Workfront Planning からGenStudio for Performance Marketing情報を更新する機能
* Workfront Planning のGenStudio Workspace で管理できる内容と管理できない内容に関する制限。

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront Planning のGenStudio ワークスペース

* GenStudio Workspace は、Workfront Planning にGenStudio for Performance Marketing Workspace を表すインジケーターを表示し、それを識別します。

  ![Planning のGenStudio カード &#x200B;](assets/genstudio-card-with-tag-highlighted.png)

  詳しくは、[Adobe Workfront Planning でのGenStudio Workspace の管理 &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md) を参照してください。
* Planning のGenStudioワークスペースに対する管理権限を持っている場合は、次の操作を実行できます。

   * Planning のGenStudioワークスペースを更新します（名前、説明、アイコン）
   * セクションの作成
   * レコードタイプを追加
   * 他のユーザーとの共有

     GenStudio アカウントを持たない他のユーザーとGenStudio Workspace を共有できます。 共有できるのは、組織のIdentity Management System （IMS）で使用可能なユーザーのみです。

     <!--
        >[!NOTE]
        >
        >You cannot remove GenStudio users from the GenStudio workspace or its record types' sharing. -->
     <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Planning のGenStudio作業領域に対する投稿権限がある場合、Workfront Planning から作業領域を変更することはできません。

### GenStudio Workspace のレコードタイプ

* GenStudio for Performance Marketingと Planning の両方に表示されるレコードタイプには、Workfront Planning にGenStudio インジケーターがあります。

  ![Workfront Planning のGenStudio レコードタイプカード &#x200B;](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Planning のGenStudioワークスペースに対する管理権限を持っている場合は、Workfront Planning から次の操作を実行できます。
   * GenStudio レコードタイプに関する情報（外観、詳細設定）を編集します。
   * GenStudio レコードタイプを他のユーザーと共有する。
   * レコードタイプを作成します。 これらのレコードタイプは、Workfront Planning にのみ残ります。 GenStudioには表示されません。
   * GenStudio Workspace のレコードを他のワークスペースから接続できるようにします。
   * GenStudio ワークスペースのレコードを他のワークスペースに追加できるようにします。
* Planning のGenStudioワークスペースに対する投稿権限がある場合、Planning からGenStudioレコード・タイプを変更できません。

### GenStudio Workspace のレコード

* WorkfrontからGenStudio レコードを編集すると、変更内容が、GenStudio for Performance MarketingのすべてのインスタンスのGenStudio Workspace に表示されます。
* Workfront Planning のGenStudio Workspace からアクティベーションレコードを作成または削除することはできません。
* Planning のGenStudioワークスペースに対する管理権限または投稿権限がある場合、Workfront Planning から次の操作を実行できます。
   * レコードを追加または削除すると、GenStudio for Performance Marketingで表示できるようになります（または削除されます）。

     Workfront Planning またはGenStudio for Performance Marketingから削除されたレコードは、Workfront Planning の最近削除されたレコード・ビンに 30 日間配置されます。 GenStudio for Performance Marketingには、最近削除された bin がありません。
   * 最近削除された bin からレコードを復元します。 削除したレコードを復元すると、Workfront Planning とGenStudio for Performance Marketingに戻ります。
   * 次の方法でレコードを追加します。

      * 新規レコードボタンを使用して、任意のビューからゼロから手動で
      * テーブル表示で CSV または Excel ファイルを使用してインポートする
      * 手動で、Workfront Planning の任意のビューで
      * Workfrontのレコードタイプリクエストフォームにリクエストを送信する。

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* Workfront Planning から、GenStudioワークスペース内のすべてのレコードに関するレコード情報を編集できます。

  詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

### GenStudio Workspace のレコードタイプフィールド

レコードタイプのフィールドは、デフォルトでGenStudio for Performance MarketingからWorkfront Planning に読み込まれます。

GenStudio レコードタイプフィールドについて、次の点を考慮してください。

* Planning のGenStudioワークスペースに対する管理権限を持っている場合は、Workfront Planning から次の操作を実行できます。

   * GenStudio フィールドの設定を編集します。
   * GenStudio レコードタイプのフィールドを作成します。

     Planning でGenStudioレコード・タイプのフィールドを作成すると、次の領域から表示されます：

      * Workfront計画ビュー
      * Workfront計画レコードの詳細ページ
      * GenStudio レコードの詳細ページ

     >[!TIP]
     >
     >Workfront Planning で作成されたフィールドは、GenStudioには表示されません。

   * Workfront Planning のGenStudio レコード タイプのテーブル ビューでフィールドを非表示にします。
&lt;!—* GenStudio レコードタイプのWorkfront Planning で作成されたフィールドをWorkfront Planning から削除します。 — Iskuhi によると、これは不可能です。リンクは存在しますが、エラーが発生します – >

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Planning のGenStudioワークスペースに対する投稿権限がある場合：

   * Workfront Planning のGenStudio Workspace からフィールド設定の編集、フィールドの削除または追加を行うことはできません。
   * Workfront Planning のテーブル・ビューでフィールドを非表示にできます。

#### 作成者フィールドと承認者フィールド

* Workfront Planning 内のWorkfront Planning のレコード タイプに対して、[ 作成者 ] フィールドと [ 承認者 ] フィールドをGenStudio Planning から追加できます。
* チャネルおよび地域レコードタイプに表示されるレコードには、作成者ユーザーとして「システム」と表示されます。 これらのレコードは、Workfront Planning でGenStudio Workspace を作成すると、自動的に作成されます。
* Workfront Planning でワークスペースが使用可能になった後にGenStudioで作成されたレコードには、作成者フィールドにレコードを作成した IMS ユーザーの名前が表示されます。ユーザーがWorkfront ユーザーでなくて、GenStudioでレコードを作成した場合でも同様です。
* 「承認者」フィールドには、Workfront Planning でGenStudio レコードタイプのレコードを作成するためにリクエストフォームが送信された際に、承認者の名前が表示されます。
* 「作成者」フィールドと「承認者」フィールドがGenStudio for Performance Marketingのレコードの詳細に表示されます。 これらはリスト表示には表示されません。

### GenStudio Workspace でのレコードのビュー

>[!NOTE]
>
>GenStudio レコードタイプは、GenStudio for Performance Marketing リストビューから読み込まれたデフォルトのテーブルビューに表示されます。
>
>デフォルトでGenStudio for Performance Marketingからインポートされた元のテーブルビューを削除することはできません。

* GenStudio for Performance Marketingでは、複数のビューを作成できません。

* Planning のGenStudioワークスペースに対する管理権限を持っている場合は、Workfront Planning から次の操作を実行できます。

   * GenStudio レコードタイプのビューを作成します。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * GenStudio レコードタイプからカスタムビューの名前変更、共有、エクスポート、複製、削除を行います。

* Planning のGenStudioワークスペースに対する投稿権限がある場合、Workfront Planning から次の操作を実行できます。

   * GenStudio レコードタイプのビューを作成します。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * GenStudio レコードタイプから、カスタムビューの名前変更、エクスポート、複製または削除を行います。

     Workfront Planning のGenStudio Workspace からのビューを共有することはできません

### GenStudio Workspace でのレコードの接続

管理権限を持つGenStudio Workspace で、レコードタイプ間の接続を作成できます。

Workfront Planning では、GenStudioレコード・タイプと他のレコードまたはオブジェクト・タイプを次のように関連付けることができます。

* 2 つのGenStudio レコードタイプ
* 同じワークスペースからのGenStudio レコードタイプと Planning レコードタイプ
* 別の作業領域から接続するようにレコード・タイプが構成されている場合、別の作業領域からのGenStudioレコード・タイプおよび計画レコード・タイプ。
* GenStudio レコードタイプとWorkfront オブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム、会社、グループ）
* GenStudio レコードタイプとAEM Assets オブジェクトタイプ。

### GenStudio レコードタイプのリクエストフォームと自動化

* リクエストフォームは、Workfront Planning のGenStudio レコードタイプに追加できます。

  詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。
* Workfront Planning で、GenStudio レコードタイプの自動化を設定できます。

  詳しくは、[Adobe Workfront Planning の自動設定の構成 &#x200B;](/help/quicksilver/planning/records/configure-automations-to-create-records.md) を参照してください。

### Workfront Planning Workspaces からのGenStudio Brands への接続

Workfront Planning とWorkfrontの間に統合がある場合、Adobe GenStudio Planning の任意のワークスペース内の任意のレコードタイプから Planning レコードタイプをGenStudio Brands に接続できます。

ブランドは、GenStudio Workspace ではレコードタイプのカードとして表示されません。 ブランドは、GenStudio Workspace のレコードを含む、任意のWorkfront Planning レコードタイプから新しい接続を作成するために使用できます。

<!-- when this releases, replace the paragraph above with these:

Brands are connected by default to the following GenStudio workspace record types:

    * Products
    * Personas

Brands are available for manually connecting to all other GenStudio workspace record types, or record types from all other workspaces you have permissions to manage. 

-->

## プレビュー環境

* 実稼動環境からアクセスできるGenStudio Workspace は、同じWorkfront インスタンスのプレビュー環境にも表示されます。
* プレビュー環境にあるWorkfront Planning のGenStudio Workspace で、この記事に記載されているすべてのアクティビティを実行できますが、これらの変更内容はGenStudioには表示されません。

  実稼動環境で項目に加えた変更のみが、Workfront Planning とGenStudioの間で同期されます。

  GenStudioにはプレビュー環境がありません。

