---
product-area: reporting
navigation-topic: text-mode-reporting
title: レポート内のコレクションの参照
description: レポート内のコレクションの参照
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '2587'
ht-degree: 99%

---

# レポート内のコレクションの参照

Adobe Workfront でレポートを作成すると、一連のオブジェクト、それぞれのフィールド、またはリンクされたオブジェクトをリスト、グリッド、グラフ形式で表示できます。

Workfront でのレポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

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
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>ビュー、フィルター、またはグループ化に対する権限の管理 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## コレクションについて

コレクションは、別のオブジェクトにリンクされているオブジェクトのリストです。

Workfront では、オブジェクト間に次の 2 つの関係があります。

* **1 対 1 の関係**：1 つのオブジェクトは、一度に 1 つの他のオブジェクトにのみリンクできます。\
  例えば、1 つのプロジェクトを一度に 1 つのポートフォリオにのみリンクできます。

* **一対多の関係**：1 つのオブジェクトは、一度に複数の他のオブジェクトにリンクできます。\
  例えば、1 つのプロジェクトに複数のタスクを含めることができます。この場合、タスクのリストはプロジェクトのコレクションを生成します。

>[!IMPORTANT]
>
>標準の Report Builder を使用して、オブジェクト間の 1 対 1 の関係を示すレポートを作成できます。ただし、Report Builder のテキストモードインターフェイスを使用して作成できるのは、オブジェクト間の 1 対多の関係を示すレポートのみです。

標準 Report Builder でのレポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

テキストモードインターフェイスを使用したレポートの作成について詳しくは、次を参照してください。

