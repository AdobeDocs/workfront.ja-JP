---
product-area: reporting
navigation-topic: text-mode-reporting
title: グループ化でテキストモードを編集
description: 「メモ：すべての FVG 記事をテキストモードでの編集に関して同じにする）」
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 99%

---

# グループ化でテキストモードを編集

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

テキストモードを使用して、リストまたはレポートのグループ化を編集すると、標準インターフェイスで使用できないフィールドにアクセスして、より複雑なグループを作成できます。

>[!TIP]
>
>標準モードでできるだけ多くのグループを作成してから、テキストモードに変換して編集することをお勧めします。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポートのグループ化を編集するためのレポート、ダッシュボード、カレンダーへの編集アクセス権限</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートのグループ化を編集するためのレポートへの管理権限</p> <p>グループ化を編集するためのグループ化に対する管理権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

レポートまたはリストでテキストモードを使用するには、あらかじめ Workfront のテキストモード構文に関する十分な知識を持っている必要があります。

詳しくは、以下を参照してください。

* [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [テキストモード構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [カスタム表示、フィルター、グループ化のサンプル：記事のインデックス](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## グループ化でテキストモードを編集

テキストモードを使用したグループ化の編集は、レポートとリストで同じです。グループ化へのアクセスは、レポートから行うか、リストから行うかによって異なります。

>[!NOTE]
>
>グループ化は、レポートでグラフを作成するための必須のレポート要素です。グラフでは、テキストモードのグループ化はサポートされていません。レポートへのグラフの追加について詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

グループ化の作成について詳しくは、[Adobe Workfront でのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)を参照してください。

レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

1. 次のいずれかの操作を行います。

   1. レポートからグループ化にアクセスするには、レポートに移動し、**レポートアクション**／**編集**／「**グループ化**」タブをクリックします。
   1. リストからグループ化にアクセスするには、リストに移動し、**グループ化**&#x200B;のドロップダウンメニューから、変更するグループ化にカーソルを合わせて、**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

      グループ化ビルダーが開きます。

1. 「**グループ化を追加**」をクリックしてグループ化を追加し、ビルダーの右上隅にある「**テキストモードに切り替え**」をクリックします。

   >[!TIP]
   >
   標準のインターフェイスでは、最大 3 つのグループ化を追加できます。4 番目のグループ化を追加するには、テキストモードを使用する必要があります。また、Workfront では 4 つを超えるグループ化レベルを持つことはできません。

1. グループ化するフィールドの名前を入力し始めます。

   フィールドがリストに表示されたら、そのフィールドの名前を選択します。

1. ビルダーの右上隅にある「**テキストモードに切り替え**」をクリックします。

   グループ化がテキストモードで表示されます。

   グループ化をテキストモードで編集すると、Workfront によって

   ```
   textmode=true
   ```

   グループ化にコード行が追加されます。これは、グループ化がテキストモードで変更されたことを示します。

   **例：**&#x200B;タスクのリストをプロジェクト名でグループ化し、プライマリ担当者の名前でさらにグループ化するには、テキストモードでのグループ化は次のようになります。

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   太字の行は必須です。

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

   グループ化の各フィールドには、そのフィールドを参照する複数のコード行が含まれています。

   次の表は、テキストモードでグループ化する際の主要な行の概要を示しています。

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   テキストモードでのグループ化における主要な行は、テキストモードでのビューの作成に必要な行に似ています。

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
      <th><strong>サンプル行</strong> </th> 
      <th><strong>説明</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>group.&lt;number&gt;.</strong> </td> 
      <td> <p>コードの各行の前には、このテキストが付いています。グループ化で選択した同じフィールドを参照するコード行には、以下に示すように同じ数字の番号が付けられます。</p> 
       <ul> 
        <li>レポートの最初のグループ化のグループ番号は 0 です。最初のグループ化を参照するすべての行は、<code>group.0</code> で始まります。</li> 
        <li>レポートの 2 番目のグループ化のグループ番号は 1 です。2 番目のグループ化を参照するすべての行は、<em><code>group.1</code></em> で始まります。</li> 
        <li>レポートの 3 番目のグループ化のグループ番号は 2 です。3 番目のグループ化を参照するすべての行は、<em><code>group.2</code></em> で始まります。</li> 
        <li>テキストモードでのみ、4 番目のグループ化に対しては、3 のグループ番号を追加できます。4 番目のグループ化を参照するすべての行は、<em><code>group.3</code></em> で始まります。</li> 
       </ul> <p>メモ：ビルダーでは、4 つのグループ化はサポートされていません。これらは、テキストモードを使用する場合にのみサポートされます。Workfront は、4 レベルを超えるグループ化をサポートしていません。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>これは、データベースに表示されるオブジェクトまたはフィールドの名前です。データベースでのオブジェクトおよびフィールドの表示について詳しくは、<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>を参照してください。</p> <p>次のシナリオが存在します。</p> 
       <ol> 
        <li value="1"> <p> 表示するフィールドの名前が単一の名詞ではなくフレーズの場合、<code>valuefield</code> 用にキャメルケース構文を使用する必要があります。例えば、タスクの予定開始日の場合、コードは以下のようになります。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>カスタムフィールドを表示する場合は、<code>valuefield</code> の値は、インターフェイスに表示されるフィールドの実際の名前です。例えば、「More information」という名前のカスタムフィールドの場合、コードは以下のようになります。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>コードの <code>valuefield</code> 行を使用して、他のオブジェクトに関連するオブジェクトごとにグループ化する場合には、オブジェクト名と属性をコロンで区切ります。</p> <p>例えば、タスクリストのポートフォリオ名でグループ化した場合、値フィールド行には以下の値が含まれます。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>これは、レポート（タスク）のオブジェクトから次の関連オブジェクト（プロジェクト）にアクセスでき、そこからプロジェクト（ポートフォリオ）から以下の関連オブジェクト（ポートフォリオ）にアクセスでき、さらにポートフォリオ名（名前）にアクセスできることを示します。</p> </li> 
       </ol> <p>オブジェクトが相互に接続する方法について詳しくは、<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront のオブジェクトについて</a>の<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">オブジェクトの相互依存性と階層</a>の節を参照してください。</p> <p>メモ：標準インターフェイスでは無効なフィールドをテキストモードで選択し、標準インターフェイスに切り替えると、グループ化が削除されます。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>この行は、<code>valuefield</code> を表示するために使用される形式を表します。<code>valueformat</code> は、オブジェクトやフィールドがテキスト、数字、率、日付のいずれとして表示されるかを示します。</p> <p>情報を最も正確に表示するために、特に <code>valueexpression</code> を使用する場合には、<code>valueformat</code> に <code>HTML</code> を使用することをお勧めします。</p> <p>この行の追加の値について詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">テキストモードでの条件付き書式の使用</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>複数のフィールド間の計算でリストをグループ化する場合は、この行を追加して <code>valuefield</code> を置換します。</p> <p>オブジェクトの <code>valuefield</code> を <code>valueexpression</code> で使用する場合は、必ず中括弧で囲む必要があります。</p> <p>次のシナリオが存在します。</p> 
       <ol> 
        <li value="1"> <p>グループ化の名前を大文字で表示する場合は、次のように使用します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>オブジェクトの <code>valuefield</code> は、API エクスプローラーで表示される通りのスペルになります。</p> </li> 
        <li value="2">複数の <code>valuefields</code> を<code>valueexpression </code> 行にまとめて追加する場合は、それらをピリオドで区切る必要があります。<p>例えば、ポートフォリオの名前をタスクリストに大文字で表示する場合、<code>valueexpression</code> 行で以下のコードを使用します。</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p><code>valueexpression</code> 行でカスタムフィールドを使用する場合は、フィールド名の前に <code>DE:</code> を付けて、それがカスタムフィールドであることを示す必要があります。フィールドの名前は、インターフェイスでの表示どおりに綴られます。</p><p>重要：<span>一部のユーザーに対して権限が制限されているカスタムフォームセクションに配置されたカスタムフィールドを使用する場合、それらのユーザーがレポートに <code>valueexpression </code>の計算を表示すると、その計算は空白になります。カスタムフォームセクションの権限の調整については、</span><span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a></span>を参照してください。</p><p>例えば、「開発者名」というラベルの付いたカスタムフィールドがあり、このフィールドでグループ化して大文字で表示する場合は、次の <code>valueexpression</code> を使用してそれを指定できます。</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>先行入力タイプのカスタムフィールドを参照する場合は、次の式を使用して、「開発者名」というラベルの付いたフィールドで選択されたオブジェクトの名前を参照します。</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= ／ name=</strong> </td> 
      <td> <p>この行はグループ化ラベルを定義します。この場合は、キーに基づく短縮値が使用されます。</p> <p>グループ化名を変更する場合は、この値を次ぎのように変更できます。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> ここでは、グループ化名に任意のテキストを入力できます。一方、<code>namekey</code> ではグループ化の名前の変換に使用されるキーを入力する必要があります。</p> <p>グループ化名を変更するには、<code>displayname </code>行が存在しない場合は追加することもできます。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>次の行を追加して列の名前を変更できます。これは <code>namekey/name</code> 値を上書きします。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>group.0.displayname=Your Value</code> </p> <p>グループ化名を変更する場合、<code>name </code>を含んだ行をすべて削除することをお勧めします。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）任意のグループ化に次のコード行のいずれかを追加して、グループ化の結果を展開リストと折りたたみリストのどちらで表示するかを指定します。デフォルトでは、グループ化は展開されて表示されます。


   ```
   group.0.iscollapsed=true
   ```

   結果が折りたたまれた状態でグループ化を表示する場合

   ```
   group.0.iscollapsed=false
   ```

   結果が展開された状態でグループ化を表示する場合

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   * リストを表示しているときにグループ化を手動で調整すると、ログアウトするまで Workfront に手動の設定が記憶されます。再度ログインすると、この設定に従ってリストが表示されます。
   * グループ化の結果は、グラフ要素からアクセスした後で常に展開表示されます。

1. 変更を保存しグループ化またはレポートの編集を続行する場合は、「**完了**」をクリックします。
1. リスト内の「**グループ化の保存**」をクリックするか、「**保存して閉じる**」をクリックして、レポートを保存します。
