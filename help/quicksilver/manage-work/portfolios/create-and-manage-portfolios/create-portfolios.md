---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: ポートフォリオの作成
description: Portfolioとは、同じリソース、予算、スケジュールを求めて競合するプロジェクトの集まりです。 Portfolio内のプロジェクトは、同じリソースプールを使用し、同じスコアカードに対して測定されるほど似ています。
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# ポートフォリオの作成

Portfolioとは、同じリソース、予算、スケジュールを求めて競合するプロジェクトの集まりです。 Portfolio内のプロジェクトは、同じリソースプールを使用し、同じスコアカードに対して測定されるほど似ています。

Portfolioを使用して、同じ製品ライン、部門、部門、会社、またはその他の事業単位に属するプロジェクトをグループ化できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Portfolioへの [!UICONTROL 編集 ] アクセス</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオを作成した後は、デフォルトで、そのポートフォリオに対する管理権限を持ちます</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ポートフォリオの作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **[!UICONTROL Portfolio]**.
1. クリック **[!UICONTROL 新規Portfolio]**.
1. 置換 **[!UICONTROL 無題のPortfolio]** を、ポートフォリオに使用する名前に設定します。

   名前は 255 文字までです。

1. （オプション） **[!UICONTROL Portfolio管理]** （ページ上部のヘッダー）を使用して、ポートフォリオに別のマネージャーを割り当てます。

   ![](assets/portfolio-manager-name-350x51.jpg)

   ポートフォリオの作成者として、デフォルトでポートフォリオマネージャとして割り当てられます。

1. クリック **[!UICONTROL Portfolioの詳細]** をクリックします。
1. 内 **[!UICONTROL 概要]** 領域で、次の情報を変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td> <p>固有の情報を示すPortfolioの説明を入力します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROLPortfolioマネージャー ]</td> 
      <td> <p>ポートフォリオマネージャとして指定するユーザの名前を入力し、リストに表示されたら選択します。 これは、[!UICONTROLPortfolio所有者 ] と同じです。 これは、ポートフォリオのプロジェクトで定義された作業を監視し、ビジネスケースを承認できる人です。</p> <p>重要：任意のユーザーを [!UICONTROLPortfolioマネージャー ] に指定すると、ポートフォリオ、プログラムおよびポートフォリオ内のプロジェクトに対する [!UICONTROL 管理 ] 権限が自動的に付与されます。 </p> <p>ヒント：ページ上部のヘッダーにある [!UICONTROLPortfolioマネージャー ] を更新することもできます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">グループ </td> 
      <td> <p>グループがポートフォリオを所有している場合や、そのポートフォリオを完了する責任を持つ場合は、1 つのグループの名前を追加します。 </p> <p>適切なグループを選択していることを確認するには、グループにマウスポインターを置いて [!UICONTROL information] アイコンをクリックします <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション） **[!UICONTROL カスタムフォームを追加]** ボックス [!UICONTROL Portfolioの詳細] ページを使用して、ポートフォリオ用のカスタムフォームを選択し、カスタムフィールドを更新します。

   >[!TIP]
   >
   >ポートフォリオに添付するには、ポートフォリオのカスタムフォームを作成済みである必要があります。

1. クリック **[!UICONTROL 変更を保存]**.
1. （オプション）「 **[!UICONTROL プログラム]** 左のパネルで、 **[!UICONTROL プログラムの追加]** をクリックして、ポートフォリオにプログラムを追加します。

   プログラムの作成の詳細については、 [プログラムの作成](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. （オプション）「 **[!UICONTROL プロジェクト]** 左のパネルで、 **[!UICONTROL プロジェクトを追加]** をクリックして、ポートフォリオにプロジェクトを追加します。

   プロジェクトをPortfolioに追加する方法について詳しくは、 [ポートフォリオへのプロジェクトの追加](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

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
