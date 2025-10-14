---
title: レコードタイプに対するクロスワークスペース機能の設定
description: レコードタイプは、Adobe Workfront Planning で別のワークスペースに追加したり、別のワークスペースから接続したりできます。
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 6%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTICLE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->


<!--this article is linked to the UI - do not delete or change the URL-->

<!--THIS MIGHT ALREADY BE ADDED TO THE "OVERVIEW" ARTICLE, BUT CHECK: add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type.

-->

# レコードタイプのクロスワークスペース機能の設定

{{planning-important-intro}}

<!--this is linked to the UI in the info icon when you enable a record to be either global or connectable-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

Adobe Workfront Planning の複数のワークスペースで機能するようにレコードタイプを設定できます。

レコードタイプは、次のいずれかとして指定できます。

* **グローバルレコードタイプ**：ユーザーは、グローバルレコードタイプを、管理可能な他のワークスペースに追加できます。
* **接続可能なレコードタイプ**：ユーザーは、他のワークスペースからこのレコードタイプに接続できます。

レコードタイプのワークスペース間機能を定義してから、ワークスペースマネージャーがそのレコードタイプを他のワークスペースに追加または接続できるようにする必要があります。

レコードタイプのワークスペース間機能は、レコードタイプの作成または編集時に定義します。

詳しくは、次のいずれかの記事を参照してください。

* [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)
* [レコードタイプの編集](/help/quicksilver/planning/architecture/edit-record-types.md)

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
<ul><li><p>任意のWorkfront パッケージ</p></li>
<p>And</p>
<li><p>接続可能なレコードタイプを作成する任意の Planning パッケージ</p></li>
<li><p>グローバル レコード タイプを作成するための Planning Plus パッケージ</p></li>
</ul>
または：
<ul><li><p>ワークフローのPrimeまたはUltimate パッケージ</p> </li>
And
<li><p>Planning PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプに対する権限の管理 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

## グローバルレコードタイプの設定

<!--this is a UI term; don't change the title of this section-->

ワークスペースマネージャーは、レコードタイプをグローバルレコードタイプに設定できます。 グローバルレコードタイプは、他のワークスペースに追加できます。

ワークスペースマネージャーは、管理対象のワークスペースにグローバルレコードタイプを追加できます。 レコードタイプの元のフィールドもセカンダリワークスペースに追加されます。

ユーザーは、投稿権限があり、グローバルレコードタイプが追加される任意のワークスペース（元のワークスペースを含む）からグローバルレコードタイプにレコードを追加できます。 表示権限のみを持つワークスペースのレコードを表示できます。

