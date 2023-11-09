---
title: フィールドの作成
description: Adobeマエストロでは、オペレーショナルレコードの種類や分類ごとにカスタムフィールドを作成できます。 次に、このフィールドを Maestro レコードに関連付けることができます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '3495'
ht-degree: 2%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# フィールドの作成

>[!IMPORTANT]
>
>この記事の情報は、Adobe・マエストロに関して、Adobeからの新しいオファーです。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Adobe・マエストロでは、オペレーショナル・レコード・タイプまたは分類のカスタム・フィールドを作成できます。 次に、フィールドを Maestro レコードに関連付けて、レコード情報を強化できます。

レコードタイプを作成してから、関連付けるフィールドを作成する必要があります。 詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## マエストロフィールドに関する考慮事項

* フィールドは、レコードタイプのページのテーブルビューからのみ作成できます。 フィールドは、テーブル表示で列として表示されます。 レコードの種類に関連付けられているすべてのフィールドも、その種類の各レコードの詳細ページに表示されます。

  テーブルの列（またはレコードのフィールド）の管理については、 [テーブル表示の管理](../views/manage-the-table-view.md).

  フィールドの管理の詳細については、次の記事も参照してください。

   * [フィールドを編集](../architecture-and-fields/edit-fields.md)
   * [フィールドを削除](./delete-fields.md)

* レコードタイプに関連付けられたフィールドは、そのタイプのすべてのレコードに関連付けることができます。 <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* レコードタイプに関連付けられたフィールドを別のレコードタイプに追加することはできません。 <!-- this will change when they open the Field library tab when creating a field-->

* 次の方法で、手動または自動でフィールドを作成できます。

   * 手動:

      * レコードタイプのページの [ テーブル ] ビューに列を追加する。 テーブルの列は、レコードタイプに関連付けられたフィールドです。 これらは、レコードの詳細ページに表示されるフィールドと同じです。

        レコードの詳細ページからは、フィールドを作成できません。

        この記事では、フィールドを手動で作成する方法について説明します。

      * レコードタイプをリンクする。 2 つの Maestro レコードタイプまたはレコードタイプと他のアプリケーションのオブジェクトタイプとの間に新しい接続を追加すると、リンクされたレコードフィールドを作成できます。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Maestro レコードタイプの接続について詳しくは、 [レコードタイプを接続](../architecture-and-fields/connect-record-types.md).

      * Excel または CSV ファイルを使用してレコードタイプをインポートする。 詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

   * 自動:

      * デフォルトでは、レコードタイプを作成するたびに使用されます。

        次に、新しい各操作レコードタイプに対してデフォルトで作成される標準フィールドを示します。

         * 名前
         * 説明
         * 開始日
         * 終了日
         * ステータス. レコードのステータスのデフォルト値は次のとおりです。
            * 開発
            * 予定
            * アクティブ
            * 完了
            * 保留中

           他の値を追加したり、既存の値の名前を変更したりできます。

        以下は、新しい分類レコードタイプごとにデフォルトで作成される標準フィールドです。

         * 名前 <!--will more be added? If not, consider rephrasing this bullet-->

      * テンプレートからワークスペースを作成する場合。 テンプレートからワークスペースを作成すると、Maestro はオペレーショナルレコードタイプと分類のフィールドを作成します。 詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).



* 自分または他のユーザーが作成したフィールドの設定を表示および更新できます。 <!--this will change with access/ permissions-->

* 1 つのレコードタイプに対して最大 500 個のフィールドを指定できます。

* フィールド名は 250 文字までです。

* オペレーショナルレコードタイプ、分類、またはワークスペースを削除すると、それらに関連付けられたすべてのフィールドとフィールドの値も削除され、復元できなくなります。 <!-- this might change with a possible recycle bin solution?!-->


## 最初からフィールドを作成する {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅、または **メインメニュー** アイコン ![](assets/main-menu-shell.png)  左上隅にある場合は、「 **マエストロ** ![](assets/maestro-icon.png).

   最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、フィールドを作成するレコードタイプを持つワークスペースを選択して、レコードタイプをクリックします。

   レコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。

   >[!TIP]
   >
   >    レコードが表示されない場合は、まだレコードが存在しない場合や、画面に表示される内容を制限するフィルターが適用されている場合があります。

   レコードタイプに関連付けられている既存のフィールドは、すべてテーブルビューの列に表示されます。 <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. 次をクリック： **+** 新しいフィールドを追加するには、テーブルビューの右上隅にあるアイコンを使用します。
