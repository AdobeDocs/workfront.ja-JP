---
title: レコードを作成
description: Adobe Workfront Planning を使用する場合、レコードはレコードタイプのインスタンスです。 Workfront Planning で各レコード・タイプに一意のレコードを作成するには、レコードを手動でテーブル・ビューに追加するか、リストからインポートするか、複製するか、または他のレコードに接続する際に作成します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '2419'
ht-degree: 22%

---


# レコードの作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

次のいずれかを行うことで、レコードを作成できます。

* [レコードタイプのテーブル表示からインラインで追加してレコードを作成](#create-records-by-adding-them-inline-from-the-record-type-table-view)
* [任意のレコードタイプ表示から「新規レコード」または「レコードをリクエスト」ボタンを使用してレコードを作成](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [外部リストからのレコードのリストのコピー&amp;ペースト](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [テーブルビューからレコードを複製](#create-records-by-duplicating-them)
* [他のレコードから接続する際のレコードの作成](#create-records-as-you-connect-them)
* [リクエストフォームをレコードタイプに送信してレコードを作成](#create-records-by-submitting-a-request-form-to-a-record-type)
* [CSV または Excel ファイルから情報を読み込んでレコードを作成](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [自動化を使用したレコードの作成](#create-records-by-using-automations)

テーブルビューまたはタイムラインビューでのレコードの管理については、次の記事を参照してください。

* [テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)
* [タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
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
   <p>レコードを関連付ける際に作成するオブジェクトタイプ（プロジェクト、プログラム、ポートフォリオ）のWorkfrontでのアクセス権を編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードを追加するワークスペース <span class="preview"> およびレコードタイプ </span> に対する投稿以上の権限。 </p>
   <p>レコード ページの「レコードをリクエスト」ボタンを使用してレコードを作成するための、ワークスペース <span class="preview"> およびレコードタイプ </span> に対する表示以上の権限</p>
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
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

   * テーブルの最後の行にある「**新規レコード**」をクリックします

   * テーブルの任意の列または行から、キーボードの **Shift + Enter** キーをクリックします。これにより、開始レコードの下に空の行が追加されます。
   * レコードの主フィールドにポインタを合わせ、フィールドの右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、**上にレコードを挿入** または **下にレコードを挿入** をクリックします。

   ![ テーブルの行に新しいキャンペーンを追加 ](assets/adding-a-new-campaign-in-table-row.png)

   Workfrontは、新しい各レコードにサムネールを自動アップロードします。 これらの画像は、後で変更できます。 詳しくは、[ レコードへのかぶり画像を追加する ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) を参照してください。

   新しいレコードがテーブルに追加されます。

1. 新しいレコードのプライマリフィールドをクリックします

   または

   レコード名の左側にある **詳細を開く** アイコン ![ テーブル名フィールドで詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックします。

   テーブルにプレビューボックスが表示されます。

1. プレビューボックスに表示されるフィールドに、新しいレコードに関する情報を入力します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクするときにレコードを識別すると便利なので、レコードの主フィールドの情報を追加することをお勧めします。 主フィールドについて詳しくは、[ テーブル表示の管理 ](/help/quicksilver/planning/views/manage-the-table-view.md) および [プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

1. （条件付き）テーブルにレコードを追加する場合、レコードのプレビューボックスを開く前に、各行に引き続き情報を追加してから、キーボードの **Enter** をクリックして変更を保存します。

   または

   新しいレコードの名前、またはレコード名の左側にある **詳細を開く** アイコン ![ テーブル名フィールドで詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックしてプレビューボックスを開き、詳細領域でレコードの情報を編集します。

   >[!TIP]
   >
   >**詳細を開く** アイコンにアクセスできるのは、レコードの名前フィールド（名前フィールドがプライマリフィールドの場合）のみです。

1. （オプション）レコードのプレビューボックスで、右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで詳細を開くアイコン ](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを新しいタブで開きます。 レコードページでレコードの編集を続行します。 詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

   Workfront では、変更を自動的に保存します。

1. （オプション） レコードのページを開いた場合は、プレビューボックスを閉じるか、レコード名の左側にある戻る矢印をクリックします。

1. （オプション）テーブル表示で新しいレコードや情報を追加する際に、テーブル表示から次のキーボードショートカットを使用して、それらの追加の取り消しまたはやり直しを行います。

   * CTRL + Z （Macの場合は ⌘ + Z）
   * Ctrl + Shift + Z （Macの場合は ⌘ + Shift + Z）

## 任意のレコードタイプ表示から「新規レコード」または「レコードをリクエスト」ボタンを使用してレコードを作成

ワークスペース <!--<span class="preview">and record type</span>--> に対する表示権限を持つユーザーは、レコードタイプ ページの「レコードをリクエスト」ボタンを使用してのみレコードを作成できます。

ワークスペースに対する投稿権限と管理権限を持つユーザー <!--<span class="preview">and record type</span>-->、レコードタイプ ページの「新しいレコード」ボタンを使用してレコードを作成できます。
<!--did the permissions to record types get released?? if not, take the record type reference here out; AND else-where in this article, including access requirements table-->

>[!IMPORTANT]
>
>表示権限を持つユーザーがリクエストフォームを使用してレコードを追加するには、ワークスペースマネージャーがレコードタイプのリクエストフォームを作成する必要があります。 そうしないと、表示権限のユーザーはレコードを作成できません。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがビューに表示されます。

1. （条件付き）ワークスペースと権限に応じて、任意の表示で、画面の右上隅にある次のいずれかをクリック <!--<span class="preview">and record type</span>--> ます。

   * ワークスペースコン <!--<span class="preview">and record type</span>--> ールに対する投稿以上の権限がある場合は、「**新しいレコード**」をクリックします

     または

   * Workspace <!--<span class="preview">and record type</span>--> ージに対する表示権限がある場合は、「**レコードをリクエスト**」をクリックします。

1. （条件付き） **新規レコード** をクリックした場合、次の操作を行います。

   1. 次のいずれかの方法でレコードを作成し、[**続行**] をクリックします。

      * **手動で追加**。 レコードのプレビューボックスが開きます。\
        この記事の [ レコードタイプのテーブル表示からインラインで追加してレコードを作成する ](#create-records-by-adding-them-inline-from-the-record-type-table-view) の手順 6 から始まる節で説明しているように、レコードに関する情報を追加します。<!--insure this stays accurate-->
      * **ファイルからアップロード**
[CSV または Excel ファイルから情報をインポートしてレコードを作成する ](/help/quicksilver/planning/records/import-file-to-create-records.md) の記事の説明に従って、手順 6 からレコードを追加します。<!--ensure this stays accurate-->
      * **リクエストの送信**
レコードタイプのリクエストフォームが開きます。

        ワークスペースマネージャーは、リクエストフォームを使用してレコードを追加できるように、リクエストフォームを作成する必要があります。

        >[!TIP]
        >
        >一部のレコードタイプには複数のフォームがある場合があります。 1 つをクリックして開きます。

        [ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) の説明に従って、手順 6 からレコードを追加します。<!--ensure this stays accurate-->

      ![ レコード選択モーダルを作成する 3 つの方法 ](assets/three-ways-to-create-records-choice-modal.png)

1. （条件付き） **レコードをリクエスト** をクリックした場合、次の操作を行います。

   1. （条件付き）レコードタイプに複数のリクエストフォームがある場合は、1 つをクリックして選択します。
   2. [ レコードを作成するためのAdobe Workfront Planning リクエストの送信 ](/help/quicksilver/planning/requests/submit-requests.md) の説明に従って、手順 6 からレコードを作成するためのフォームに情報を追加し続けます。<!--ensure this stays accurate-->

1. （条件付き）新しいレコードを確認します。

   レコードの追加方法によっては、次の問題が発生する場合があります。

   * 承認プロセスを備えたリクエストフォームを使用して追加することを選択した場合を除き、新しいレコードがレコードタイプに追加されます。 レコードを作成する前に、すべての承認者から承認を付与する必要があります。
   * CSV または Excel スプレッドシートを使用してレコードを追加した場合、複数のレコードがレコードタイプに追加されます。
   * リクエストフォームを送信してリクエストを追加した場合、新しいリクエストがWorkfront リクエスト エリアの「計画」タブに追加されます。

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

レコードの複製について詳しくは、「[ レコードの複製 ](/help/quicksilver/planning/records/copy-or-duplicate-records.md)」を参照してください。

## 接続するレコードの作成

他のレコードから接続する際に、次のオブジェクトタイプを作成できます。

* Workfront計画レコード
* Workfront オブジェクト

この節では、Workfront Planning のレコードを他のレコードと連結しながら作成する方法について説明します。

>[!NOTE]
>
>Workfront プロジェクトおよびポートフォリオをWorkfront Planning レコードに関連付けて作成することは、Planning レコードを他のレコードから関連付けて作成することと似ています。
>
>Workfront Planning からWorkfront オブジェクトを作成する方法については、[ レコードに関連付ける際にWorkfront Planning からWorkfront オブジェクトを作成する ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。

既存のレコードから新しいレコードを接続して追加するには、次のものが必要です。

* 接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* レコード。
* この記事の [ アクセス要件 ](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

他のレコードとの接続時にレコードを作成するには、次の手順に従います。

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、Workfront Planning レコードの接続を開始します。 次の領域からレコードを接続できます。

   * Workfront Planning の次の領域の接続フィールド：

      * テーブル表示
      * レコードの詳細ページまたはプレビューボックス

   * Workfrontのプロジェクト、ポートフォリオまたはプログラムの「計画」セクションの「接続」フィールド。

     詳しくは、[Workfront オブジェクトからのレコード接続の管理 ](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。

1. （条件付き）接続しようとしてもレコードが見つからない場合は、「**+追加」をクリックし** す。

   または
名前の入力を開始し、「**+追加**」をクリックします。 「**+追加**」ボタンの後に、接続先のレコードタイプの名前が続きます。 例えば、既存のキャンペーンにブランドを追加する場合は「ブランドを追加」などと入力します。 入力した名前は、「追加」ボタンの後にも続きます。

   ![ ハイライト表示された、コンテキスト内のレコードを作成する「追加」ボタン ](assets/add-button-to-create-records-in-context-highlighted.png)

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

詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

Workfront ユーザーと組織外のユーザーの両方が、リクエストフォームへのリンクがある場合、Planning レコードタイプにリクエストを送信し、レコードを作成できます。

詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

## レコードタイプを CSV または Excel ファイルから読み込む際のレコードの作成

CSV または Excel ファイルを使用してレコードタイプを読み込む場合、レコードを読み込むことができます。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## CSV または Excel ファイルからレコードを読み込むことによるレコードの作成

既存のレコードタイプのレコードを読み込むには、CSV または Excel ファイルから情報を読み込みます。

詳しくは、[CSV または Excel ファイルから情報を読み込むことによるレコードの作成 ](/help/quicksilver/planning/records/import-file-to-create-records.md) を参照してください。

## 自動化を使用したレコードの作成

Workfront Planning で自動化を構成できます。自動化を構成すると、アクティブ化されたときに、Planning レコードからトリガーされたときにレコードが作成されます。 作成したレコードは、自動処理をトリガーするレコードに自動的に接続されます。

Workfront計画のレコードのページで、自動処理を設定してアクティブにすることができます。 作成された接続済みレコードは、自動処理を実行するレコードタイプの「接続済み」フィールドに配置されます。

詳しくは、[Adobe Workfront計画レコードの自動作成を使用したオブジェクトの作成 ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。