詳しくは、[&#x200B; ワークスペース間のレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) を参照してください。

レコードタイプをグローバルとして設定するには：

{{step1-to-planning}}

1. グローバルとして設定するレコードタイプのワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックします

     ![&#x200B; レコードタイプカードのその他のメニューオプション &#x200B;](assets/more-menu-options-from-record-type-card.png)

   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **その他** メニュー ![&#x200B; その他 &#x200B;](assets/more-menu.png) をクリックします。
1. **編集** または **設定** をクリックします。

   >[!TIP]
   >
   >レコードタイプが別のワークスペースに追加されると、そのワークスペースではグローバルレコードタイプとして表示されます。 この場合、編集オプションと設定オプションはグレー表示になります。

1. （条件付き） **編集** をクリックした場合、「レコードタイプを編集 **ボックスで** 「**クロスワークスペース設定**」タブをクリックします

   または、「**設定**」をクリックした場合は、左パネルの「**クロスワークスペース設定**」セクションをクリックします。
1. 「**このレコードタイプを他のワークスペースに追加することを許可**」設定を有効にします。

   ![&#x200B; 「他のワークスペースに追加」が有効になっているレコードタイプのクロスワークスペース設定を編集 &#x200B;](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >グローバルレコードタイプを別のワークスペースに追加すると、この設定は無効になりません。

1. 「**管理対象のワークスペースにこのレコードタイプを追加できるユーザーを選択**」フィールドで、管理対象のワークスペースにこのレコードタイプを追加できるようにするエンティティを追加します。

   あなたの名前が自動的にフィールドに追加されます。

   管理するワークスペースにこのレコードタイプを追加できるようにするユーザー、グループ、チーム、担当業務または会社を個別に追加できます。

   レコードタイプを保存した後で、このフィールドを編集できます。

1. （オプション）「**管理するワークスペースにこのレコードタイプを追加できるユーザーを選択**」フィールドから名前を削除します。

   >[!TIP]
   >
   >この設定を有効にするには、少なくとも 1 つのエンティティ （ユーザー、チーム、グループ、役割、または会社）を指定する必要があります。

1. （条件付き） **レコードタイプを編集** ボックスの **保存** をクリックするか、ページヘッダーの **設定** の左側にある戻る矢印をクリックして変更を保存します。

   次のことが発生します。

   * これで、指定したユーザーがレコードタイプとそのフィールドを別のワークスペースに追加できるようになりました。

   >[!NOTE]
   >
   >レコードタイプの外観と設定および元のフィールドは、元のワークスペースからのみ編集できます。

   * レコードタイプカードに **グローバルレコードタイプ** アイコン ![&#x200B; グローバルレコードタイプアイコン &#x200B;](assets/global-icon.png) が表示され、レコードタイプを他のワークスペースに追加できることを示します。
   * システム生成の **Workspace** フィールドが、レコードタイプとそのレコードの詳細のテーブルビューに追加されます。

     「Workspace」フィールドには、各レコードの作成元のワークスペースが表示されます。

     このフィールドは読み取り専用で、削除できません。
1. （オプション）別のワークスペースに移動し、既存のレコードタイプを使用してレコードタイプを作成します。 上記の手順で有効にしたレコードタイプを選択します。

   詳しくは、[&#x200B; 別のワークスペースから既存のレコードタイプを追加する &#x200B;](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md) を参照してください。

   セカンダリワークスペースのグローバルレコードタイプから追加されたレコードタイプには、**グローバルレコードタイプ** アイコン ![&#x200B; グローバルレコードタイプアイコン &#x200B;](assets/global-icon.png) も表示されます。
1. （オプション）グローバルレコードタイプを作成した元のワークスペースに戻り、<!--ensure this stays accurate--> の手順 1～4 に従ってレコードタイプを編集します
1. （オプション）グローバルレコードが追加されたワークスペースのリストを確認します。**このレコードタイプが使用されるワークスペース** セクション。

   ![&#x200B; このレコードタイプが使用されるワークスペース &#x200B;](assets/workspaces-where-this-record-type-is-used.png)


## 接続可能なレコードタイプの設定

<!--this is a UI term; don't change the title of this section-->

レコードタイプの作成または編集時に、他のワークスペースから接続するレコードタイプを設定できます。

レコードタイプを接続可能として設定するには、次の手順に従います。

{{step1-to-planning}}

1. 接続可能として設定するレコードタイプのワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックします

     ![&#x200B; レコードタイプカードのその他のメニューオプション &#x200B;](assets/more-menu-options-from-record-type-card.png)

   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **その他** メニュー ![&#x200B; その他 &#x200B;](assets/more-menu.png) をクリックします。
1. **編集** または **設定** をクリックします。

1. （条件付き） **編集** をクリックした場合、「レコードタイプを編集 **ボックスで** 「**クロスワークスペース設定**」タブをクリックします

   または、「**設定**」をクリックした場合は、左パネルの「**クロスワークスペース設定**」セクションをクリックします。

1. **他のワークスペースでこのレコードタイプへの接続を許可** 設定を有効にします。<!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   <!-- add new screen shot with new tab name-->

   ![&#x200B; 他のワークスペースからの接続が有効になっているレコードタイプの「クロスワークスペース設定」タブを編集 &#x200B;](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   有効にすると、レコードタイプにアクセスでき、他のワークスペースから接続できるようになります。

1. レコードタイプにアクセスできるワークスペースを選択します。 次のオプションから選択します。

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **すべてのワークスペース**：ユーザーは、管理権限を持つすべてのワークスペースからこのレコードタイプに接続できます。
   * **特定のワークスペース**：ドロップダウンメニューから、ワークスペースマネージャーがこのレコードタイプに接続できるワークスペースの名前を追加します。
1. （条件付き） **レコードタイプを編集** ボックスの **保存** をクリックするか、ページヘッダーの **設定** の左側にある戻る矢印をクリックして変更を保存します。

   次のことが発生します。

   * レコードタイプとそのフィールドは、指定したワークスペースから接続できるようになりました。
   * レコードタイプカードに、接続可能なレコードタイプアイコン ![&#x200B; 接続可能なレコードタイプアイコン &#x200B;](assets/connect-from-other-workspaces-icon.png) が表示されます。これは、レコードタイプが、設定で指定した任意のワークスペースから接続できることを示します。

1. （オプション）別のワークスペースに移動し、上記の手順でワークスペース間接続を有効にしたレコードタイプに接続を追加します。

   詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。









