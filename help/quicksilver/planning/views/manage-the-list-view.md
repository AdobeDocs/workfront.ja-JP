---
title: Adobe Workfront Planningでのリスト表示の管理
description: Adobe Workfront Planningのレコードの接続レコードページでオブジェクトにアクセスする場合、オブジェクトとそのフィールドをリストビューに表示できます。 この記事では、レコードの接続されたレコードページでリストビューを作成または編集する方法について説明します。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '1857'
ht-degree: 2%

---


# Adobe Workfront Planningでのリストビューの管理

<!--
although list views in Planning are very similar to Workfront enhanced lists, keep this one separate with all the information, because of Planning standalone; some information here is also duplicated in this main Glist article: help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md
-->

<span class="preview">このページで強調表示されている情報は、まだ一般公開されていない機能を指しています。 すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Workfront Planningの次の領域では、リストビューでオブジェクトを表示できます。

* レコードの詳細領域にあるプロジェクトの接続されたレコードページ

  ![&#x200B; リスト表示の接続されたレコード ページ上のプロジェクト &#x200B;](assets/projects-on-connected-records-page-list-view.png)

* レコードタイプレベルでのリクエストフォームのリスト

  ![&#x200B; リストビューのリクエストフォーム &#x200B;](assets/request-forms-in-list-view.png)

ここでは、Workfront Planningでリスト表示を操作、作成または編集する方法について説明します。

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
<p>任意のWorkfrontおよびプランニングパッケージ</p>
<p>任意のワークフローとプランニングパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p> ビューの作成と削除を行う標準</p>
   <p>ビュー要素を更新する貢献者以上</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ビューに対する権限を管理</p>  
   <p>ビューの権限を表示して、ビュー設定を一時的に変更したり、ビュー設定を複製したりできます</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> LightまたはContributor ライセンスを持つユーザーには、Planningを含むレイアウトテンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトでプランニング領域を有効にできます。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++ 

## リストビューに関する考慮事項

* 接続されたレコードのページリストビューについては、次を考慮してください。

   * プロジェクトは、レコードの接続されたレコードページのリストビューでのみ表示できます。 リスト表示は、接続されたレコードページ内の他のオブジェクトまたはレコードタイプでは使用できません。

  接続レコードページの作成について詳しくは、[接続レコードページをレコードに追加](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)を参照してください。
   * レコードの接続されたレコードページでリストビューを表示する前に、Workfront プロジェクトをプランニングレコードタイプに接続する必要があります。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   * レコードの接続されたレコードページで、プロジェクトの複数のリストビューを作成できます。

* リクエストフォームのリストビューでは、次の点を考慮してください。

   * Planning リクエストフォームの追加リストビューを作成または編集することはできません。 Workfrontは、リクエストフォームに対して1つのリストビューを作成します。<!--this will change-->

     リクエストフォームについて詳しくは、[Adobe Workfront Planningでのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)を参照してください。
* 表示される場所に応じて、すべてのリストビューがこの記事に記載されているすべての要素を持っているわけではありません。

## リスト表示の管理 {#manage-a-list-view}

Workfront計画のリストビューは、Workfrontの拡張リストと似ています。 拡張ビューからのほとんどの要素は、Workfront Planningのリストビューにも存在します。

詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。

<!--
Removed - more direct steps below: 
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. 次のいずれかの領域でリスト表示に移動します。

   * レコードの詳細領域にあるプロジェクトの接続されたレコードページ
   * レコードタイプのリクエストフォームページ

1. （条件付き）使用可能な場合は、次のいずれかの操作を行ってリスト表示を変更します。

   1. リストの左上隅にあるドロップダウンビューメニューを展開して別のビューを選択するか、**新しいビュー**&#x200B;をクリックして別のビューを作成します。

      >[!TIP]
      >
      >ビューはシステム全体で共有されます。 1つのレコードタイプのプロジェクトビューを作成すると、接続されたプロジェクトを表示する他のレコードタイプで表示できます。

   1. 既存のビューの名前にカーソルを合わせて、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、次のいずれかをクリックします。
      * **名前を変更**&#x200B;して、ビューに新しい名前を付けます
      * **共有**、他のユーザーとビューを共有する
      * **削除**、ビューを削除します。

      >[!NOTE]
      >
      >* ビューを編集、共有、または削除するには、ビューの管理権限が必要です。
      >
      >* システムビューは変更できません。
      >
      >* <span class="preview">自分と共有していたビューを、元の環境設定を復元するように変更した後に表示する権限のみを持つビューにリセットするか、変更内容をコピーしてコピーを共有することができます。 詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。</span>

   1. **フィルター** アイコン ![&#x200B; フィルターアイコン &#x200B;](assets/filter-icon.png)をクリックして、フィルターをビューに追加します。 結果はリスト内ですぐにフィルタリングされます。 フィルターを保存して名前を付けることはできません。 フィルターは、後でページにアクセスしたときに記憶され、共有ビューの一部になります。

      >[!TIP]
      >
      ><span class="preview"> パーソナライズされたフィルターを適用するには、フィールド値に次のいずれかのオプションを選択します。
      >
      ><div class="preview">
      >
      >* ユーザーを参照するフィールドでログイン ユーザーを参照するには、**自分（ログイン ユーザー）**。
      >
      >* **マイチーム**&#x200B;または&#x200B;**マイホームチーム**&#x200B;は、チームを参照するフィールドでチームを参照します。
      >
      >* **マイグループ**&#x200B;または&#x200B;**マイホームグループ**&#x200B;は、グループを参照するフィールドでグループを参照します。
      >
      >* **会社**&#x200B;は、会社を参照するフィールドで会社を参照します。
      > 
      >* **自分の役割**&#x200B;または&#x200B;**自分の主な役割**&#x200B;を参照して、役割を参照するフィールドで自分の担当業務を参照します。
      >
      ></div>

   1. **列** アイコン ![列アイコン &#x200B;](assets/columns-icon.png)をクリックして、表示する列または表示しない列を選択します。
   1. 列の名前にカーソルを合わせ、列名の左側にある下向き矢印をクリックしてから、次のいずれかをクリックします。
      * **列の** カスタムラベル **を追加するには、**&#x200B;の名前を変更します。 Workfrontの元のフィールド名は変更されません。
      * **並べ替え**。選択したフィールドでリストを並べ替えます。 列ヘッダーには、並べ替えの方向を示す並べ替えアイコンが追加される。
   1. リストの右上隅にある&#x200B;**+** アイコンをクリックして、リストに列を追加または削除し、**保存**&#x200B;をクリックします。

      **列マネージャー**&#x200B;が開きます。

      リスト表示に追加できるのは、既存のフィールドのみです。
最初の列に表示されるリストビューのプライマリフィールドは削除できません。

   1. <span class="preview"> 「**セルを書式設定**」アイコン ![&#x200B; セルを書式設定アイコン &#x200B;](assets/format-cells-icon.png)をクリックします。 **形式** ボックスが開きます。</span> <!--change the name of the box when they update it-->
      <span class="preview">次の操作を行います：</span>

      1. <span class="preview"> クリック **条件を追加**.</span>
      1. <span class="preview">**If**&#x200B;行で、フィールドを選択し、フィールド値を選択して修飾子を追加します。 選択したフィールドタイプによって修飾子が変更されます。</span>

         >[!TIP]
         >
         ><span class="preview">条件付き書式を設定できるのは、リスト表示に表示されるフィールドのみです。</span>

      1. <span class="preview"> （オプション）フィールド値を追加する代わりに、**別のフィールドと比較** アイコン ![別のフィールドと比較](assets/compare-to-another-field-icon.png)をクリックし、選択したフィールドの値と比較するフィールドを選択します。 例えば、「プロジェクト所有者」フィールドと「プロジェクトのスポンサー」フィールドを比較できます。</span>

         >[!TIP]
         >
         ><span class="preview">条件付き書式設定には、リスト表示に表示されるフィールドのみが使用できます。 比較するフィールドは同じタイプである必要があります。</span>

      1. <span class="preview"> （オプション） **If**&#x200B;行の&#x200B;**条件を追加**&#x200B;をクリックして、同じルールにさらに条件を追加します。</span>

         >[!TIP]
         >
         ><span class="preview">条件付きルールには最大10個の条件を追加でき、1つのフィールドには最大20個のルールを追加できます。</span>

      1. <span class="preview">条件間の&#x200B;**または** コネクタをクリックして&#x200B;**および**&#x200B;に変更し、複数の条件を同時に満たす必要があることを示します。 **または**&#x200B;が既定のコネクタです。</span>
      1. <span class="preview">**Format**&#x200B;行で、書式設定する列を示すフィールドを選択します。</span> <!--edit this area, if it changes names??-->
      1. <span class="preview"> （オプション）選択したフィールドの横にある&#x200B;**カラーサークル** アイコン ![&#x200B; カラーサークル アイコン &#x200B;](assets/color-circle.png)をクリックして展開し、**セルの塗りつぶし**&#x200B;領域で別の色を選択して、セルの背景の色を変更するか、**テキストの色**&#x200B;領域から色を選択して、セルのテキストの色を変更します。</span>
      1. <span class="preview">**テキスト形式** アイコン ![&#x200B; テキスト形式アイコン &#x200B;](assets/text-format-icon.png)をクリックし、次のオプションから選択して、セル内のテキストを書式設定します：</span>
         * <span class="preview">太字</span>
         * <span class="preview">斜体</span>

      1. <span class="preview">行に適用&#x200B;**設定を有効にして、条件を満たすフィールドの行全体に書式を適用します。**</span>
      1. <span class="preview"> （オプション）「**形式**」ボックスの&#x200B;**条件を追加**&#x200B;をクリックして、別のフィールドに別のルールを追加し、上記の手順を繰り返します。</span>
      1. <span class="preview"> （オプション）「**すべてクリア**」をクリックして、すべての書式設定を削除します。</span>
      1. <span class="preview"> 「**形式**」ボックスの外側をクリックして閉じます。</span>

         <span class="preview">これにより、リスト表示に戻ります。</span>
         <span class="preview">書式設定はリスト表示にすぐに適用されます。</span>
         <span class="preview"> 「**セルを書式設定**」アイコンの横に青い点があり、ビューに特殊な書式設定が適用されていることを示します。</span>

   1. <span class="preview"> （オプション）「**グループ化**」アイコン「![&#x200B; グループ化」アイコン「](assets/grouping-icon.png)」をクリック &lt;! – 共通フィールドでリスト内の項目をグループ化するために、これを「グループ化」??->に更新しました。 オプションのいずれかを選択するか、検索バーを使用してフィールドを検索します。</span>

      <span class="preview"> フィールドをグループ化するには、リストの列である必要があります。 すべてのフィールドタイプをグループ化に使用できるわけではありません。</span>

   1. <span class="preview">行の縦の長さを更新するには、**行の高さ** アイコン ![行の高さアイコン &#x200B;](assets/row-height-icon.png)をクリックします。 次のオプションから選択してください：</span>

      <div class="preview">

      * 低い
      * 標準： これはデフォルトの選択肢です。
      * 中
      * 高い

      </div>

   <!--leave these here, although they duplicate for Enhanced lists in Workfront-->

1. （オプション）リストの右上隅にある検索ボックスにキーワードを追加して、項目を検索します。

   検索語に一致する項目がリストで強調表示されます。

1. （オプションおよび条件付き）接続されたプロジェクト <!--change projects to items here when more items will display in the Glist-->のページで、リストにさらに項目を追加し、選択したレコードに自動的に接続するには、次のいずれかの操作を行います。

   * リストの右上隅にある「**レコードを接続**」をクリックして、既存の項目を追加します。
   * リストの下部にある&#x200B;**新しい行**&#x200B;をクリックして、新しい項目を追加します。
1. リスト内の接続されたアイテムの名前をクリックして、別のブラウザータブで開きます。
1. リスト内のセル内をダブルクリックしてフィールドの情報を編集し、Enter キーを押して変更を保存します。

   一部のフィールドは読み取り専用です。 例えば、プロジェクトの完了率は、システムによって計算されたフィールドであり、手動で編集することはできません。

1. リスト内の項目の名前にカーソルを合わせ、**詳細** メニュー[詳細メニュー](assets/more-menu.png)をクリックし、**表示**&#x200B;をクリックして、別のタブでプロジェクトを開きます

   または

   1つ以上の項目を選択し、リストの下部にあるアクションバーに注目してから、次のいずれかをクリックします（使用可能な場合）。 リスト表示にアクセスする領域に応じて、次のいずれかのオプションをクリックします。

   * 項目を削除するには、**削除**&#x200B;してください。 プロジェクトを削除すると、レコードからそのレコードが切断され、Workfrontのごみ箱に移動されます。 Workfront管理者は、削除されたプロジェクトを削除してから最大30日後に復元できます。 フォームを削除しても、フォームの送信時に作成されたリクエストやレコードは削除されません。
   * **切断**&#x200B;して、プロジェクトをレコードから切断します。 プロジェクトを切断すると、そのプロジェクトとそのルックアップフィールドのすべての値が現在のレコードから削除されます。

     <!--update screen shot at preview release-->

     ![接続されたレコード ページ リスト ビューのアクション バー](assets/actions-bar-connected-records-page-list-view.png)

   * **フォームを編集**：計画依頼フォームを開き、それを編集できます。
   * **非公開**: リクエストフォームを非公開にします。 これにより、リクエスト領域からフォームが削除され、ユーザーはこのレコードタイプにリクエストを追加できなくなります。
   * **共有**：他のユーザーと共有できるリクエストフォームの共有ボックスを開きます。
   * **リンクをコピー**: リンクをPlanning リクエストフォームにコピーして、他のユーザーと共有できるようにします。 フォームが公開されている場合は、Workfront Planning以外のユーザーとリンクを共有できます。

     ![計画要求リストのアクション バー](assets/actions-bar-in-inake-forms-list.png)