1. Adobe Analytics の **新しいフィールド** 「 」タブで、次のフィールドタイプから選択します。

   * [1 行テキスト](#single-line-text)
   * [段落](#paragraph)
   * [複数選択](#multi-select)
   * [単一選択](#single-select)
   * [日付](#date)
   * [数値](#number)
   * [パーセンテージ](#percentage)
   * [通貨](#currency)
   * [チェックボックス](#checkbox)
   * [ユーザー](#people)
   * [作成者](#created-by)
   * [作成日](#created-date)
   * [最終変更者](#last-modified-by)
   * [最終変更日](#last-modified-date)

   >[!IMPORTANT]
   >
   >    フィールドを保存した後で、フィールドのフィールドタイプを変更することはできません。

1. 以下の節で説明するように、各フィールドの追加を続けます。

### 1 行テキスト {#single-line-text}

1 行のテキストフィールドでは、英数字に制限のある情報が取り込まれます。 例えば、所有者、関係者、チームまたは組織単位の情報を 1 行のテキストフィールドに取り込むことができます。 1 行のテキストフィールドのコンテンツは、最大 250 文字までです。 <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **1 行のテキスト** フィールドタイプ。

   ![](assets/single-line-text-field-type.png)

1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列見出しにマウスポインターを置くと表示されます。
1. 「**作成**」をクリックします。

   新しい 1 行フィールドがレコードタイプに列として追加され、その値をレコードに関連付けることができます。


### 段落 {#paragraph}

段落フィールドでは、「説明」フィールドと同様に、レコードに関する追加の英数字情報が取り込まれます。

>[!TIP]
>
>* 段落フィールドの内容は、1,000 文字までです。
>
>* リッチテキスト書式を使用すると、段落フィールドがテーブルビューやレコードの詳細ページに表示される際に、その内容を拡張できます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **段落** フィールドタイプ。

   ![](assets/paragraph-field-type.png)


1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
1. 「**作成**」をクリックします。

   新しい段落フィールドがレコードタイプの列として追加され、その値をレコードに関連付けることができます。


### 複数選択 {#multi-select}

複数選択フィールドを使用して、ドロップダウンメニューから複数のオプションを選択することで、任意の形式で追加情報を取り込むことができます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **複数選択** フィールドタイプ。

   ![](assets/multi-select-field-type.png)


1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **選択肢**：フィールドを保存した後、ドロップダウンメニューから選択できるオプション。 各選択肢の名前には、数字と文字の両方を使用できます。
1. クリック **選択肢を追加** をクリックして、必要な数だけ選択を追加します。 複数選択フィールドに追加できる選択肢の数に制限はありません。
1. （オプション）各選択肢を必要な順序で手動でドラッグ&amp;ドロップするか、
   **並べ替えの選択肢 A ～ Z** 」オプションを使用します。 <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. 次をクリック： **x** アイコンをクリックして、選択項目を削除します。
1. 選択した色見本の左側をクリックして色セレクターを展開し、各オプションの色をカスタマイズします。
1. 「**作成**」をクリックします。

   新しい複数選択フィールドがレコードタイプに列として追加され、その値をレコードに関連付けることができます。

### 単一選択 {#single-select}

単一選択フィールドでは、ドロップダウンメニューから 1 つのオプションを選択することで、あらゆる形式の追加情報が取得されます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **単一選択** フィールドタイプ。

   ![](assets/single-select-field-type.png)


1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **選択肢**：フィールドを保存した後、ドロップダウンメニューから選択できるオプション。 各選択肢の名前には、数字と文字の両方を使用できます。

1. クリック **選択肢を追加** をクリックして、必要な数だけ選択を追加します。 1 つの選択フィールドに追加できる選択肢の数に制限はありません。
1. （オプション）各選択肢を必要な順序で手動でドラッグ&amp;ドロップするか、 **並べ替えの選択肢 A ～ Z** 」オプションを使用します。 <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. 次をクリック： **x** アイコンをクリックして、選択項目を削除します。
1. 選択した色見本の左側をクリックして色セレクターを展開し、各オプションの色をカスタマイズします。
1. 「**作成**」をクリックします。

   新しい単一選択フィールドがレコードタイプに列として追加され、その値をレコードに関連付けることができます。

### 日付 {#date}

日付フィールドを使用して、日付と時刻の形式で追加の情報を取り込むことができます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **日付** フィールドタイプ。

   ![](assets/date-field-type.png)


1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **日付の形式**：このフィールドに表示する日付形式のタイプ。 <!--update this casing - submitted bug for it-->

     次の形式から選択します。
      * **ロケール**：ブラウザーのロケールに一致します。
      * **標準**: 05/16/2023
      * **Long**:2023 年 5 月 17 日
      * **ヨーロッパ語**: 16/05/2023
      * **ISO**: 2023-05-16
   * **時間フィールドを含める**：タイムスタンプを含める場合は、このオプションを選択します。 デフォルトでは選択されていません。 <!--update this setting name - submitted bug for it to be changed-->

     次のオプションから選択します。

      * **24 時間**：例：18:00
      * **12 時間**：例：午後 6 時

1. 「**作成**」をクリックします。

   新しい日付フィールドがレコードタイプの列として追加され、その値をレコードに関連付けることができます。

### 数値 {#number}

数値フィールドタイプは、数値フォーマットの情報を取り込みます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **数値** フィールドタイプ。

   ![](assets/number-field-type.png)
1. 次の情報を **新しいフィールド** タブ：

   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **精度**：フィールドに記録する小数点以下の桁数です。 最大 6 桁まで表示できます。
   * **負の数を許可**：このフィールドで負の数を許可する場合は、このオプションを選択します。 デフォルトでは、このオプションは選択されていません。

   >[!NOTE]
   >
   >    「負の数を許可」を選択した場合、フィールドが添付されるレコードに負の値が格納される場合は、今後、設定の選択を解除できなくなります。

1. 「**作成**」をクリックします。

   新しい数値フィールドがレコードタイプに列として追加され、その値をレコードに関連付けることができます。

### パーセンテージ {#percentage}

割合 (%) フィールドタイプは、数値フォーマットの情報に続く割合記号を取得します。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **割合** フィールドタイプ。

   ![](assets/percentage-field-type.png)

1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **精度**：フィールドに記録する小数点以下の桁数です。 最大 6 桁まで表示できます。
   * **負の数を許可**：このフィールドで負の割合の値を許可する場合は、このオプションを選択します。 デフォルトでは、このオプションは選択されていません。

   >[!NOTE]
   >
   >    「負の数を許可」を選択した場合、フィールドが添付されるレコードに負の値が格納される場合は、今後、設定の選択を解除できなくなります。

1. 「**作成**」をクリックします。

   新しい割合フィールドがレコードタイプの列として追加され、その値をレコードに関連付けることができます。

### 通貨 {#currency}

通貨フィールドタイプは、通貨記号の前に数値形式の情報を取り込みます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **通貨** フィールドタイプ。

   ![](assets/currency-field-type.png)

1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **通貨**：このフィールドに表示する通貨のタイプ。 これは、国際標準化機構 (ISO) に基づく通貨のリストです。
   * **精度**：フィールドに記録する小数点以下の桁数です。 最大 6 桁まで表示できます。
   * **負の数を許可**：このフィールドで負の通貨値を許可する場合は、このオプションを選択します。 デフォルトでは、このオプションは選択されていません。

   >[!NOTE]
   >
   >    「負の数を許可」を選択した場合、フィールドが添付されるレコードに負の値が格納される場合は、今後、設定の選択を解除できなくなります。

1. 「**作成**」をクリックします。

   新しい通貨フィールドがレコードタイプに列として追加され、その値をレコードに関連付けることができます。

### チェックボックス

「チェックボックス」フィールドタイプを使用して、レコードに単一のチェックボックスオプションを追加できます。 このフィールドを使用して、特定のレコードの特定の属性またはステータスを示すことができます。 例えば、各レコードのトラッキング完了、承認またはその他のバイナリ属性のフラグとして使用できます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **チェックボックス** フィールドタイプ。

   ![](assets/checkbox-field-type.png)

1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
1. 「**作成**」をクリックします。

   新しいチェックボックスフィールドがレコードタイプに列として追加され、その値をレコードに関連付けることができます。

### ユーザー

「ユーザー」フィールドタイプを使用して、ユーザーを追加できます <!--, job role, or team--> をレコードに追加します。 これは先行入力フィールドです。追加できるのはユーザーのみです<!--, roles, or teams--> 既にWorkfrontに存在する

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **People** フィールドタイプ。

   ![](assets/people-field-type.png)

1. 次の情報を **新しいフィールド** タブ：
   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **複数の値を許可**：ユーザーがこのフィールドに複数のユーザーを追加できるようにする場合は、このオプションを選択します。 デフォルトでは、このオプションは選択されていません。

   >[!NOTE]
   >
   >    「複数の値を許可」を選択した場合、フィールドが添付されるレコードに複数のユーザーが格納される場合、このフィールドの編集時に、今後、この設定の選択を解除できなくなります。

1. 「**作成**」をクリックします。

   新しい「人」タイプフィールドがレコードタイプの列として追加され、その値をレコードに関連付けることができます。

### 作成者

「作成者」フィールドタイプを使用して、レコードを作成したユーザーをレコードに追加できます。 これは読み取り専用フィールドで、レコードの作成時にログインしたユーザーの名前が自動的に入力されます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **作成者** フィールドタイプ。

   ![](assets/created-by-field-type.png)

1. 次の情報を **新しいフィールド** タブ：

   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--this might change and they might prepopulate it with "Created by"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。

1. 「**作成**」をクリックします。

   新しい「作成者タイプ」フィールドがレコードタイプに列として追加され、その値には各レコードを作成したユーザーの名前が事前入力されます。


### 作成日

「作成日」フィールドタイプを使用して、レコードが作成された日付をレコードに追加できます。 これは読み取り専用フィールドで、レコードが作成された日付（およびオプションで時刻）が自動的に入力されます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **作成日** フィールドタイプ。

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 次の情報を **新しいフィールド** タブ：

   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--this might change and they might prepopulate it with "Created date"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **日付の形式**：次の形式から選択します。

      * **ロケール**：ブラウザーのロケールに一致します。
      * **標準**: 05/16/2023
      * **Long**:2023 年 5 月 17 日
      * **ヨーロッパ語**: 16/05/2023
      * **ISO**: 2023-05-16
   * **時間フィールドを含める**：タイムスタンプを含める場合は、このオプションを選択します。 デフォルトでは選択されていません。 <!--submitted a UI text change for this - check the UI-->

     次のオプションから選択します。

      * **24 時間**：例：18:00
      * **12 時間**：例：午後 6 時

1. 「**作成**」をクリックします。

   新しい「作成日付タイプ」フィールドがレコードタイプに列として追加され、その値には、レコードが作成された日付（または日時）が事前入力されます。


### 最終変更者

「最終変更者」フィールドタイプを使用して、レコードを最後に変更したユーザーをレコードに追加できます。 これは読み取り専用フィールドで、レコードが最後に更新されたときにログインしたユーザーの名前が自動的に入力されます。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **最終変更者** フィールドタイプ。

   ![](assets/last-modified-by-field-type.png)

1. 次の情報を **新しいフィールド** タブ：

   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--this might change and they might prepopulate it with "Created by"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。

1. 「**作成**」をクリックします。

   新しい「最終変更者タイプ」フィールドがレコードタイプに列として追加され、その値には、各レコードを最後に変更したユーザーの名前が事前入力されます。


### 最終変更日

「最終変更日」フィールドタイプを使用して、レコードが最後に変更された日付をレコードに追加できます。 これは読み取り専用フィールドで、レコードが最後に変更された日付（および時刻）を自動的に入力します。

1. 「 」セクションの説明に従って、フィールドの作成を開始します。 [最初からフィールドを作成する](#create-fields-from-scratch) この記事で、「 **作成日** フィールドタイプ。

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. 次の情報を **新しいフィールド** タブ：

   * **名前**：テーブルまたはレコードの詳細ページに表示される、フィールドタイプの名前。 <!--this might change and they might prepopulate it with "Created date"-->
   * **説明**：フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **日付の形式**：次の形式から選択します。

      * **ロケール**：ブラウザーのロケールに一致します。
      * **標準**: 05/16/2023
      * **Long**:2023 年 5 月 17 日
      * **ヨーロッパ語**: 16/05/2023
      * **ISO**: 2023-05-16
   * **時間フィールドを含める**：タイムスタンプを含める場合は、このオプションを選択します。 デフォルトでは選択されていません。 <!--submitted a UI text change for this - check the UI-->

     次のオプションから選択します。

      * **24 時間**：例：18:00
      * **12 時間**：例：午後 6 時

1. 「**作成**」をクリックします。

   新しい「最終変更日」タイプフィールドがレコードタイプの列として追加され、その値には、レコードが最後に変更された日付（または日時）が事前入力されます。


## レコードタイプをリンクしてフィールドを作成

2 つの Maestro レコードタイプまたはレコードタイプと他のアプリケーションのオブジェクトタイプとの間に新しい接続を追加すると、リンクされたレコードフィールドを作成できます。

Maestro レコードタイプの接続について詳しくは、 [レコードタイプを接続](../architecture-and-fields/connect-record-types.md).

## Excel および CSV ファイルを使用してレコードタイプをインポートしてフィールドを作成する

詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

## レコードタイプを作成してフィールドを作成する

レコードタイプを作成すると、新しいレコードタイプに関連付けられた複数のフィールドもデフォルトで作成されます。 詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

## テンプレートからワークスペースを作成してフィールドを作成

テンプレートからワークスペースを作成すると、Maestro はオペレーショナルレコードタイプと分類のフィールドを作成します。

詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
