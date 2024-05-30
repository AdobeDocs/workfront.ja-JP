---
title: フィールドの作成
description: Adobe Workfront Planning では、レコードタイプの種類ごとにカスタムフィールドを作成できます。そしてフィールドを Workfront Planning レコードに関連付けることができます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '3283'
ht-degree: 88%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Create fields
description: In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with Maestro records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# フィールドの作成

{{maestro-important-intro}}

Adobe Workfront Planning では、レコードタイプのカスタムフィールドを作成できます。そしてフィールドを Workfront Planning レコードに関連付けて、レコードの情報を強化できます。

レコードタイプに関連付けるフィールドを作成するには、まずレコードタイプを作成する必要があります。詳しくは、[リクエストタイプの作成](../architecture/create-record-types.md)を参照してください。

Maestro では、次の方法でフィールドを作成できます。

* 最初から
* レコードタイプを接続する方法
* Excel または CSV ファイルを使用してレコードタイプを読み込む
* レコードタイプを作成する方法
* テンプレートからのワークスペースを作成する方法

Maestro フィールドについて詳しくは、を参照してください。 [フィールドの概要](/help/quicksilver/maestro/fields/fields-overview.md).

## アクセス要件

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>組織は、Adobe Workfront Planning の限定ベータ版プログラムに登録する必要があります。この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Workfront Planning には、アクセスレベルの制御はありません。</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する管理権限</a> </p>  
   <p>システム管理者は、自分が作成したものでないものも含めて、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## フィールドを最初から作成 {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-maestro}}

最後にアクセスしたワークスペースが、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、フィールドを作成するレコードタイプのワークスペースを選択してから、レコードタイプをクリックします。

   レコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。

   >[!TIP]
   >
   >    レコードが表示されない場合は、まだレコードが存在しないか、画面に表示される内容を制限するフィルターが適用されている可能性があります。

   そのレコードタイプに関連付けられている既存のすべてのフィールドが、テーブルビューの列に表示されます。<!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. テーブルビューの右上隅にある **+** アイコンをクリックして、新しいフィールドを追加します。
