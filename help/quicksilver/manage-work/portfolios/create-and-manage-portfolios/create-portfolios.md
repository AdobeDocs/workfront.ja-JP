---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: ポートフォリオを作成
description: ポートフォリオとは、同じリソース、予算およびスケジュールに対して競合するプロジェクトの集まりです。ポートフォリオ内のプロジェクトは類似しているため、同じリソースプールを使用し、同じスコアカードに対して測定されます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 78%

---

# ポートフォリオを作成

<!--Audited: 7/2024-->

ポートフォリオとは、同じリソース、予算およびスケジュールに対して競合するプロジェクトの集まりです。ポートフォリオ内のプロジェクトは類似しているため、同じリソースプールを使用し、同じスコアカードに対して測定されます。

ポートフォリオを使用して、同じ製品ライン、部門、部署、会社、またはその他のビジネスユニットに属するプロジェクトをグループ化できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>新規：[!UICONTROL Standard]</p>
   <p>現在：[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ポートフォリオへの[!UICONTROL Edit]アクセス権</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオの作成者は、デフォルトで、そのポートフォリオに対する管理権限があります。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## ポートフォリオの作成方法

Workfrontでポートフォリオを作成するには、次のいずれかの方法を使用します。

* メインメニューの「ポートフォリオ」領域から開始して、ポートフォリオを最初から作成します。 この記事では、ポートフォリオをゼロから作成する方法について説明します。

* キックスタートを使用したポートフォリオの読み込み。

  Workfrontの管理者は、キックスタートを使用してポートフォリオを読み込むことができます。

  Workfront でのキックスタートを使用したデータの読み込みについて詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込む](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

* Workfront Planning のレコードタイプからポートフォリオを接続する際に、ポートフォリオを追加します。

  Workfront Planning 用に新しいWorkfront ライセンスと追加のWorkfront Planning ライセンスが必要です。

  Workfront Planning へのアクセスについて詳しくは、[&#x200B; アクセスの概要 &#x200B;](/help/quicksilver/planning/access/access-overview.md) を参照してください。

  レコードにポートフォリオを追加してポートフォリオを作成する方法については、「レコードの作成 [&#x200B; に関する記事の「接続時にレコードを作成する」を参照し &#x200B;](/help/quicksilver/planning/records/create-records.md) ください。


## ポートフォリオを作成

{{step1-click-main-menu}}

1. 「**[!UICONTROL ポートフォリオ]**」をクリックします。
1. 「**[!UICONTROL 新規ポートフォリオ]**」をクリックします。
1. **[!UICONTROL 名称未設定のポートフォリオ]**&#x200B;を、ポートフォリオに使用する名前に変更します。

   名前は 255 文字まで入力できます。

1. （オプション）ページ上部のヘッダーの&#x200B;**[!UICONTROL ポートフォリオマネージャー]**&#x200B;の下にある名前をクリックして、ポートフォリオに別のマネージャーを割り当てます。

   ![Portfolioマネージャー名 &#x200B;](assets/portfolio-manager-name-350x51.jpg)

   ポートフォリオの作成者は、デフォルトでポートフォリオマネージャーとして割り当てられます。

1. 左側のパネルで「**[!UICONTROL ポートフォリオの詳細]**」をクリックします。
1. **[!UICONTROL 概要]**&#x200B;領域で、次の情報を変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>ポートフォリオの説明を入力して、その独自性を示します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>ポートフォリオマネージャーとして指定するユーザーの名前を入力し、リストに名前が表示されたらそれを選択します。これは、[!UICONTROL Portfolio Owner]と同じです。これは、ポートフォリオのプロジェクトで定義された作業を監視し、ビジネスケースを承認できる人です。</p> <p>重要：任意のユーザーを[!UICONTROL Portfolio Manager]に指定すると、ポートフォリオ、プログラムおよびポートフォリオ内のプロジェクトに対する[!UICONTROL Manage]権限が自動的に付与されます。 </p> <p>ヒント：ページ上部のヘッダーで[!UICONTROL Portfolio Manager]を更新することもできます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">グループ </td> 
      <td> <p>グループがポートフォリオを所有する場合、またはグループがポートフォリオの完了を担当する場合は、単一のグループの名前を追加します。 </p> <p>適切なグループを選択していることを確認するには、グループにポインタを合わせて、横に表示された[!UICONTROL information]アイコン <img src="assets/info-icon.png"> をクリックします。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）[!UICONTROL ポートフォリオの詳細]ページの右上隅にある&#x200B;**[!UICONTROL カスタムフォームを追加]**&#x200B;ボックス内をクリックして、ポートフォリオ用のカスタムフォームを選択し、カスタムフィールドを更新します。

   >[!TIP]
   >
   >カスタムフォームをポートフォリオに添付するには、ポートフォリオのカスタムフォームを作成しておく必要があります。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
1. （オプション）左パネルで「**[!UICONTROL プログラム]**」をクリックし、「**[!UICONTROL プログラム追加]**」をクリックして、ポートフォリオにプログラムを追加します。

   プログラムの作成について詳しくは、[プログラムを作成](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)を参照してください。

1. （オプション）左パネルの「**[!UICONTROL プロジェクト]**」をクリックし、「**[!UICONTROL プロジェクトの追加]**」をクリックして、ポートフォリオにプロジェクトを追加します。

   プロジェクトをポートフォリオに追加する方法について詳しくは、[ポートフォリオへのプロジェクトの追加](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
