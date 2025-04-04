---
title: Workfront計画レコードの自動作成を使用したAdobe Workfront オブジェクトの作成
description: Adobe Workfront Planning で自動化を構成して、アクティブ化するとWorkfrontにオブジェクトを作成したり、Workfront Planning にレコードを作成したりできます。 作成したオブジェクトとレコードは、既存の Planning レコードに自動的に接続されます。 ここでは、自動化を管理する方法（オブジェクトとレコードを作成するために自動化を編集、無効化、削除、トリガーする方法など）について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 585a65c497211c84cffafeeaa5016218fd66acd2
workflow-type: tm+mt
source-wordcount: '2197'
ht-degree: 7%

---

# Adobe Workfrontの計画レコードの自動作成を使用したオブジェクトの作成

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

Adobe Workfront Planning で自動化を構成して、アクティブ化すると、Workfront内にオブジェクトを作成したり、計画レコードからトリガーされたときにWorkfront Planning 内にレコードを作成できます。 作成したオブジェクトまたはレコードは、自動処理をトリガーするレコードに自動的に接続されます。

Workfront Planning のレコードタイプのページで自動処理を設定してアクティブ化できます。 作成された接続オブジェクトは、オートメーションを実行するレコードタイプの接続フィールドに配置されます。

例えば、Workfront Planning キャンペーンを受け取り、Workfrontでプロジェクトを作成して、そのキャンペーンの進行状況を追跡する自動処理を作成できます。 プロジェクトが、キャンペーンの「接続されたプロジェクト」フィールドのWorkfront計画キャンペーンに接続されます。

接続されたレコードについて詳しくは、「[ 接続されたレコードの概要 ](/help/quicksilver/planning/records/connected-records-overview.md)」を参照してください。

Workfront Planning の自動化を使用して、次の項目を作成できます。

* 1 つ <span class="preview"> または複数 </span> のプロジェクト
* グループ
* プログラム
* ポートフォリオ
* プロジェクト
* レコード

## アクセス要件

+++ 展開してアクセス要件を表示します…

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
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
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
   <td> 標準
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>作成するオブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム）のWorkfrontでオブジェクトを作成アクセス権を使用してアクセスを編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>ワークスペースに対する権限の管理による自動化の作成 </p>
   <p>既存の自動化を使用してオブジェクトを作成するワークスペース <!--<span class="preview">and to the record type</span>--> ースに、投稿以上の権限を付与します。 </p>  
   <p>子オブジェクト（プログラムまたはプロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）に対する権限を管理します。</p>
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 自動処理を使用したオブジェクトとレコードの作成に関する考慮事項

* オートメーションによって作成されたオブジェクトまたはレコードの名前は、単一のオブジェクトを作成するときに作成したレコードの名前と同じです。

<div class="preview">

