---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Portfolioへのプロジェクトの追加
description: プロジェクトの開始時に、プロジェクトをポートフォリオに追加することをお勧めします。 ただし、プロジェクトの全期間中いつでもポートフォリオに追加できます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UkUQdW12tLqRjh5zmbwtjNfRxFwc-Uhj2gGwjmDyKb8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c6b02fbaf2ee03728543c9d34068e4dd353ac441
workflow-type: tm+mt
source-wordcount: 689
ht-degree: 40%

---

# ポートフォリオへのプロジェクトの追加

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

プロジェクトの開始時に、プロジェクトをポートフォリオに追加することをお勧めします。 ただし、プロジェクトの全期間中いつでもポートフォリオに追加できます。

ポートフォリオにプロジェクトを追加する際は、次の点を考慮してください。

* 1つのプロジェクトに関連付けることができるポートフォリオは1つだけです。
* プロジェクトは、削除されるか、別のポートフォリオに関連付けられるまで、ポートフォリオ内に残ります。
* ポートフォリオには、無制限の数のプロジェクトを含めることができます。

>[!CAUTION]
>
>多数の子オブジェクトで使用されている場合、継承された権限が正しく適用されない場合があります。
>   
>継承された権限の問題を回避するには、次をお勧めします。
>
>* 1つの親（ポートフォリオまたはプログラム）の下にある子オブジェクト（プロジェクト）の数を制限します。 1つのポートフォリオまたはプログラムにつき、10,000件を超えるプロジェクトは推奨しません。
>
>* 下位レベルのオブジェクトに権限を適用することで、継承の深さを減らします。
>
>  例えば、ポートフォリオからプログラムに、そしてプロジェクトに継承された権限に依存するのではなく、プロジェクトレベルで直接権限を適用できます。
>
>* プログラムを分割してプロジェクトの数を減らし、権限の複雑性を低減します。
>


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] パッケージ</td> 
   <td> <p>任意</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>標準</p> 
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL Edit] アクセス ポートフォリオ</p> <p>プロジェクトへの [!UICONTROL Edit] アクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオへの権限の [!UICONTROL Manage]</p> <p>プロジェクトへの [!UICONTROL Manage] 権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

* 詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## ポートフォリオへのプロジェクトの追加

1. ポートフォリオに移動し、左側のパネルで「**[!UICONTROL プロジェクト]**」をクリックします。

   ![&#x200B; プロジェクトを含むPortfolio](assets/qs-portfolio-with-projects-350x90.png)

1. 「**[!UICONTROL 新規プロジェクト]**」をクリックして、プロジェクトを追加する方法を選択します。

   >[!TIP]
   >
   >[!UICONTROL &#x200B; マイルストーン &#x200B;] ビューでプロジェクトのリストを表示する場合、プロジェクトを追加することはできません。

   次のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody>

   <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>新しいプロジェクトを追加します。 </p> <p>プロジェクトの作成について詳しくは、<a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">プロジェクトの作成</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project （レガシーストレージ） &#x200B;]</td> 
      <td> <p>新しいWorkfront ストレージプロジェクトを追加します。 </p>
      <p>このオプションは、組織がWorkfrontとAdobeの両方のクラウドドキュメントストレージを使用している場合にのみ表示されます。 Workfront インスタンスには、両方のタイプのストレージがない可能性があります。</p>
       <p>プロジェクトの作成について詳しくは、<a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">プロジェクトの作成</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project from Template]</td> 
      <td> <p>既存のテンプレートを使用して新しいプロジェクトを追加します。 </p> <p>テンプレートからプロジェクトを作成する方法について詳しくは、<a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">テンプレートを使用したプロジェクトの作成</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import [!DNL MS Project]] </td> 
      <td> <p>以前に書き出したプロジェクトを追加します。 [!DNL MS Project] お使いのコンピューターに保存しました。 </p> <p>新しいプロジェクトを [!DNL Microsoft Project] から読み込んで作成する方法について詳しくは、<a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">[!DNL Microsoft Project]</a> からのプロジェクトの読み込みを参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>プロジェクトの承認をリクエストします。</p> <p>プロジェクトのリクエストについては、<a href="../../../manage-work/projects/create-projects/request-project.md">プロジェクトのリクエスト</a>を参照してください。 </p> </td> 
     </tr> 
          <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>既に作成済みのプロジェクトを追加します。</p> </td> 
     </tr>
    </tbody> 
   </table>

   <!-- update screen shot for both kinds of storages??-->

   ![新規プロジェクトのドロップダウン &#x200B;](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. （条件付き）既存のプロジェクトを追加することを選択した場合、「**プロジェクトを追加**」ボックスが開きます。<!--check this after UI changes-->

   ![既存のプロジェクトを追加](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. 「**[!UICONTROL このポートフォリオにプロジェクトを追加]**」フィールドにプロジェクトの名前を入力し始め、リストにプロジェクトが表示されたらクリックします。 <!--check this after UI changes-->

   複数のプロジェクトを追加できます。

   >[!NOTE]
   >
   >ドキュメントに従来のWorkfrontとAdobe クラウドストレージの両方を使用する場合、次のシナリオが存在します。
   >
   >
   >* Adobe クラウドストレージプロジェクトを従来のWorkfront ストレージポートフォリオに追加し、そのポートフォリオにドキュメントが添付されていない場合、そのポートフォリオはAdobe クラウドストレージポートフォリオに変換されます。
   >* Adobe クラウドストレージプロジェクトを従来のWorkfront ストレージポートフォリオに追加し、ポートフォリオにドキュメントが添付されている場合、ポートフォリオドキュメントストレージはWorkfront ストレージに残ります。 ただし、従来のWorkfront ストレージアイコン ![従来のWorkfront ストレージアイコン &#x200B;](assets/legacy-storage-project-icon.png)はポートフォリオから削除されます。
   >* 従来のWorkfront ストレージプロジェクトをAdobe クラウドストレージポートフォリオに追加することはできません。
   >
   >詳しくは、[&#x200B; プロジェクトおよび関連オブジェクトのドキュメント管理の概要](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)を参照してください。
   >
   >すべてのWorkfront インスタンスに両方の種類のドキュメントストレージがあるわけではありません。

   <!--
    For preview/ prod release: replace all bullets (i think!!) in the Note with this:
    * You cannot add a Legacy storage project to an Adobe cloud storage portfolio, or an Adobe cloud storage project to a Legacy storage portfolio. 
    * You cannot create a project from an Adobe cloud storage template in a Legacy storage portfolio. 
    * You can create a project from a Legacy storage template in an Adobe cloud storage portfolio, but the documents and folders on the template are not added to the new project. The project receives Adobe cloud storage.
    -->

1. （オプション）プロジェクト名の右側にある&#x200B;**X** アイコンをクリックして、ポートフォリオに追加しない場合は、リストから削除します。

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. 「**[!UICONTROL プロジェクトを追加]**」をクリックします。<!--check this after UI changes-->

   選択した 1 つまたは複数のプロジェクトが、ポートフォリオに関連付けられます。