* [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [テキストモードの一般的な使用法の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
* [テキストモード構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## API エクスプローラーでのコレクションオブジェクトとそのフィールドの検索 {#find-collection-objects-and-their-fields-in-the-api-explorer}

すべてのコレクションをレポートできるわけではありません。

どのオブジェクトを他のコレクションと関連付けることができるかについては、API エクスプローラーを使用する必要があります。\
API エクスプローラーテーブルについて詳しくは、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

レポートできるコレクションを確認するには、次の手順に従います。

1. [API エクスプローラー](../../../wf-api/general/api-explorer.md)に移動します。
1. レポートのオブジェクトを検索します。
1. 「**コレクション**」タブを選択します。

   >[!NOTE]
   >
   >選択したオブジェクトのレポート内では、このタブにリストされたオブジェクトのみをコレクションとして表示できます。

1. それをクリックして、コレクションのオブジェクトを展開します。
1. 表示されたリンクをクリックして、コレクションのオブジェクトに移動します。\
   これにより、コレクションのオブジェクトの「**フィールド**」タブを開くことができます。

   >[!NOTE]
   >
   >コレクションレポートで参照できるのは、このタブに表示されるフィールドのみです。または、このタブに表示されるオブジェクトに関連付けられたフィールドも参照できます。

## レポートでのコレクションの参照

以下のレポート要素内のコレクションからオブジェクトを参照することができます。

* ビュー
* フィルター
* プロンプト

以下のレポート要素内のコレクションからオブジェクトを参照することはできません。

* グループ化
* グラフ

例えば、プロジェクトレポートからタスクやイシューのコレクションを参照して、プロジェクトレベルでタスクやイシューの情報を表示することができます。

* [レポートのビューのコレクションを参照](#reference-a-collection-in-the-view-of-a-report)
* [レポートのフィルターでコレクションを参照](#reference-a-collection-in-the-filter-of-a-report)
* [レポートのカスタムプロンプトでコレクションを参照](#reference-a-collection-in-the-custom-prompt-of-a-report)

### レポートのビューでコレクションを参照 {#reference-a-collection-in-the-view-of-a-report}

レポートのビューでオブジェクトのコレクションを参照して、レポートのオブジェクトに関連付けられたオブジェクトの属性を表示できます。

例えば、レポートのビューでタスクやイシューのコレクション列を作成して、プロジェクトレポートでタスクやイシューの情報を表示できます。

コレクションビューには、名前、日付、プライマリ担当者、完了率などのタスクやイシューに関する情報を表示できます。

ビューには、タスクやイシューに関する情報がリスト形式で表示され、リストのそれぞれの行がタスクやイシューに関する情報を表します。タスクやイシューとそのフィールドのリストは、タスクやイシューが属するプロジェクトと同じ行に表示されます。\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [レポートビューにコレクション列を追加](#add-a-collection-column-in-a-report-view)
* [テキストモードでのコレクションビューの行について](#understand-the-lines-of-a-collection-view-in-text-mode)
* [コレクションビューの制限事項](#limitations-of-a-collection-view)

### レポートビューにコレクション列を追加 {#add-a-collection-column-in-a-report-view}

レポートビューにコレクション列を追加するには、以下の手順を実行します。

1. **メイン**&#x200B;メニュー ![](assets/main-menu-icon.png)、「**レポート**」の順にクリックします。
1. 「**新規レポート**」をクリックします。
1. レポートのオブジェクトを選択します。
1. レポートから移動して、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を選択し、レポート用に選択したオブジェクトに対して使用できるコレクションを決定します。

   コレクションのオブジェクトの選択について詳しくは、この記事にある [API エクスプローラーでコレクションオブジェクトとそのフィールドを検索](#find-collection-objects-and-their-fields-in-the-api-explorer)の節を参照してください。\
   コレクションのオブジェクトの名前をメモします。

1. [API エクスプローラー](../../../wf-api/general/api-explorer.md)を使用して、コレクションに表示するオブジェクトのフィールドのリストに移動します。

   コレクションのオブジェクトのフィールドの検索について詳しくは、この記事にある [API エクスプローラーでコレクションオブジェクトとそのフィールドを検索](#find-collection-objects-and-their-fields-in-the-api-explorer)の節を参照してください。

   コレクションに表示するフィールドの名前をメモします。

1. レポートに戻り、「**列（表示）**」タブで、「**列を追加**」をクリックします。
1. 「**テキストモードに切り替え**」をクリックします。
1. ダイアログボックスの上にマウスを移動して、「**クリックしてテキストを編集**」をクリックします。
1. コレクションオブジェクトのフィールドを参照する場合は、**テキストモード**&#x200B;ダイアログボックスのすべてのテキストを選択してから削除し、続いて以下のコードをペーストします。

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. **列名**&#x200B;を、`displayname` 行の列の名前に置き換えます。
1. **コレクションオブジェクト名**&#x200B;を、[API エクスプローラー](../../../wf-api/general/api-explorer.md)に表示されている `listmethod` 行のコレクションオブジェクトの名前に置き換えます。

1. **コレクションオブジェクトフィールド**&#x200B;を、[API エクスプローラー](../../../wf-api/general/api-explorer.md)に表示されている `valuefield` 行のコレクションオブジェクトフィールドの名前に置き換えます。

   ビューでカスタム式を作成する場合は、**valuefield** を **valueexpression** に置き換えることができます。

   計算されたカスタム式について詳しくは、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   例えば、タスクのリストをプロジェクトレポートに表示する場合です。このコレクションでは、タスクの名前を参照するために `valuefield` 行を使用します。

   次のいずれかの操作を行います。

   * 次のコードを使用して、列を作成します。

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * 次のコードを使用して、レポートにイシューのリストを表示します。

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     コレクションでは、イシューのデータベース名である **opTasks** ではなく、**listmethod** 行に **issues** を使用する必要があることに注意してください。イシューを参照する際に **issue** を使用する場合と **opTask** を使用する場合について詳しくは、[イシューを参照する際に「opTask」と「issue」を使用](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md)を参照してください。

   * プロジェクトレポート内のタスクのリストとそのプライマリ当者を表示する際に、プライマリ当者の名前の隣にあるタスクの名前を参照するには、**valuefield** の代わりに **valueexpression** 行を使用します。

     次のコードを使用して、列を作成します。

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. 次の列は、プロジェクトレポートに表示され、各プロジェクトのすべてのタスクはプライマリ担当者と共に表示されます。

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. 「**保存**」をクリックします。
1. （オプション）レポートの編集を続けます。

   または

   「**保存して閉じる**」をクリックしてレポートを保存します。

#### テキストモードでコレクションビューの行について

コレクションのテキストモードビューの行についての概要を次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>サンプルの行</strong> </th> 
   <th><strong>説明</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>この行には様々な値を使用できますが、コレクションリストの <code style="font-weight: normal;">valueformat</code> は <strong>HTML</strong> をお勧めします。</p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>この行は、列がテキストモードを使用して設定されたことを示します。この行を削除すると、Workfront はデフォルトでその行を再び追加します。</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>ビュー作成時は、リストの <code>type</code> は常に <code>iterate</code> です。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>これは、リスト内の値を区切るために使用される区切り文字です。<br>値の間に改行を追加する <code>&lt;p&gt;</code> の使用をお勧めします。</p> <p>また、次の機能も使用できます。</p> <p><code>&amp;zwj;</code> （ゼロ幅の結合子）。コレクションの値は、それらの間に区切りはありません。<br><strong>,</strong> =コンマ区切り。コレクションの値は、コンマで区切られ、スペースは含まれません。<br><strong>/</strong> =スラッシュ区切り。コレクションの値はスラッシュで区切られます。<br><strong>-</strong> =ダッシュ区切り。コレクションの値はダッシュで区切られます。<br>この行を空のままにすると、デフォルトでは、コレクションの値の間にコンマとスペースが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>列名</em> </td> 
   <td> <p><strong>列名</strong>を新しい列の実際の名前に置き換えます。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> この行は、参照するコレクションを定義します。</p> <p><a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>に表示されるように、<strong>コレクションオブジェクト名</strong>をコレクション内で参照するオブジェクトの名前に置き換えます。この値は、通常、コレクションオブジェクト名の複数形式です。</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>この行は、コレクションオブジェクトから参照するフィールドを定義します。</p> <p><a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>に表示されるように、<strong>コレクションオブジェクトフィールド</strong>をコレクション内で参照するオブジェクトのフィールドの名前に置き換えます。</p> <p>この行を次に置き換えることができます。</p> <p><strong>valueexpression</strong>=計算済みコレクションオブジェクトフィールド</p> <p><strong>valueexpression</strong> を使用すると、計算済みカスタム式を列に表示できます。</p> <p><strong>valueexpression</strong> 行のフォーマット方法について詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">テキストモードの構文の概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### コレクションビューの制限事項 {#limitations-of-a-collection-view}

コレクションビューを作成する際は、次の制限事項を考慮してください。

* コレクションデータの表示順序は変更できません。
* コレクションビューには条件付き書式を適用できません。
* コレクション内のオブジェクトをクリック可能なリンクにすることはできません。
* 別のコレクションのコレクションビューは作成できません。\
  例えば、各タスクのすべての担当者をプロジェクトレポートに表示することはできません。プライマリ担当者は、プロジェクトビューの各タスクに対してのみ表示できます。

### レポートのフィルターでコレクションの参照 {#reference-a-collection-in-the-filter-of-a-report}

レポートのフィルターでオブジェクトのコレクションを参照し、レポートのオブジェクトに関連付けられたオブジェクトの属性をフィルタリングできます。

例えば、フィルターステートメントでタスクの属性やプロジェクトのイシューを参照して、プロジェクトレポート内のタスクまたはイシューの情報をフィルタリングできます。

レポートフィルターでコレクションへの参照を追加するには、次の手順に従います。

1. **メイン**&#x200B;メニュー ![](assets/main-menu-icon.png) をクリックし、次に「**レポート**」をクリックします。
1. 「**新規レポート**」をクリックします。
1. レポートのオブジェクトを選択します。
1. レポートから移動して、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を選択し、レポート用に選択したオブジェクトに対して使用できるコレクションを決定します。

   コレクションのオブジェクトの選択について詳しくは、この記事にある [API エクスプローラーでコレクションオブジェクトとそのフィールドを検索](#find-collection-objects-and-their-fields-in-the-api-explorer)の節を参照してください。

   コレクションのオブジェクトの名前をメモします。

1. [API エクスプローラー](../../../wf-api/general/api-explorer.md)を使用して、コレクションに表示するオブジェクトのフィールドのリストに移動します。

   コレクションのオブジェクトのフィールドの検索について詳しくは、この記事にある [API エクスプローラーでコレクションオブジェクトとそのフィールドを検索](#find-collection-objects-and-their-fields-in-the-api-explorer)の節を参照してください。

   コレクションに表示するフィールドをメモします。

1. レポートに戻り、「**フィルター**」タブで、「**テキストモードに切り替え**」をクリックします。

1. **レポートのフィルタールールを設定**&#x200B;エリアに次のコードをペーストします。

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. **コレクションオブジェクト名**&#x200B;を、[API エクスプローラー](../../../wf-api/general/api-explorer.md)に表示されているコレクションオブジェクトの名前に置き換えます。この値は、通常、コレクションオブジェクト名の複数形式です。

1. **コレクションオブジェクトフィールド**&#x200B;を、[API エクスプローラー](../../../wf-api/general/api-explorer.md)に表示されているコレクションオブジェクトのフィールドの名前に置き換えます。

1. **コレクションオブジェクトの値**&#x200B;を、Workfront に表示されるコレクションオブジェクトの値に置き換えます。
1. **修飾子の値**&#x200B;を有効な修飾子に置き換えます。

   修飾子のリストについて詳しくは、[フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)を参照してください。\
   例えば、名前に「マーケティング」が含まれるタスクのみを表示するプロジェクトレポートを作成するには、次のコードを使用します。

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   このレポートには、名前に「マーケティング」という単語を含むタスクが 1 つ以上あるプロジェクトのみが表示されます。

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. イシューの名前をフィルタリングするには、次のコードを使用します。

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >コレクション オブジェクト名には、API エクスプローラーでイシューを表示する際に使用する `optask` ではなく、`issues` を使用する必要があることに注意してください。

1. 「**完了**」をクリックします。
1. （オプション）レポートの編集を続けます。

   または

   「**保存して閉じる**」をクリックしてレポートを保存します。

### レポートのカスタムプロンプトでコレクションを参照 {#reference-a-collection-in-the-custom-prompt-of-a-report}

レポートのカスタムプロンプトでオブジェクトのコレクションを参照して、レポートのオブジェクトに関連付けられたオブジェクトの属性についてレポートの結果をフィルタリングできます。

例えば、レポートのカスタムプロンプトでプロジェクトのタスクの属性への参照を使用することにより、プロジェクトレポートでタスク情報の入力を求めることができます。

>[!NOTE]
>
>標準プロンプトでは、コレクションを参照できません。

カスタムプロンプトは、ステートメントがアンパサンド記号で結合されたカスタムフィルターです。まずフィルターでステートメントを作成し、アンパサンドを使用してステートメントの行を結合することをお勧めします。

コレクション参照を含むフィルターステートメントの作成について詳しくは、[レポートのフィルターでコレクションを参照](#reference-a-collection-in-the-filter-of-a-report)を参照してください。

レポートのカスタムプロンプトでコレクションへの参照を追加するには、以下のように行います。

1. **メイン**&#x200B;メニュー ![](assets/main-menu-icon.png)、「**レポート**」の順にクリックします。
1. 「**新規レポート**」をクリックします。
1. レポートのオブジェクトを選択します。
1. この記事にある[レポートのフィルターでコレクションを参照](#reference-a-collection-in-the-filter-of-a-report)の節の説明に従って、コレクション参照を含むフィルターを作成します。
1. 「**レポート設定**」をクリックします。
1. 「**レポートのプロンプト**」をクリックします。
1. 「**プロンプトを追加**」をクリックします。
1. 「**カスタムプロンプト**」をクリックします。
1. 「**フィールド****名**」フィールドでプロンプトの名前を指定します。

1. **ドロップダウン項目のラベル**&#x200B;を指定します。
1. 「**状況**」フィールドで以下を指定します。

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. （オプション）この選択肢がデフォルトでプロンプトに表示されるかどうかを指定します。
1. **コレクションオブジェクト名**&#x200B;を、[API エクスプローラー](../../../wf-api/general/api-explorer.md)に表示されているコレクションオブジェクトの名前に置き換えます。この値は、通常、コレクションオブジェクト名の複数形です。
1. **コレクションオブジェクトフィールド**&#x200B;を、[API エクスプローラ](../../../wf-api/general/api-explorer.md)に表示されているコレクションオブジェクトのフィールドの名前に置き換えます。
1. **コレクションオブジェクトの値**&#x200B;を、Workfront に表示されるコレクションオブジェクトの値に置き換えます。

   例えば、タスク名に「マーケティング」が含まれるプロジェクトをフィルタリングする場合は、**コレクションオブジェクトの値**&#x200B;を、**マーケティング**&#x200B;に置き換えます。

1. **修飾子の値**&#x200B;を有効な修飾子に置き換えます。

   修飾子のリストについて詳しくは、[フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)を参照してください。

   **例：**&#x200B;例えば、特定のユーザーに 1 つ以上のタスクが割り当てられているプロジェクトのみを表示するカスタムプロンプトを使用してプロジェクトレポートを作成するには、次のコードを使用します。

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   これにより、GUID が 57cf1b7a000077c9f02f66cb09c8f86c のユーザーに割り当てられたタスクをリストされたすべてのプロジェクトに 1 つ以上含むレポートが生成されます。

   >[!NOTE]
   >
   >[API エクスプローラー](../../../wf-api/general/api-explorer.md)にあるように、タスクのプライマリ担当者（「割り当て先」フィールド）の名前を参照することはできません。参照できるのは、プライマリ担当者の ID のみです。

   例えば、プロジェクトのイシューによって特定のユーザーに割り当てられたプロジェクトをフィルタリングするには、次のコードをカスタムプロンプトに使用します。

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   これにより、GUID が 57cf1b7a000077c9f02f66cb09c8f86c のユーザーに割り当てられたイシューをリストされたすべてのプロジェクトに 1 つ以上含むレポートが生成されます。

   >[!NOTE]
   >
   コレクションオブジェクト名に&#x200B;**イシュー**&#x200B;を使用する必要があることに注意してください。現時点で、API エクスプローラーにイシューのコレクションオブジェクト名は用意されていません。

1. 「**完了**」をクリックします。
1. （オプション）レポートの編集を続けます。

   または

   「**保存して閉じる**」をクリックしてレポートを保存します。
