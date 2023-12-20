---
product-area: reporting
navigation-topic: text-mode-reporting
title: グループ化でのテキストモードの編集
description: 'メモ：すべての FVG 記事をテキストモードで編集するために同じにする )'
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# グループ化でのテキストモードの編集

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

テキストモードを使用して、リストまたはレポートのグループ化を編集し、標準インターフェイスで使用できないフィールドにアクセスし、より複雑なグループを作成できます。

>[!TIP]
>
>標準モードでできるだけ多くのグループを作成し、編集するにはテキストモードに変換することをお勧めします。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートのグループ化を編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートのグループを編集するためのレポートに対する権限を管理します</p> <p>グループに対する権限を管理して編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

レポートまたはリストでテキストモードの使用を開始する前に、必ずWorkfrontのテキストモード構文に関する十分な知識を持っておく必要があります。

詳しくは、以下を参照してください。

* [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [テキストモードの構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [カスタム表示、フィルター、グループ化のサンプル：記事のインデックス](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## グループ化でのテキストモードの編集

テキストモードを使用したグループ化の編集は、レポートとリストで同じです。 レポートから、またはリストからのグループ化へのアクセスは異なります。

>[!NOTE]
>
>グループ化は、レポートでグラフを作成するための必須のレポート要素です。 グラフでは、テキストモードのグループ化はサポートされていません。 レポートへのグラフの追加について詳しくは、 [レポートにグラフを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

グループ化の作成について詳しくは、 [Adobe Workfrontでのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 次のいずれかの操作を行います。

   1. レポートからグループにアクセスするには、レポートに移動し、 **レポートのアクション** > **編集** > **グループ化** タブをクリックします。
   1. リストからグループ化にアクセスするには、リストに移動し、 **グループ化** ドロップダウンメニューで、変更するグループ化の上にマウスを移動し、 **編集** アイコン ![](assets/edit-icon.png).

      グループ化ビルダーが開きます。

1. クリック **グループを追加** グループを追加するには、「 **テキストモードに切り替え** をクリックします。

   >[!TIP]
   >
   標準のインターフェイスでは、最大 3 つのグループを追加できます。 4 番目のグループは、テキストモードを使用してのみ追加できます。また、Workfrontに 4 つを超えるグループ化レベルを持つことはできません。

1. グループ化するフィールドの名前を入力します。

   フィールドがリストに表示されたら、そのフィールドの名前を選択します。

1. クリック **テキストモードに切り替え** をクリックします。

   グループ化がテキストモードで表示されます。

   グループ化をテキストモードで編集すると、Workfrontによって

   ```
   textmode=true
   ```

   グループ化するコードの行。 これは、グループがテキストモードで変更されたことを示します。

   **例：** タスクのリストをプロジェクト名でグループ化し、プライマリ担当者の名前でグループ化するには、テキストモードでグループ化を次のようにします。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   太字の線は必須です。

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   グループ内の各フィールドには、そのフィールドを参照するコードの複数行が含まれます。

   次の表は、テキストモードでグループ化する際の主要な行の概要を示しています。

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   テキストモードのグループ化のキーラインは、テキストモードビューの作成に必要な行に似ています。

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>横断抽出ライン</strong> </th> 
      <th><strong>説明</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>グループ化します。&lt;number&gt;.</strong> </td> 
      <td> <p>コードの各行の前には、このテキストが付きます。 グループ化で選択した同じフィールドを参照するコード行には、次のように同じ番号の番号が付けられます。</p> 
       <ul> 
        <li>レポートの最初のグループ化のグループ番号は 0 です。 最初のグループ化を参照するすべての行は、 <code>group.0</code>.</li> 
        <li>レポートの 2 番目のグループのグループ番号は 1 です。 2 番目のグループ化を参照するすべての行は、 <em><code>group.1</code></em>.</li> 
        <li>レポートの 3 番目のグループのグループ番号は 2 です。 3 番目のグループを参照するすべての行は、 <em><code>group.2</code></em>.</li> 
        <li>4 番目のグループに対しては、テキストモードでのみ、3 のグループ番号を追加できます。 4 番目のグループを参照するすべての行は、次の文字列で始まります。 <em><code>group.3</code></em>.</li> 
       </ul> <p>注意：ビルダーでは、4 つのグループ化はサポートされていません。 これらは、テキストモードを使用する場合にのみサポートされます。 Workfrontは、4 レベルを超えるグループ化をサポートしていません。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>これは、データベースに表示される、オブジェクトまたはフィールドの名前です。 データベースでのオブジェクトおよびフィールドの表示の詳細については、 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラ</a>.</p> <p>次のシナリオが存在します。</p> 
       <ol> 
        <li value="1"> <p> 表示するフィールドの名前が単一名詞ではなくフレーズの場合、 <code>valuefield</code>. 例えば、タスクの計画開始日の場合、コードは次のようになります。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>カスタムフィールドを表示する場合は、 <code>valuefield</code> 「値」は、インターフェイスに表示されるフィールドの実際の名前です。 例えば、「More information」という名前のカスタムフィールドの場合、コードは次のようになります。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>他のオブジェクトに関連するオブジェクトでグループ化する場合は、 <code>valuefield</code> コードの行では、オブジェクトの名前と属性がコロンで区切られます。</p> <p>たとえば、タスクリストのPortfolio名でグループ化した場合、値フィールド行には次の値が含まれます。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>これは、レポート（タスク）のオブジェクトから次の関連オブジェクト（プロジェクト）にアクセスでき、そこからプロジェクト（ポートフォリオ）から次の関連オブジェクト（ポートフォリオ）にアクセスでき、ポートフォリオ名（名前）にアクセスできることを示します。</p> </li> 
       </ol> <p>オブジェクトが相互に接続する方法については、「 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">オブジェクトの相互依存性と階層</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfrontのオブジェクトについて</a>.</p> <p>注意：標準インターフェイスで有効でないテキストモードのフィールドを選択し、標準インターフェイスに切り替えた場合、グループは削除されます。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>この行は、 <code>valuefield</code>. The <code>valueformat</code> オブジェクトまたはフィールドをテキスト、数値、割合、日付のどれで表示するかを指定します。</p> <p>次を使用することをお勧めします。 <code>HTML</code> の <code>valueformat</code>( 特に <code>valueexpression</code>を使用して、情報を最も正確に表示できます。</p> <p>この行の追加の値について詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">テキストモードでの条件付き書式の使用</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>この行を追加して、 <code>valuefield</code>複数のフィールド間の計算でリストをグループ化する場合は、を使用します。</p> <p>次を囲む必要があります。 <code>valuefield</code> を中括弧で囲んだオブジェクトの <code>valueexpression</code>.</p> <p>次のシナリオが存在します。</p> 
       <ol> 
        <li value="1"> <p>グループの名前を大文字で表示する場合は、次のように使用します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>The <code>valuefield</code> の値は、API エクスプローラーで表示されるとおりに入力されます。</p> </li> 
        <li value="2">複数の <code>valuefields</code> それらを一緒に <code>valueexpression </code>行の後には、ピリオドで区切る必要があります。<p>例えば、ポートフォリオの名前をタスクリストで大文字で表示する場合、 <code>valueexpression</code> 行：</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>カスタムフィールドを <code>valueexpression</code> 行をフィールド名の前に指定する必要があります <code>DE:</code> をクリックして、カスタムフィールドであることを示します。 フィールドの名前は、インターフェイスで表示されるとおりに入力されます。</p><p>重要： <span>一部のユーザーに対して制限された権限を持つカスタムフォームセクションに配置されたカスタムフィールドを使用する場合、 <code>valueexpression </code>は、ユーザーがレポートでこの計算を表示する場合は空白です。 カスタムフォームセクションの権限の調整について詳しくは、</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a></span>.</p><p>例えば、「開発者名」というラベルの付いたカスタムフィールドがあり、このフィールドでグループ化して大文字で表示する場合、次のように使用できます <code>valueexpression</code> 次のように指定します。</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Typeahead タイプのカスタムフィールドを参照する場合は、次の式を使用して、「開発者名」というラベルの付いたフィールドで選択されたオブジェクトの名前を参照します。</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>この行はグループ化ラベルを定義します。 この場合、キーに基づく短縮値を使用します。</p> <p>グループ名を変更する場合は、この値を次のように変更できます。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> では、グループ化名に任意のテキストを入力できます。 <code>namekey</code> では、グループの名前を翻訳するために使用するキーを入力する必要があります。</p> <p>グループ名を変更するには、 <code>displayname </code>行が存在しない場合は。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>次の行を追加して、列の名前を変更できます。これは、 <code>namekey/name</code> 値：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>を含む行をすべて削除することをお勧めします。 <code>name </code>グループ名を変更する場合。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）任意のグループに次のコードの 1 行を追加して、グループ化の結果を展開リストと折りたたみリストのどちらで表示するかを指定します。 デフォルトでは、グループ化は展開されて表示されます。


   ```
   group.0.iscollapsed=true
   ```

   結果を折りたたんだ状態でグループ化を表示する場合

   ```
   group.0.iscollapsed=false
   ```

   結果を展開した状態でグループ化を表示する場合

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   * リスト表示時にグループを手動で調整すると、Workfrontでは、ログアウトするまで手動の設定が記憶されます。 再度ログインすると、この設定に従ってリストが表示されます。
   * グループ化の結果は、グラフ要素からアクセスした後で常に展開表示されます。

1. クリック **完了** 変更を保存し、グループ化またはレポートの編集を続行する場合。
1. クリック **グループ化を保存** リスト内または **保存して閉じる** をクリックしてレポートを保存します。
