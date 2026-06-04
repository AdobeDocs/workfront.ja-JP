---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Portfolioの作成
description: ポートフォリオとは、同じリソース、予算およびスケジュールに対して競合するプロジェクトの集まりです。 ポートフォリオ内のプロジェクトは類似しているため、同じリソースプールを使用し、同じスコアカードに対して測定されます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/p47W1Seb-Ew-p-ogdb-ebjLAuxvY-0rdRHLMQtWCH30
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 890
ht-degree: 57%

---

# ポートフォリオを作成

<!--Audited: 08/2025-->

ポートフォリオとは、同じリソース、予算およびスケジュールに対して競合するプロジェクトの集まりです。 ポートフォリオ内のプロジェクトは類似しているため、同じリソースプールを使用し、同じスコアカードに対して測定されます。

ポートフォリオを使用して、同じ製品ライン、部門、部署、会社、またはその他のビジネスユニットに属するプロジェクトをグループ化できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] パッケージ</td> 
   <td> <p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ポートフォリオへの[!UICONTROL Edit]アクセス権</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオを作成したら、そのポートフォリオに対する管理権限があります</p>  </td> 
  </tr> 
 </tbody> 
</table>

* 詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## ポートフォリオの作成方法

Workfrontでは、次のいずれかの方法を使用してポートフォリオを作成できます。

* メインメニューのポートフォリオ領域から最初にポートフォリオを作成します。 この記事では、ポートフォリオをゼロから作成する方法について説明します。

* キックスタートを使用してポートフォリオを読み込みます。

  Workfront管理者は、キックスタートを使用してポートフォリオをインポートできます。

  Workfront でのキックスタートを使用したデータの読み込みについて詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込む](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

* 次の方法で、Workfront Planningからポートフォリオを追加します。

   * Workfront Planningのレコードタイプから連結するだけです。

  レコードに追加してポートフォリオを作成する方法について詳しくは、「[ レコードを作成](/help/quicksilver/planning/records/create-records.md)」の「レコードを接続する際にレコードを作成する」の節を参照してください。
   * Workfront計画の自動処理の使用。

  詳しくは、[Adobe Workfront Planning レコードの自動処理を使用したオブジェクトの作成](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)を参照してください。

  Workfront Planning用の新しいWorkfront ライセンスと、追加のWorkfront Planning パッケージが必要です。

  Workfront Planningへのアクセスについて詳しくは、[ アクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。


## ポートフォリオを作成

{{step1-click-main-menu}}

1. 「**[!UICONTROL ポートフォリオ]**」をクリックします。

1. （条件付き）組織が使用しているドキュメントストレージに応じて、次のいずれかをクリックします。

   * **新しいポートフォリオ**。Workfront管理者が&#x200B;**Adobe クラウドストレージ**&#x200B;または&#x200B;**レガシーWorkfront**&#x200B;のいずれかを選択し、**ユーザーがストレージプロバイダー**&#x200B;の選択を許可する設定を選択したか、選択しなかった場合。
   * **新しいポートフォリオ （レガシーストレージ）**。Workfront管理者が&#x200B;**Adobe クラウドストレージ**&#x200B;または&#x200B;**レガシーWorkfront**&#x200B;のいずれかを選択し、**ユーザーにストレージプロバイダー**&#x200B;の選択を許可する設定も選択した場合。

     このオプションは、**ユーザーがストレージ プロバイダー**&#x200B;を選択することを許可する設定がセットアップ エリアで選択されている場合にのみ表示されます。

     詳しくは、[組織でAdobe クラウドストレージを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)を参照してください。

     >[!NOTE]
     >
     >Workfront インスタンスには、両方の種類のドキュメントストレージがない可能性があります。

     ポートフォリオが作成され、そのデフォルト名は、Workfrontがドキュメントに使用するストレージに応じて、次のパターンに従います。

      * レガシーWorkfront ストレージポートフォリオの`Untitled Portfolio`。

        レガシーWorkfront ストレージポートフォリオには、名前の横に&#x200B;**レガシーWorkfront ストレージ** アイコン ![ レガシーストレージポートフォリオアイコン ](assets/legacy-storage-project-icon.png)が表示されます。

      * Adobe クラウドストレージポートフォリオの`Untitled Portfolio - < Month day, year hour.minute.second >`

        >[!IMPORTANT]
        >
        >Adobe クラウドストレージを使用するポートフォリオには、一意の名前を付ける必要があります。

     Adobe クラウドストレージポートフォリオの場合、ポートフォリオと同じ名前の新しいドキュメントフォルダーがドキュメント領域に自動的に作成されます。

1. ポートフォリオの名前を、ポートフォリオヘッダーの新しい名前に置き換えます。

   名前は 255 文字まで入力できます。

1. （オプション）ページ上部のヘッダーの&#x200B;**[!UICONTROL ポートフォリオマネージャー]**&#x200B;の下にある名前をクリックして、ポートフォリオに別のマネージャーを割り当てます。

   ![Portfolio manager name](assets/portfolio-manager-name-350x51.jpg)

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
      <td> <p>ポートフォリオマネージャーとして指定するユーザーの名前を入力し、リストに名前が表示されたらそれを選択します。 これは、[!UICONTROL Portfolio Owner]と同じです。 これは、ポートフォリオのプロジェクトで定義された作業を監視し、ビジネスケースを承認できる人です。</p> <p>重要：任意のユーザーを[!UICONTROL Portfolio Manager]に指定すると、ポートフォリオ、プログラムおよびポートフォリオ内のプロジェクトに対する[!UICONTROL Manage]権限が自動的に付与されます。 </p> <p>ヒント：ページ上部のヘッダーで[!UICONTROL Portfolio Manager]を更新することもできます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">グループ </td> 
      <td> <p>グループがポートフォリオを所有する場合、またはグループがポートフォリオの完了を担当する場合は、単一のグループの名前を追加します。 </p> <p>適切なグループを選択していることを確認するには、グループにポインタを合わせて、横に表示される[!UICONTROL information]アイコン <img src="assets/info-icon.png"> をクリックします。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
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