* 複数のプロジェクトを作成すると、次のパターンに従って自動的に名前が付けられます。

  `[ Name of the record ] Name of the field choice`

  詳しくは、この記事の [Workfront Planning オートメーションを使用したオブジェクトまたはレコードの作成 ](#use-a-workfront-planning-automation-to-create-an-object-or-a-record) の節を参照してください。

</div>

* 新しいオブジェクトまたはレコードは、同じフィールド内の既存のオブジェクトまたはレコードを上書きしません。 同じレコードに対して同じ自動処理を複数回トリガーすると、以前に作成したオブジェクトに加えて、元のレコードの同じ接続されたフィールドに新しいオブジェクトまたはレコードが追加されます。

<!--hide this for now; they are trying to remove this militation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

## Workfront Planning での自動処理の設定

Workfront Planning を使用してオブジェクトを作成する前に、レコードタイプの自動処理を設定する必要があります。

{{step1-to-planning}}

1. レコードの種類カードをクリックし、レコードの名前をクリックします。

   レコードタイプのページが開きます。
1. レコードタイプ名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、**自動化の管理** をクリックします。

   選択したレコードタイプで使用可能な自動化のリストが開きます。

1. 画面の右上隅にある「**新しいオートメーション**」をクリックします。 **新しい自動化** ボックスが開きます。
1. 次のフィールドを更新します。

   * **名称未設定のオートメーション** を、オートメーションボタンに表示するテキストに置き換えます。 自動処理を使用してWorkfront オブジェクトまたは計画レコードを作成する際に、このボタンをクリックします。
   * **説明**：説明を追加して、自動化の目的を特定します。
1. 「**保存**」をクリックします。
自動処理の詳細ページが開きます。

1. 自動処理の詳細ページの「**トリガー**」セクションで、次のフィールドを更新します。

   * **トリガー**：自動処理をトリガーにするアクションを選択します。 例えば、「**ボタンをクリック**」を選択します。<!--update this step with a list of all possible triggers; right now only Button click is available-->

1. 「**アクション**」セクションの次のフィールドを更新します。<!--submitted bugs for these fields - see if they need changing here-->
   * **アクション**：自動処理をトリガーするときにWorkfrontで実行するアクションを選択します。 必須フィールドです。
次のいずれかのアクションを選択します。

      * <span class="preview"> 複数のプロジェクトの作成 </span>
      * <span class="preview">1 つのプロジェクトの作成 </span>
      * プロジェクトを作成
      * レコードを作成
      * プログラムを作成
      * ポートフォリオを作成
      * グループを作成

     >[!TIP]
     >
     >自動処理を保存すると、このフィールドで選択したアクションを変更できなくなります。

1. （条件付き）選択したアクションに応じて、次のフィールドを更新します。

   * **<span class="preview">1 つの </span> プロジェクト** を作成：<!--replace to the left: Create a single project-->
      * **プロジェクトが作成される「接続」フィールド**：新しいプロジェクトが表示される「接続」フィールドです。 必須フィールドです。
      * **プロジェクトテンプレート**:Workfrontでプロジェクトの作成に使用するプロジェクトテンプレートを選択します。

   <div class="preview">

   * 複数のプロジェクトを作成します。
      * **プロジェクトが作成される「接続」フィールド**：新しいプロジェクトが表示される「接続」フィールドです。 必須フィールドです。
      * **選択肢がレコードを作成するフィールド**：選択したレコードタイプから複数選択または単一選択のフィールドを選択します。 Workfrontは、オートメーションのトリガーとなるレコードで現在選択されているフィールド選択ごとにプロジェクトを作成します。

     >[!TIP]
     >
     >プロジェクトは、オートメーションを実行するレコードの複数選択または単一選択フィールドで現在選択されているオプションに対してのみ作成され、そのフィールドで可能なすべての選択に対しては作成されません。
     >

      * **同じテンプレートを使用**：新規プロジェクトごとに同じテンプレートを使用する場合は、このオプションを選択します。 このオプションの選択を解除した場合は、フィールドの選択ごとに **プロジェクトテンプレート** を選択します。
      * **プロジェクトテンプレート**:「**同じテンプレートを使用**」オプションを選択した場合は、Workfrontがプロジェクトの作成に使用するプロジェクトテンプレートを選択します。

   </div>

   * **ポートフォリオを作成**:
      * **ポートフォリオが作成される接続されたフィールド**：新しいポートフォリオが表示される接続されたフィールドです。 必須フィールドです。
      * **新しいポートフォリオに添付するカスタムフォーム**：新しいポートフォリオに添付するカスタムフォームを選択します。 ポートフォリオのカスタム フォームを作成してから選択する必要があります。
   * **プログラムを作成**:
      * **プログラムが作成される接続フィールド**：新しいプログラムが表示される接続フィールドです。 必須フィールドです。
      * **プログラムポートフォリオ**：新しいプログラムが追加されるポートフォリオを選択します。 必須フィールドです。
      * **新しいプログラムに添付するカスタムフォーム**：新しいプログラムに添付するカスタムフォームを選択します。 選択する前に、プログラムカスタムフォームを作成する必要があります。
   * **グループを作成**:
      * **グループが作成される接続フィールド**：新しいグループが表示される接続フィールドです。 必須フィールドです。
      * **新規グループに添付するカスタムフォーム**：新しいプログラムに添付するカスタムフォームを選択します。 選択する前に、プログラムカスタムフォームを作成する必要があります。
   * **レコードを作成**:
      * **レコードタイプ**：作成するレコードタイプを選択します。

        **設定** サブセクションが表示されます。 **設定** サブセクションの次のフィールドを更新します。

         * **接続されたレコードタイプのフィールドで、現在のレコードが表示されます**：これは、現在のレコードが表示されるアクション用に選択されたレコードタイプの接続されたフィールドです。

        例えば、製品レコードを接続するキャンペーンの自動化を作成している場合、これは、自動化を使用して製品を作成した後にキャンペーンが表示される、製品レコードタイプの接続されたフィールドです。

        必須フィールドです。

        <!--submitted a change in functionality and UI text for this - revise??-->
**フィールドをマッピング** 領域で、次の情報を更新します。

         * **転送元**：オートメーションが作成されるレコードタイプからフィールドを選択して、接続されたレコードタイプのフィールドにマッピングします。
         * **転送先**：新しく作成したレコードから、自動処理を実行しているレコードの情報を取り込むフィールドを選択します。

        >[!TIP]
        >
        >* 元のレコードタイプのフィールドタイプは、新規作成したレコードタイプのフィールドタイプと一致する必要があります。
        >* どのフィールドも選択しない場合、新しいレコードの名前は **名称未設定のレコード** になります。

1. （オプションおよび条件付き）レコードの作成を選択した場合は、「**フィールドの追加** をクリックして、追加の参照フィールドをレコード間でマッピングします。
1. （条件付き）元のレコードタイプと、「**レコードタイプ**」フィールドで選択されたレコードタイプの間に接続フィールドがない場合は、「**接続されたフィールドを追加**」をクリックします。

   ![ レコードを作成するための自動化設定 ](assets/automation-setup-create-record.png)

   次の 2 つのフィールドが作成されます。

   * 「**レコードタイプ**」フィールドで指定したレコードタイプに対して、「**接続されたレコード**」という名前の新しい接続フィールドが作成されます。
   * **レコードタイプ** フィールドに示された名前と同じ名前を持つ新しい接続フィールドが、オートメーションを設定するレコードタイプに対して作成されます。

     例えば、ブランドと呼ばれる別のレコードタイプを自動的に作成するようにキャンペーンの自動処理を設定しており、「**接続フィールドを追加**」をクリックすると、次のフィールドが作成されます。

      * **Brands** レコードタイプの **接続レコード** 接続フィールドが作成されます。
      * **Brands** 接続フィールドは **Campaigns** レコードタイプ用に作成されます。

1. （オプション）元のレコードタイプと「アクション」領域で選択したWorkfront オブジェクトとの間に接続フィールドがない場合は、「**接続フィールドを追加**」をクリックします。

   ![ 複数のプロジェクトを作成するための自動化設定 ](assets/automation-setup-create-multiple-projects.png)

   以下が作成されます。

   * 自動処理を作成するレコードタイプに対して、**Connected &lt; Workfront オブジェクト名 >** という名前の新しい接続フィールドが作成されます。 例えば、プロジェクトを自動的に作成することを選択した場合、自動化を作成するレコードタイプに対して「**接続されたプロジェクト**」フィールドが作成されます。
   * 新しいレコードタイプカードが、自動処理を設定しているレコードタイプの名前で、WorkfrontのWorkfront プロジェクトの「計画」セクションに追加されます。

1. 自動処理の詳細ページの右上隅にある「**保存**」をクリックします。

   自動処理は自動処理のリストに表示され、レコードで使用できます。

## 既存の自動化の管理

{{step1-to-planning}}

1. レコードの種類カードをクリックし、レコードの名前をクリックします。

   レコードタイプのページが開きます。
1. レコードタイプ名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、**自動化の管理** をクリックします。

   選択したレコードタイプで使用可能な自動化のリストが開きます。

1. （オプション）オートメーションを編集、無効化、または削除するには、次のいずれかの操作を行います。

   1. オートメーションのリストで、保存されているオートメーションの名前にポインタを合わせ、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックします。

   1. **編集** をクリックして、次の情報を更新します。

      * オートメーション名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックしてから、**編集** をクリックしてオートメーションの名前を変更します。
      * **アクション** フィールドを除く、自動処理のすべてのフィールド。

        >[!TIP]
        >
        >自動処理に対して最初に選択したアクションを変更することはできません。


   1. レコードのテーブルビューからオートメーションを削除し、ユーザーがレコードやオブジェクトの作成にオートメーションを使用できないようにするには、「**無効**」をクリックします。

      無効な自動処理を使用して作成されたレコードは、最初に選択されたレコードに接続されたままになります。

      再び使用できるようにするには、**その他** メニュー ![ その他のメニュー ](assets/more-menu.png) を再度クリックし、**アクティブ化** をクリックします。
   1. **削除** をクリックして、自動処理を削除します。 削除されたオートメーションは復元できません。

      削除された自動処理を使用して作成されたレコードは、最初に選択されたレコードに接続されたままになります。

## Workfront Planning 自動処理を使用したオブジェクトまたはレコードの作成

1. Workfront Planning で、レコードまたはオブジェクトの自動作成と自動接続に使用するオートメーションが含まれているレコード タイプ ページを開きます。
1. テーブル表示を開きます。
1. 1 つ以上のレコードを選択します。

   テーブルの下部に青いバーが表示され、オートメーションボタンなどの追加ボタンも表示されます。
1. 画面の右下隅付近にあるオートメーションボタンをクリックします。

   ![ オートメーションボタン ](assets/automation-custom-button.png)

   次のことが発生します。

   * オートメーションでオブジェクトまたはレコードが正常に作成された場合、画面の下部に確認メッセージが表示されます。

   * 新しいオブジェクトは、オートメーションボタンの設定で示された接続フィールドに表示されます。 場合によっては、新しいオブジェクトを表示する前にページを更新する必要があります。 新しいオブジェクトは、元のレコードと同じ名前を持ちます。

   <div class="preview">

   * 複数選択または単一選択フィールドの選択に基づいて複数のプロジェクトが作成された場合、プロジェクトは次のパターンに従って自動的に名前が付けられます。

     `[ Name of the record ] Name of the field choice`

     例えば、`Summer breeze` という名前のキャンペーンが `EMEA` というフィールド選択からプロジェクトを生成した場合、プロジェクトの名前は `[ Summer breeze ] EMEA` になります。

   </div>

   * 自動処理のトリガー元となるレコードが、新しいレコードの「接続」フィールドに追加されます。

   >[!NOTE]
   >
   >オブジェクトまたはレコードが作成され、期待どおりに接続されたことを確認することをお勧めします。

1. （オプション）接続フィールドで新しいオブジェクトをクリックします。 オブジェクトページが開き、新しいオブジェクトに追加の変更を加えることができます。

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

