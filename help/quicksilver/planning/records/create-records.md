---
title: レコードを作成
description: Adobe Workfront Planning を使用する場合、レコードはレコードタイプのインスタンスです。 Workfront Planning で各レコード・タイプに一意のレコードを作成するには、レコードを手動でテーブル・ビューに追加するか、リストからインポートするか、複製するか、または他のレコードに接続する際に作成します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '3240'
ht-degree: 14%

---


# レコードの作成

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

次のいずれかを行うことで、レコードを作成できます。

* [任意のレコードタイプ表示の「新規レコード」または「レコードをリクエスト」ボタンを使用します](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [レコードタイプのテーブル表示からインラインで追加する](#create-records-by-adding-them-inline-from-the-record-type-table-view)
* [レコードタイプのタイムライン表示に追加](#create-records-by-adding-them-in-the-record-type-timeline-view)
* [レコードタイプのカレンダー表示に追加](#create-records-by-adding-them-in-the-record-type-calendar-view)
* [外部リストからのレコードのリストのコピー&amp;ペースト](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [テーブルビューからレコードを複製](#create-records-by-duplicating-them)
* [他のレコードから接続](#create-records-as-you-connect-them)
* [レコードタイプにリクエストフォームを送信する](#create-records-by-submitting-a-request-form-to-a-record-type)
* [CSV または Excel ファイルからの情報の読み込み](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [自動化の使用](#create-records-by-using-automations)

テーブルビューまたはタイムラインビューでのレコードの管理については、次の記事を参照してください。

* [テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)
* [タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
<p>任意のWorkfrontと任意の Planning パッケージ</p> <p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードを追加するワークスペースとレコードタイプに対する投稿以上の権限。 </p>
   <p>レコード ページの「レコードをリクエスト」ボタンを使用して、ワークスペースおよびレコードタイプに対する表示以上の権限を表示し、レコードを作成します</p>
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
   </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

<!--Old:
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
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect the records to them. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>
   <p>View or higher permissions to the workspace and record type to create records using the Request record button on the record page</p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 

</tbody> 
</table> -->

## レコードを作成する際の考慮事項

* グローバルレコードタイプに追加されたレコードは、追加したワークスペースに応じて、次のタイプのユーザーに表示されます。

   * グローバルレコードタイプの元のワークスペースに追加されたレコードは、元のワークスペースから表示できます。
   * グローバルレコードタイプのセカンダリワークスペースに追加されたレコードは、作成されたワークスペースと、グローバルレコードタイプの元のワークスペースからのみ表示されます。
詳しくは、[&#x200B; クロスワークスペースレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) を参照してください。

* ワークスペースに対する権限とレコードタイプに応じて、ユーザーは次の方法でレコードを作成できます。

   * ワークスペースおよびレコードタイプに対する表示権限を持つユーザーは、レコードタイプページの「レコードをリクエスト」ボタンを使用してのみレコードを作成できます。
   * ワークスペースおよびレコードタイプに対する投稿権限と管理権限を持つユーザーは、レコードタイプページの「新しいレコード」ボタンを使用してレコードを作成できます。

  >[!IMPORTANT]
  >
  >表示権限を持つユーザーがリクエストフォームを使用してレコードを追加するには、ワークスペースマネージャーがレコードタイプのリクエストフォームを作成する必要があります。 そうしないと、表示権限のユーザーはレコードを作成できません。


## 任意のレコードタイプ表示から「新規レコード」または「レコードをリクエスト」ボタンを使用してレコードを作成

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがビューに表示されます。

1. （条件付き）ワークスペースとレコードタイプの権限に応じて、任意の表示から、画面の右上隅にある次のいずれかをクリックします。

   * ワークスペースおよびレコードタイプに対する投稿以上の権限がある場合は、「**新しいレコード**」をクリックします

     または

   * ワークスペースとレコードタイプに対する表示権限がある場合は、「**レコードをリクエスト**」をクリックします。

1. （条件付き） **新規レコード** をクリックした場合、次の操作を行います。

   1. 次のいずれかの方法でレコードを作成し、[**続行**] をクリックします。

      * **手動で追加**。 レコードのプレビューボックスが開きます。\
        この記事の [&#x200B; レコードタイプのテーブル表示からインラインで追加してレコードを作成する &#x200B;](#create-records-by-adding-them-inline-from-the-record-type-table-view) の手順 6 から始まる節で説明しているように、レコードに関する情報を追加します。<!--insure this stays accurate-->
      * **ファイルからアップロード**
[CSV または Excel ファイルから情報をインポートしてレコードを作成する &#x200B;](/help/quicksilver/planning/records/import-file-to-create-records.md) の記事の説明に従って、手順 6 からレコードを追加します。<!--ensure this stays accurate-->
      * **リクエストの送信**
レコードタイプのリクエストフォームが開きます。

        ワークスペースマネージャーは、リクエストフォームを使用してレコードを追加できるように、リクエストフォームを作成する必要があります。

        >[!TIP]
        >
        >一部のレコードタイプには複数のフォームがある場合があります。 1 つをクリックして開きます。

        [&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの発行 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) の説明に従って、手順 6 からレコードを追加します。<!--ensure this stays accurate-->

      ![&#x200B; レコード選択モーダルを作成する 3 つの方法 &#x200B;](assets/three-ways-to-create-records-choice-modal.png)

1. （条件付き） **レコードをリクエスト** をクリックした場合、次の操作を行います。

   1. （条件付き）レコードタイプに複数のリクエストフォームがある場合は、1 つをクリックして選択します。
   2. [&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの送信 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) の説明に従って、手順 6 からレコードを作成するためのフォームに情報を追加し続けます。<!--ensure this stays accurate-->

1. （条件付き）新しいレコードを確認します。

   レコードの追加方法によっては、次の問題が発生する場合があります。

   * 承認プロセスを備えたリクエストフォームを使用して追加することを選択した場合を除き、新しいレコードがレコードタイプに追加されます。 レコードを作成する前に、すべての承認者から承認を付与する必要があります。
   * CSV または Excel スプレッドシートを使用してレコードを追加した場合、複数のレコードがレコードタイプに追加されます。
   * リクエストフォームを送信してリクエストを追加した場合、新しいリクエストが「Workfrontのリクエスト」領域に追加されます。

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## レコードタイプのテーブル表示からインラインで追加してレコードを作成

レコードタイプページのテーブル表示でレコードを作成するには、レコードをインラインで追加します。

レコード情報の編集については、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのレコードがビューに表示されます。

1. （条件付き）テーブル表示から、次のいずれかの操作を行います。

   * テーブルの最後の行、またはグループ化の最後のレコードの後にある **新規レコード** をクリックします

     >[!TIP]
     >
     >グループ化またはサブグループ化の最後のレコードの後に新しいレコードを追加すると、Workfrontはグループに含まれるフィールドを自動的に設定します。 必要に応じてこれらのフィールドを手動で編集でき、レコードがグループから削除される可能性があります。

   * テーブルの任意の列または行から、キーボードの **Shift + Enter** キーをクリックします。これにより、開始レコードの下に空の行が追加されます。
   * レコードの主フィールドにポインタを合わせ、フィールドの右側にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックし、**上にレコードを挿入** または **下にレコードを挿入** をクリックします。

   ![&#x200B; テーブルの行に新しいキャンペーンを追加 &#x200B;](assets/adding-a-new-campaign-in-table-row.png)

   Workfrontは、新しい各レコードにサムネールを自動アップロードします。 これらの画像は、後で変更できます。 詳しくは、[&#x200B; レコードへのかぶり画像を追加する &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) を参照してください。

   新しいレコードがテーブルに追加されます。

1. 新しいレコードのプライマリフィールドをクリックします

   または

   レコード名の左側にある **詳細を開く** アイコン ![&#x200B; テーブル名フィールドで詳細を開くアイコン &#x200B;](assets/open-details-icon-in-table-name-field.png) をクリックします。

   テーブルにプレビューボックスが表示されます。

1. プレビューボックスに表示されるフィールドに、新しいレコードに関する情報を入力します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクするときにレコードを識別すると便利なので、レコードの主フィールドの情報を追加することをお勧めします。 主フィールドについて詳しくは、[&#x200B; テーブル表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) および [プライマリフィールドの概要 &#x200B;](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

1. （条件付き）テーブルにレコードを追加する場合、レコードのプレビューボックスを開く前に、各行に引き続き情報を追加してから、キーボードの **Enter** をクリックして変更を保存します。

   または

   新しいレコードの名前、またはレコード名の左側にある **詳細を開く** アイコン ![&#x200B; テーブル名フィールドで詳細を開くアイコン &#x200B;](assets/open-details-icon-in-table-name-field.png) をクリックしてプレビューボックスを開き、詳細領域でレコードの情報を編集します。

   >[!TIP]
   >
   >**詳細を開く** アイコンにアクセスできるのは、レコードの名前フィールド（名前フィールドがプライマリフィールドの場合）のみです。

1. （オプション）レコードのプレビューボックスで、右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで詳細を開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを新しいタブで開きます。 レコードページでレコードの編集を続行します。 詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

   Workfront では、変更を自動的に保存します。

1. （オプション） レコードのページを開いた場合は、プレビューボックスを閉じるか、レコード名の左側にある戻る矢印をクリックします。

1. （オプション）テーブル表示で新しいレコードや情報を追加する際に、テーブル表示から次のキーボードショートカットを使用して、それらの追加の取り消しまたはやり直しを行います。

   * CTRL + Z （Macの場合は ⌘ + Z）
   * Ctrl + Shift + Z （Macの場合は ⌘ + Shift + Z）


## レコードタイプのタイムラインビューに追加してレコードを作成

レコードタイプのページのタイムライン表示で、タイムラインをダブルクリックしてレコードを作成できます。

タイムラインビューの作成について詳しくは、[&#x200B; タイムラインビューの管理 &#x200B;](/help/quicksilver/planning/views/manage-the-timeline-view.md) を参照してください。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプ ページが、最後にアクセスしたビューで開きます。

1. まず、クリックしてタイムラインビューを開くか、タイムラインビューを作成します。

   >[!NOTE]
   >
   >タイムラインビューを作成できるのは、レコードタイプに関連付けられた日付フィールドが 2 つ以上ある場合のみです。
1. タイムラインの任意の場所をダブルクリックします。

   **新規レコード** ボックスが開きます。<!--might need a new screen shot for Production - might add a title etc-->

   ![&#x200B; 名前のないレコード バーを含むタイムライン上の新規レコード ボックス &#x200B;](assets/new-record-small-box-on-timeline.png)

   >[!NOTE]
   >
   >レコードバーが名前付きグループ化で表示されている場合、タイムラインビューでレコードを作成することはできません。
1. 次の情報を更新します。


   * **名前**: レコードの名前を入力します。 空のままにすると、Workfrontはデフォルトで **名称未設定** と名前を付けます。

     >[!TIP]
     >
     >タイムライン設定に従ってレコードバーにレコードの名前を表示する場合、空のままにすると、その名前はレコードバーに表示されません。

   * **レコード日付フィールド**：レコードの日付を更新します。

     日付フィールドの名前は、タイムラインビューが作成された際に、「開始日」および「終了日」で選択されたフィールドに従ってカスタマイズされます。

     デフォルトでは、タイムラインビューの表示方法に応じて、日付値は事前に選択されています。 次のシナリオが存在します。

      * **年** 別：レコードの開始日と終了日は月に及びます。
      * **四半期** 別：レコードの開始日と終了日が 1 週間にまたがる。
      * **月** 別：レコードの開始日と終了日は 3 日間です。

1. （オプション）次のいずれかのアイコンをクリックします。

   * **展開**![&#x200B; 展開アイコン &#x200B;](assets/expand-icon.png) をクリックして、プレビューウィンドウでレコードの詳細を開きます。
   * **削除**![&#x200B; 削除アイコン &#x200B;](assets/delete-icon.png)：レコードを削除します。
   * **閉じる**![&#x200B; 閉じるアイコン &#x200B;](assets/close-icon.png) 新規レコードボックスを閉じます。

   **削除** アイコンをクリックしなかった場合、レコードは直ちにタイムラインおよびテーブルビューとカレンダービューに追加されます。

1. （オプション）タイムラインのレコードバーの余白の 1 つにポインタを合わせ、バーの端を別の日付にドラッグ&amp;ドロップします。 これにより、レコードの開始日と終了日が自動的に変更されます。

   詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

1. （オプション）タイムラインのレコードバーをクリックしてレコードの詳細ウィンドウを開き、情報を更新、削除またはコメントを追加します。

   >[!TIP]
   >
   >デフォルトでは、Workfrontはレコードをサムネールとカバー画像に関連付けます。
   >
   >サムネールは、ビューの設定で有効になっている場合にのみ、タイムラインビューに表示されます。



## レコードタイプのカレンダー表示に追加してレコードを作成

レコード タイプ ページのカレンダー表示でレコードを作成するには、カレンダー上の任意の場所をダブルクリックします。

カレンダービューの作成について詳しくは、「[&#x200B; カレンダービューの管理 &#x200B;](/help/quicksilver/planning/views/manage-the-calendar-view.md)」を参照してください。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプ ページが、最後にアクセスしたビューで開きます。

1. クリックしてカレンダービューを開くか、カレンダービューを作成します。

   >[!NOTE]
   >
   >レコードタイプに関連付けられた日付フィールドが少なくとも 2 つ存在する場合にのみ、カレンダー表示を作成できます。
1. カレンダー上の任意の場所をダブルクリックします。

   **新規レコード** ボックスが開きます。<!--(********might need a new screen shot for Production - might add a title etc*********ALSO CHECK IF THE SAME ONE NEEDS REPLACING FOR TIMELINE?????)-->

   ![&#x200B; 名前のないレコード バーを含む、カレンダーの新しいレコード ボックス &#x200B;](assets/new-record-small-box-on-calendar.png)

1. 次の情報を更新します。

   * **名前**: レコードの名前を入力します。 空のままにすると、Workfrontはデフォルトで **名称未設定** と名前を付けます。

     >[!TIP]
     >
     >カレンダーの設定に従ってレコード バーにレコードの名前を表示する場合、レコード バーに名前が表示されません（空のままの場合）。

   * **レコード日付フィールド**：レコードの日付を更新します。

     日付フィールドの名前は、カレンダービューが作成された際に、「開始日」および「終了日」で選択されたフィールドに従ってカスタマイズされます。

     デフォルトでは、カレンダーの表示方法に応じて、日付値が事前に選択されています。 次のシナリオが存在します。

      * **月** 別：レコードの開始日と終了日は 1 日に及びます。
      * **週** 別：レコードの開始日と終了日は 2 日間に及びます。

1. （オプション）次のいずれかのアイコンをクリックします。

   * **展開**![&#x200B; 展開アイコン &#x200B;](assets/expand-icon.png) をクリックして、プレビューウィンドウでレコードの詳細を開きます。
   * **削除**![&#x200B; 削除アイコン &#x200B;](assets/delete-icon.png)：レコードを削除します。
   * **閉じる**![&#x200B; 閉じるアイコン &#x200B;](assets/close-icon.png) 新規レコードボックスを閉じます。

   **削除** アイコンをクリックしなかった場合、レコードは直ちにカレンダーとテーブルビューおよびタイムラインビューに追加されます。
1. （オプションおよび条件付き）左上隅のドロップダウンメニューから **月** を選択し、カレンダーのレコードバーの余白の 1 つにポインタを合わせて、バーの端を別の日付にドラッグ&amp;ドロップします。 これにより、レコードの開始日と終了日が自動的に変更されます。

   詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。
1. （オプション）カレンダーのレコードバーをクリックしてレコードの詳細ウィンドウを開き、情報を更新、削除またはコメントを追加します。

   >[!TIP]
   >
   >デフォルトでは、Workfrontはレコードをサムネールとカバー画像に関連付けます。
   >
   >サムネールは、ビューの設定で有効になっている場合にのみ、カレンダービューに表示されます。

   <!--(*********when this is available in both monthly and weekly, add more steps to show resizing the timeline and dragging and dropping the record in the calendar*******)-->

## 外部リストからレコードをコピー&amp;ペーストして作成

1. この記事の[レコードタイプにレコードを手動で追加してレコードを作成](#create-records-by-manually-adding-them-to-a-record-type)の節の説明に従って、テーブルビューでレコードの作成を開始します。

   新しいレコード情報を入力する列（またはフィールド）がテーブルビューに含まれていることを確認します。

1. テーブルの最後の行の&#x200B;**新規 &lt; レコードタイプ名 >**&#x200B;をクリックして、新しいレコードを追加する数だけ新しい行をテーブルに追加します。

   例えば、別のアプリケーションから 10 件の新しいレコードの情報を貼り付ける場合は、10 行をテーブルビューに追加します。

1. 別のアプリケーションで、読み込むレコードのリストを作成します。

   例えば、Excel スプレッドシートを使用してリストを作成できます。

   リストには、情報が表形式で含まれている必要があります。

   >[!TIP]
   >
   > リストの列には、Workfront 内の既存のフィールドに関する情報を含める必要があります。
   >
   > 目的のフィールドが Workfront で既に作成され、シート内の情報が Workfront の各フィールドと一致する正しい形式で表示されていることを確認します。

1. 別のアプリケーションから、複数の行と列を選択し、最初の新しいレコードから始まるレコードタイプのテーブルビューに情報を貼り付けます。

   次の情報が Workfront Planning エリアに読み込まれます。

   * 行には新しいレコードが含まれています
   * 列には、レコードのフィールドに関する情報が入力されます。

## レコードを複製して作成

レコードの複製について詳しくは、「[&#x200B; レコードの複製 &#x200B;](/help/quicksilver/planning/records/copy-or-duplicate-records.md)」を参照してください。

## 接続するレコードの作成

他のレコードから接続する際に、次のオブジェクトタイプを作成できます。

* Workfront計画レコード
* Workfront オブジェクト

この節では、Workfront Planning のレコードを他のレコードと連結しながら作成する方法について説明します。

>[!NOTE]
>
>Workfront プロジェクトおよびポートフォリオをWorkfront Planning レコードに関連付けて作成することは、Planning レコードを他のレコードから関連付けて作成することと似ています。
>
>Workfront Planning からWorkfront オブジェクトを作成する方法については、[&#x200B; レコードに関連付ける際にWorkfront Planning からWorkfront オブジェクトを作成する &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。

既存のレコードから新しいレコードを接続して追加するには、次のものが必要です。

* 接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* レコード。
* この記事の [&#x200B; アクセス要件 &#x200B;](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

他のレコードとの接続時にレコードを作成するには、次の手順に従います。

1. [&#x200B; レコードの接続 &#x200B;](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、Workfront Planning レコードの接続を開始します。 次の領域からレコードを接続できます。

   * Workfront Planning の次の領域の接続フィールド：

      * テーブル表示
      * レコードの詳細ページまたはプレビューボックス

   * Workfrontのプロジェクト、ポートフォリオまたはプログラムの「計画」セクションの「接続」フィールド。

     詳しくは、[Workfront オブジェクトからのレコード接続の管理 &#x200B;](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。

1. （条件付き）接続しようとしてもレコードが見つからない場合は、「**+追加」をクリックし** す。

   または
名前の入力を開始し、「**+追加**」をクリックします。 「**+追加**」ボタンの後に、接続先のレコードタイプの名前が続きます。 例えば、既存のキャンペーンにブランドを追加する場合は「ブランドを追加」などと入力します。 入力した名前は、「追加」ボタンの後にも続きます。

   ![&#x200B; ハイライト表示された、コンテキスト内のレコードを作成する「追加」ボタン &#x200B;](assets/add-button-to-create-records-in-context-highlighted.png)

   レコードが作成され、接続されたレコードフィールドに追加されます。

   >[!IMPORTANT]
   >
   >* レコードから接続する場合、Workfrontで作成できるのは、プロジェクト、ポートフォリオおよびプログラムのみです。
   >
   >* Workfront Planning のレコードからグループや会社を関連付ける場合は、それらのグループや会社を作成できません。
   > 

1. （オプション）作成したレコードを持つレコードタイプのテーブル表示に移動します。 新しいレコードがビューの最後の行に表示されます。
1. （オプション）テーブル表示で新しいレコードの情報の追加を開始します
または
名前をクリックして詳細ページを開き、情報を追加します。

## リクエストフォームをレコードタイプに送信してレコードを作成

レコードタイプのリクエストフォームが作成され、リンクが共有されたら、そのレコードタイプのレコードを作成するリクエストを送信できます。

詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

Workfront ユーザーと組織外のユーザーの両方が、リクエストフォームへのリンクがある場合、Planning レコードタイプにリクエストを送信し、レコードを作成できます。

詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの発行 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

## レコードタイプを CSV または Excel ファイルから読み込む際のレコードの作成

CSV または Excel ファイルを使用してレコードタイプを読み込む場合、レコードを読み込むことができます。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## CSV または Excel ファイルからレコードを読み込むことによるレコードの作成

既存のレコードタイプのレコードを読み込むには、CSV または Excel ファイルから情報を読み込みます。

詳しくは、[CSV または Excel ファイルから情報を読み込むことによるレコードの作成 &#x200B;](/help/quicksilver/planning/records/import-file-to-create-records.md) を参照してください。

## 自動化を使用したレコードの作成

Workfront Planning で自動化を構成できます。自動化を構成すると、アクティブ化されたときに、Planning レコードからトリガーされたときにレコードが作成されます。 作成したレコードは、自動処理をトリガーするレコードに自動的に接続されます。

Workfront計画のレコードのページで、自動処理を設定してアクティブにすることができます。 作成された接続済みレコードは、自動処理を実行するレコードタイプの「接続済み」フィールドに配置されます。

詳しくは、[Adobe Workfront計画レコードの自動作成を使用したオブジェクトの作成 &#x200B;](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。