1. 「**新しいフィールド**」タブで、「**フィールドタイプ**」ボックスでフィールドタイプを検索するか、次のフィールドタイプの中から選択します。

   * [1 行テキスト](#single-line-text)
   * [段落](#paragraph)
   * [複数選択](#multi-select)
   * [単一選択](#single-select)
   * [日付](#date)
   * [数値](#number)
   * [パーセンテージ](#percentage)
   * [通貨](#currency)
   * [チェックボックス](#checkbox)
   * [式](#formula)
   * [ユーザー](#people)
   * [作成者](#created-by)
   * [作成日](#created-date)
   * [最終変更者](#last-modified-by)
   * [最終変更日](#last-modified-date)

   >[!IMPORTANT]
   >
   >    フィールドのフィールドタイプは、保存すると変更できません。

1. 以下の節の説明に従って、それぞれのフィールドの追加に進みます。

### 1 行テキスト {#single-line-text}

1 行テキストフィールドは、限られた英数字の情報を取り込みます。例えば、所有者、関係者、チームまたは組織単位の情報を 1 行テキストフィールドに取り込むことができます。1 行テキストフィールドのコンテンツは、250 文字まで可能です。<!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**1 行テキスト**&#x200B;フィールドタイプを選択します。

   ![](assets/single-line-text-field-type.png)

1. 「**新しいフィールド**」タブで次の情報を追加します。
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列ヘッダーにポインタを合わせると表示されます。
1. 「**作成**」をクリックします。

   新しい単一行フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。


### 段落 {#paragraph}

段落フィールドは、説明フィールドと同様に、レコードに関する追加の英数字情報を取り込みます。

>[!TIP]
>
>* 段落フィールドのコンテンツは、1,000 文字まで可能です。
>
>* リッチテキスト形式を使用して、テーブルビューやレコードの詳細ページに表示される際に、段落フィールドの内容を向上させることができます。詳しくは、[レコードの編集](/help/quicksilver/maestro/records/edit-records.md)を参照してください。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**段落**&#x200B;フィールドタイプを選択します。

   ![](assets/paragraph-field-type.png)


1. 「**新しいフィールド**」タブで次の情報を追加します。
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
1. 「**作成**」をクリックします。

   新しい段落フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。


### 複数選択 {#multi-select}

複数選択フィールドを使用して、ドロップダウンメニューから複数のオプションを選択することにより、任意の形式で追加情報を取り込むことができます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**複数選択**&#x200B;フィールドタイプを選択します。

   ![](assets/multi-select-field-type.png)


1. 「**新しいフィールド**」タブで次の情報を追加します。
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **選択肢**：フィールドを保存した後、ドロップダウンメニューから選択できるオプション。それぞれの選択肢の名前には、数字と文字の両方を使用できます。
1. 「**選択肢を追加**」をクリックして、必要な数だけ選択肢を追加します。複数選択フィールドに追加できる選択肢の数に制限はありません。
1. （オプション）各選択肢を目的の順序で手動でドラッグ＆ドロップするか、または
   選択肢を自動的にアルファベット順に表示する場合は、「**A ～ Z の順に選択肢を並べ替える**」オプションを選択します。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （オプション）選択肢を削除するには、 **x** その右側にあるアイコン。
1. 選択肢の左側にあるカラースウォッチをクリックしてカラーセレクターを展開し、それぞれのオプションの色をカスタマイズします。
1. 「**作成**」をクリックします。

   新しい複数選択フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### 単一選択 {#single-select}

単一選択フィールドでは、ドロップダウンメニューから 1 つのオプションを選択することで、あらゆる形式の追加情報を取り込むことができます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**単一選択**&#x200B;フィールドタイプを選択します。

   ![](assets/single-select-field-type.png)


1. 「**新しいフィールド**」タブで次の情報を追加します。
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **選択肢**：フィールドを保存した後、ドロップダウンメニューから選択できるオプション。それぞれの選択肢の名前には、数字と文字の両方を使用できます。

1. 「**選択肢を追加**」をクリックして、必要な数だけ選択肢を追加します。単一選択フィールドに追加できる選択肢の数に制限はありません。
1. （オプション）各選択肢を目的の順序で手動でドラッグ＆ドロップするか、選択肢を自動的にアルファベット順に表示する場合は、「**A ～ Z の順に選択肢を並べ替える**」オプションを選択します。<!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. （オプション）選択肢を削除するには、 **x** その右側にあるアイコン。
1. 選択肢の左側にあるカラースウォッチをクリックしてカラーセレクターを展開し、それぞれのオプションの色をカスタマイズします。
1. 「**作成**」をクリックします。

   新しい単一選択フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### 日付 {#date}

日付フィールドを使用して、日付と時刻の形式で追加の情報を取り込むことができます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**日付**&#x200B;フィールドタイプを選択します。

   ![](assets/date-field-type.png)


1. 「**新しいフィールド**」タブで次の情報を追加します。
   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **日付形式**：このフィールドに表示する日付形式のタイプ。<!--update this casing - submitted bug for it-->

     次の形式から選択します。
      * **ロケール**：ブラウザーのロケールに一致します。
      * **標準**：05/16/2023
      * **長い日付形式**：2023年5月16日
      * **ヨーロッパ**：16/05/2023
      * **ISO**：2023-05-16
   * **時間フィールドを含める**：タイムスタンプを含める場合は、このオプションを選択します。デフォルトでは選択されていません。<!--update this setting name - submitted bug for it to be changed-->

     次のオプションから選択します。

      * **24 時間**：例：18:00
      * **12 時間**：例：6:00 PM

1. 「**作成**」をクリックします。

   新しい日付フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### 数値 {#number}

数値フィールドタイプは、数値形式の情報を取り込みます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**数値**&#x200B;フィールドタイプを選択します。

   ![](assets/number-field-type.png)
1. 次の情報を「**新しいフィールド**」タブに追加します。

   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **精度**：フィールドに記録する小数点以下の桁数。 6 桁まで表示できます。
   * **負の数を許可**：このフィールドで負の数を許可する場合は、このオプションを選択します。このオプションは、デフォルトでは選択されていません。

   >[!NOTE]
   >
   >    「負の数を許可」を選択し、フィールドが関連付けられているレコードに負の値が格納されている場合、今後この設定の選択は解除できなくなります。

1. 「**作成**」をクリックします。

   新しい数値フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### パーセンテージ {#percentage}

パーセンテージフィールドタイプは、パーセント記号に続く数値形式で情報を取り込みます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**パーセンテージ**&#x200B;フィールドタイプを選択します。

   ![](assets/percentage-field-type.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。
   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **精度**：フィールドに記録する小数点以下の桁数。 6 桁まで表示できます。
   * **負の数を許可**：このフィールドで負のパーセンテージの値を許可する場合は、このオプションを選択します。このオプションは、デフォルトでは選択されていません。

   >[!NOTE]
   >
   >    「負の数を許可」を選択し、フィールドが関連付けられているレコードに負の値が格納されている場合、今後この設定の選択は解除できなくなります。

1. 「**作成**」をクリックします。

   新しいパーセンテージ フィールドは、レコードの種類に列として追加され、その値をレコードに関連付けることができます。

### 通貨 {#currency}

通貨フィールドタイプでは、通貨記号が前に付いた数値形式の情報を取り込みます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**通貨**&#x200B;フィールドタイプを選択します。

   ![](assets/currency-field-type.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。
   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **通貨**：このフィールドに表示する通貨のタイプ。これは、国際標準化機構（ISO）に基づく通貨のリストです。
   * **精度**：フィールドに記録する小数点以下の桁数。 6 桁まで表示できます。
   * **負の数を許可**：このフィールドで負の通貨値を許可する場合は、このオプションを選択します。このオプションは、デフォルトでは選択されていません。

   >[!NOTE]
   >
   >    「負の数を許可」を選択し、フィールドが関連付けられているレコードに負の値が格納されている場合、今後この設定の選択は解除できなくなります。

1. 「**作成**」をクリックします。

   新しい通貨フィールドは、列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### チェックボックス

チェックボックスフィールドタイプを使用して、レコードに単一の「チェックボックス」オプションを追加できます。このフィールドを使用して、特定のレコードの具体的な属性やステータスを示すことができます。例えば、各レコードのトラッキング完了、承認や、その他のバイナリ属性のフラグとして使用できます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**チェックボックス**&#x200B;フィールドタイプを選択します。

   ![](assets/checkbox-field-type.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。
   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
1. 「**作成**」をクリックします。

   新しいチェックボックスフィールドが、列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### 式

数式フィールドは、レコードタイプの他のフィールドの既存の値と、既存の値の計算方法を示す関数を使用して、新しい値を生成します。

詳しくは、[式フィールドの概要](/help/quicksilver/maestro/fields/formula-fields.md)を参照してください。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**式**&#x200B;フィールドタイプを選択します。

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。

   * **名前**：新しいフィールドの名前を入力します。
   * **説明**：新しいフィールドに関する追加情報。
   * **式**：少なくとも 1 文字を入力し始めて式にアクセスし、式がリストに表示されたら選択します。

1. 選択した式をクリックすると、定義が表示され、その形式が表示されます。

   ![](assets/description-of-formula-expression.png)

   サポートする式について詳しくは、[式フィールドの概要](/help/quicksilver/maestro/fields/formula-fields.md)を参照してください。

1. フィールド名をWorkfront Planning に表示されるとおりに追加して、式で参照します。

   >[!NOTE]
   >
   > 複数選択タイプのフィールドは、式に追加できません。



1. 「**作成**」をクリックします。

   新しい式フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。


### ユーザー

ユーザーフィールドタイプを使用すると、レコードにユーザー <!--, job role, or team--> を追加できます。これは「先行入力」フィールドで、ユーザーのみを追加できます<!--, roles, or teams--> はWorkfront インスタンスに既に存在します。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**ユーザー**&#x200B;フィールドタイプを選択します。

   ![](assets/people-field-type.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。
   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **複数の値を許可**：ユーザーがこのフィールドに複数のユーザーを追加できるようにする場合は、このオプションを選択します。このオプションは、デフォルトでは選択されていません。

   >[!NOTE]
   >
   >    「複数の値を許可」を選択し、フィールドが関連付けられたレコードに複数のユーザーが格納されている場合、今後このフィールドの編集時に、この設定の選択は解除できなくなります。

1. 「**作成**」をクリックします。

   新しい人物タイプ フィールドが列としてレコードタイプに追加され、その値をレコードに関連付けることができます。

### 作成者

作成者フィールドタイプを使用して、レコードを作成したユーザーをレコードに追加できます。これは読み取り専用フィールドであり、レコードの作成時にログインしたユーザーの名前が自動的に入力されます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**作成者**&#x200B;フィールドタイプを選択します。

   ![](assets/created-by-field-type.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。

   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--this might change and they might prepopulate it with "Created by"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。

1. 「**作成**」をクリックします。

   新しい作成者タイプフィールドがレコードタイプに列として追加され、その値には各レコードを作成したユーザーの名前が事前入力されます。


### 作成日

「作成日」フィールドタイプを使用して、レコードが作成された日付をレコードに追加できます。 これは読み取り専用フィールドであり、レコードが作成された日付（およびオプションで時刻）が自動的に入力されます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**作成日**&#x200B;フィールドタイプを選択します。

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 次の情報を「**新しいフィールド**」タブに追加します。

   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--this might change and they might prepopulate it with "Created date"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **日付形式**：次の形式から選択します。

      * **ロケール**：ブラウザーのロケールに一致します。
      * **標準**：05/16/2023
      * **長い日付形式**：2023年5月16日
      * **ヨーロッパ**：16/05/2023
      * **ISO**：2023-05-16
   * **時間フィールドを含める**：タイムスタンプを含める場合は、このオプションを選択します。デフォルトでは選択されていません。<!--submitted a UI text change for this - check the UI-->

     次のオプションから選択します。

      * **24 時間**：例：18:00
      * **12 時間**：例：6:00 PM

1. 「**作成**」をクリックします。

   新しい作成日タイプフィールドがレコードタイプに列として追加され、その値にはレコードが作成された日付（または日付および時刻）が事前入力されます。


### 最終変更者

最終変更者フィールドタイプを使用して、レコードを最後に変更したユーザーをレコードに追加できます。これは読み取り専用フィールドであり、レコードが最後に更新されたときにログインしたユーザーの名前が自動的に入力されます。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**最終変更者**&#x200B;フィールドタイプを選択します。

   ![](assets/last-modified-by-field-type.png)

1. 次の情報を「**新しいフィールド**」タブに追加します。

   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--this might change and they might prepopulate it with "Created by"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。

1. 「**作成**」をクリックします。

   新しい最終変更者タイプフィールドがレコードタイプに列として追加され、その値には、各レコードを最後に変更したユーザーの名前が事前入力されます。


### 最終変更日

最終変更日フィールドタイプを使用して、レコードが最後に変更された日付をレコードに追加できます。これは読み取り専用フィールドであり、レコードが最後に更新された日付（およびオプションで時刻）を自動的に入力します。

1. この記事の[フィールドを最初から作成](#create-fields-from-scratch)の節の説明に従ってフィールドの作成を開始し、**作成日**&#x200B;フィールドタイプを選択します。

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 次の情報を「**新しいフィールド**」タブに追加します。

   * **名前**：テーブルまたはレコードページに表示される、フィールドタイプの名前。<!--this might change and they might prepopulate it with "Created date"-->
   * **説明**：フィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **日付形式**：次の形式から選択します。

      * **ロケール**：ブラウザーのロケールに一致します。
      * **標準**：05/16/2023
      * **長い日付形式**：2023年5月16日
      * **ヨーロッパ**：16/05/2023
      * **ISO**：2023-05-16
   * **時間フィールドを含める**：タイムスタンプを含める場合は、このオプションを選択します。デフォルトでは選択されていません。<!--submitted a UI text change for this - check the UI-->

     次のオプションから選択します。

      * **24 時間**：例：18:00
      * **12 時間**：例：6:00 PM

1. 「**作成**」をクリックします。

   新しい最終変更日タイプフィールドがレコードタイプの列として追加され、その値にはレコードが最後に変更された日付（または日付と時刻）が事前入力されます。

## レコードタイプを接続してフィールドを作成

2 つの Maestro レコードタイプ間で、または、1 つのレコードタイプと他のアプリケーションのオブジェクトタイプとの間で新しい接続を追加する際に、リンクされたレコードフィールドを作成できます。

Workfront Planning レコードタイプの接続について詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

## Excel または CSV ファイルを使用してレコードタイプを読み込むことによるフィールドの作成

詳しくは、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

## レコードタイプを作成することでフィールドを作成

レコードタイプを作成する際、新しいレコードタイプに関連付けられた複数のフィールドもデフォルトで作成されます。詳しくは、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

## テンプレートからワークスペースを作成することでフィールドを作成

テンプレートからワークスペースを作成する際に、Adobe Workfront Planning はレコードタイプ用のフィールドを作成します。

詳しくは、[ワークスペースの作成](/help/quicksilver/maestro/architecture/create-workspaces.md)を参照してください。