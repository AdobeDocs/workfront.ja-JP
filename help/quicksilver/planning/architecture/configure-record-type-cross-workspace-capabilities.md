---
title: レコードタイプに対するクロスワークスペース機能の設定
description: レコードタイプは、別のワークスペースに追加することも、別のワークスペースから接続することもできます。
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 943c26efa6f6351abf885dbc5f3aa09c0b0fab05
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 13%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# レコードタイプのクロスワークスペース機能の設定

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

Adobe Workfront Planning で、別の作業領域に追加されるレコード・タイプ、または別の作業領域から接続されるレコード・タイプを指定できます。

ワークスペースマネージャーがレコードタイプのワークスペース間機能を定義する前に、最初にレコードタイプを他のワークスペースから接続するか、他のワークスペースに読み込む必要があります。

レコードタイプのワークスペース間機能は、レコードタイプの作成または編集時に定義します。

詳しくは、次のいずれかの記事を参照してください。

* [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)
* [レコードタイプの編集](/help/quicksilver/planning/architecture/edit-record-types.md)

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 他のワークスペースへのレコードタイプの追加の設定

ワークスペースマネージャーは、レコードタイプの作成または編集時に他のワークスペースに追加されるレコードタイプを設定できます。

他のワークスペースへのレコードタイプの追加を設定する場合、ワークスペースマネージャーはレコードタイプとそのすべての情報を、管理するワークスペースの 1 つに読み込むことができます。

レコードタイプの編集時に別のワークスペースへのレコードタイプの追加を設定するには、次の手順を実行します。

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックします
または
   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **その他** メニュー ![ その他 ](assets/more-menu.png) をクリックします。
1. 「**編集**」をクリックします。

   ![ レコードタイプカードのその他のメニューオプション ](assets/more-menu-options-from-record-type-card.png)

1. **レコードタイプを編集** ボックスで、「**詳細設定**」タブを選択します。
1. 「**このレコードタイプを他のワークスペースに追加することを許可**」設定を有効にします。

   ![ レコードタイプを編集「他のワークスペースに追加」を使用した詳細設定で ](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. 「**管理するワークスペースにこのレコードタイプを追加できるユーザーを選択**」フィールドで、管理するワークスペースにこのレコードタイプを追加できるようにするユーザーを追加します。

   あなたの名前が自動的にフィールドに追加されます。

   管理するワークスペースにこのレコードタイプを追加できるようにするユーザー、グループ、チーム、担当業務または会社を個別に追加できます。

   レコードタイプを保存した後で、このフィールドを編集できます。
1. （オプション）「**管理するワークスペースにこのレコードタイプを追加できるユーザーを選択**」フィールドから名前を削除します。

1. **保存**&#x200B;をクリックします。

   次のことが発生します。

   * これで、指定したユーザーがレコードタイプとそのフィールドを別のワークスペースに追加できるようになりました。

   >[!NOTE]
   >
   >レコードタイプとそのフィールドは、元のワークスペースからのみ編集できます。

   * レコードタイプカードに ![ グローバルレコードタイプアイコン ](assets/global-icon.png) グローバルレコードタイプアイコン）が表示され、レコードタイプが、設定でマネージャーを指定したワークスペースに追加できることを示します。
   * システム生成の **Workspace** フィールドがレコードタイプに追加されます。

     「Workspace」フィールドには、各レコードが作成されたワークスペースが表示されます。

     このフィールドは読み取り専用で、削除できません。

## 他のワークスペースからレコードタイプへの接続の設定

レコードタイプの作成または編集時に、他のワークスペースから接続するレコードタイプを設定できます。

レコードタイプの編集時に他のワークスペースから接続するレコードタイプを設定するには：

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックしてから、**編集** をクリックします
または
   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**編集** をクリックします。

   ![ レコードタイプカードのその他のメニューオプション ](assets/more-menu-options-from-record-type-card.png)

1. **レコードタイプを編集** ボックスで、「**詳細設定**」タブを選択します。
1. **他のワークスペースでこのレコードタイプへの接続を許可** 設定を有効にします。<!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![ 他のワークスペースからの接続が有効なレコードタイプの「詳細設定」タブを編集 ](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   有効にすると、レコードタイプにアクセスでき、他のワークスペースから接続できるようになります。

1. レコードタイプにアクセスできるワークスペースを選択します。 次のオプションから選択します。

   * **システム全体**：ユーザーは、管理権限を持つすべてのワークスペースから、このレコードタイプに接続できます。
   * **特定のワークスペース**：ワークスペースマネージャーがこのレコードタイプに接続できるワークスペースの名前を追加します。
1. 「**編集**」をクリックします。

   次のことが発生します。

   * レコードタイプとそのフィールドは、指定したワークスペースから接続できるようになりました。
   * レコードタイプカードに、ワークスペース間接続アイコン ![ ワークスペース間接続アイコン ](assets/connect-from-other-workspaces-icon.png) ワークスペース間接続アイコン）が表示され、レコードタイプが設定で指定した任意のワークスペースから接続できることを示します。

   レコードタイプは、指定したワークスペースから接続できるようになります。









