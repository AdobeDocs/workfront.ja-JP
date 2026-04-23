---
title: ワークスペースの作成
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。レコードタイプは、ワークスペースのセクション別に整理されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 19%

---


# ワークスペースを作成

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

ワークスペースの一般的な情報については、[&#x200B; ワークスペースの概要](/help/quicksilver/planning/architecture/workspaces-overview.md)を参照してください。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

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
<p>任意のWorkfrontまたはWorkflow パッケージ</p> 
<p>任意のWorkfront計画パッケージ</p>
<p>一度に複数のワークスペースを作成するWorkfront Planning Prime以降のパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   <p>システム管理者は、ベストプラクティスのテンプレートバンドルを使用して、一度に複数のワークスペースを作成できます</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## ワークスペースの作成

ワークスペースを作成し、それにレコードタイプを追加して、Workfront Planningでオブジェクトを整理できます。

ワークスペースの編集について詳しくは、[&#x200B; ワークスペースの編集](/help/quicksilver/planning/architecture/edit-workspaces.md)を参照してください。

ワークスペースは、次の方法で作成できます。

* ゼロから、またはテンプレートから1つのワークスペースを作成する

  詳しくは、この記事の「[&#x200B; ゼロから、またはテンプレートからワークスペースを作成する](#create-a-workspace-from-scratch-or-from-a-template)」の節を参照してください。
* AIを活用したPlanning Designerを使用して、ひとつのワークスペースを作成できます。 この機能は現在、Beta プログラムの一部のお客様のみが利用できます。

  詳しくは、「[Adobe Workfront計画Designerの基本を学ぶ](/help/quicksilver/planning/general/planning-ai-designer.md)」を参照してください。

* ベストプラクティスのマルチワークスペーステンプレートバンドルを使用して複数のワークスペースを作成する

  詳しくは、この記事の「[&#x200B; ベストプラクティスのマルチワークスペーステンプレートバンドルを使用した複数のワークスペースの作成](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle)」の節を参照してください

  >[!TIP]
  >
  >複数のワークスペースを一度に作成できるのは、ベストプラクティスのテンプレートバンドルを使用している場合のみです。

### ゼロから、またはテンプレートからワークスペースを作成する

{{step1-to-planning}}

1. 「**ワークスペースを作成**」をクリックします

   「ワークスペースを作成」ボックスが表示されます。 ワークスペースをゼロから作成することも、使用可能なテンプレートを使用して作成することもできます。

1. （オプションおよび条件付き）次の事前定義済みのワークスペーステンプレートのいずれかで「**プレビュー**」をクリックします。

   * ベーシック：マーケティング管理
   * アドバンスト：マーケティング管理
   * エンタープライズ：マーケティング管理
   * セールス管理
   * 製品管理

   テンプレートプレビューボックスが開きます。

   運用中のレコードタイプ、分類および各テンプレートに関連付けられているフィールドの数が示されます。

   ![&#x200B; ワークスペース テンプレートのプレビュー](assets/previewing-a-workspace-template.png)

   Workfront Planning ワークスペーステンプレートについて詳しくは、[ワークスペーステンプレートのリスト](/help/quicksilver/planning/architecture/workspace-templates.md)を参照してください。

1. テンプレートのプレビューボックスで、「**テンプレートを使用**」をクリックして、選択したテンプレートからワークスペースの作成を開始します

   または

   **戻る**&#x200B;をクリックしてから、**新しいワークスペース**&#x200B;をクリックして、ワークスペースをゼロから作成します。

   次のタイプのワークスペースの 1 つが作成されます。

   * **名称未設定のWorkspace**&#x200B;という名前の空のワークスペース。このワークスペースをゼロから作成すると、レコードタイプを手動で追加できます。
   * 選択したテンプレートにちなんで名前が付けられたワークスペース。サンプルレコードタイプが入力されます。 レコードタイプとワークスペースをさらにカスタマイズできます。

   Workfront管理者の場合、新しいワークスペースは「**自分が所属するワークスペース**」タブに表示されます。

   ワークスペースを作成できる他のすべてのユーザーの場合、新しいワークスペースが&#x200B;**ワークスペース**&#x200B;領域に表示されます。

1. 新しいワークスペースのヘッダーにあるワークスペースの名前をクリックして名前を変更し、Enter キーを押します。

1. （オプションおよび条件付き）ワークスペースをテンプレートから作成した場合は、「**運用中のレコードタイプ**」または「**分類**」セクションの名前内をクリックします。

   または

   セクションの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**名前変更**&#x200B;をクリックしてセクションの名前を変更します。

   >[!TIP]
   >
   >セクションを作成しなかった場合でも、任意のワークスペースから任意のセクションの名前を変更できます。

   ワークスペースのセクションの編集など、ワークスペースの編集について詳しくは、[&#x200B; ワークスペースの編集](/help/quicksilver/planning/architecture/edit-workspaces.md)を参照してください。

1. （オプション）「**レコードタイプを追加**」をクリックして、任意のセクションのワークスペースにレコードタイプを追加します。

   詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   ワークスペースでのレコードタイプの編集と削除について詳しくは、[&#x200B; ワークスペースの編集](/help/quicksilver/planning/architecture/edit-workspaces.md)を参照してください。

1. （オプション）新しいワークスペースの左側にある戻る矢印をクリックして、プランニングのメインページを開きます。 新しいワークスペース用に新しいワークスペースカードが&#x200B;**自分が所属するワークスペース** タブに作成されます。

   ワークスペースを作成したユーザーの名前は、所有者としてワークスペースカードに保存されます。

   >[!TIP]
   >
   >Workfrontのみのユーザーが作成したワークスペースのうち、**System**&#x200B;が作成したようにAdobe Admin Consoleの表示に追加されていないユーザーが作成したものです。
   >

### ベストプラクティスのマルチワークスペーステンプレートバンドルを使用して複数のワークスペースを作成する

>[!IMPORTANT]
>
>ベストプラクティスのテンプレートバンドルを使用して複数のワークスペースを一度に作成できるのは、次の前提条件が満たされている場合のみです。
>
>* Workfront計画PrimeまたはUltimate パッケージを購入しました。
>* システム管理者です

マルチワークスペーステンプレートバンドルを使用して、ワンクリックで6つのワークスペースを作成できます。

バンドルに含まれるテンプレートには、プランニングの実装を開始するのに役立つワークスペース、レコードタイプ、レコード、ビュー、フィールドが含まれています。

>[!IMPORTANT]
>
>バンドルに含まれるワークスペースとレコードの名前は例であり、独自の環境を反映するものではありません。
>
>レコードタイプとフィールドの名前は、推奨事項に従って、任意の業界での実装の標準として、任意の組織で使用できます。
>

{{step1-to-planning}}

1. 「**ワークスペースを作成**」をクリックします

   「ワークスペースを作成」ボックスが表示されます。 ワークスペースをゼロから作成することも、使用可能なテンプレートを使用して作成することもできます。

1. **ここから開始（推奨）**&#x200B;領域の&#x200B;**ワークスペース設定を確認**&#x200B;をクリックします。
1. （オプション）次の定義済みワークスペーステンプレート内の&#x200B;**プレビュー**&#x200B;をクリックして、各テンプレートのプレビューボックスを開きます。

   * &#x200B;1. グローバル分類と分類

     Global Classifications &amp; Taxonomies テンプレートには、Workfront Planningの導入を成功させるために、環境で作成することをお勧めするすべてのレコードタイプとフィールドが含まれています。

     後で、作成した他のワークスペースでこのテンプレートのレコードタイプをリンクまたはインポートできます。
   * 2.Fréscopa グローバルマーケティング
   * 3.Fréscopa ソーシャルマーケティング
   * &#x200B;4. フレスコパ・メディア&amp;PR
   * &#x200B;5. フレスコパ・グローバル・イベント
   * 6.Fréscopa経営陣

1. 各ワークスペーステンプレートの「**プレビュー**」ボックスを開いた後、「戻る」をクリックして「**ワークスペースを作成」ボックスに戻るか、「テンプレートを使用」をクリックして、バンドルを含むテンプレートを使用し、ワークスペースを作成します。**

   ワークスペースが作成され、システム管理者用の&#x200B;**ワークスペースに表示されます。自分は**&#x200B;です。**すべてのワークスペース** タブに表示されます。 すべての標準ライセンスのユーザーは、システム管理者がワークスペースを作成し、新しいワークスペースを共有すると、ワークスペース領域にワークスペースが表示されます。

1. 作成したワークスペースの編集を開始し、組織に関連するレコードタイプ、レコード、ビュー、フィールドを追加します。

   Workfrontを実装するためのベストプラクティスについて詳しくは、[Adobe Workfront計画のベストプラクティス：記事インデックス &#x200B;](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md)の節の記事を参照してください。

   ワークスペースの編集について詳しくは、[&#x200B; ワークスペースの編集](/help/quicksilver/planning/architecture/edit-workspaces.md)を参照してください。



