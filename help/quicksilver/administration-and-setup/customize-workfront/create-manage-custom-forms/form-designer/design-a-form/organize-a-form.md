---
title: フォームデザイナーを使用したフォームの整理とプレビュー
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: カスタムフォームは、フォームデザイナーを使用して整理できます。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 529de9d31be883325d425dceb286d750397c5d8e
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# フォームデザイナーを使用したフォームの整理とプレビュー

{{highlighted-preview-article-level}}

カスタムフォームをフォームデザイナーと共に整理できます。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>
   <p>現在のプラン：標準</p>
   <p>または</p>
   <p>レガシープラン：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## セクション区切りを追加

カスタムフォームのカスタムフィールドとウィジェットを、見出し付きのセクションにグループ化できます。 これは、フォームに入力するユーザーに、整理されたエクスペリエンスを提示する場合に役立ちます。 また、特定のカスタムフィールドとウィジェットへのアクセスを特定のユーザーに制限する必要がある場合は、それらをセクションに配置し、そのセクションへのアクセス権をそれらのユーザーにのみ付与することができます。

例えば、システム管理者だけが表示または編集できる機密情報を追跡する必要がある場合は、「管理者のみ」の権限を持つセクション区切りを作成し、そのセクションに機密フィールドを配置できます。

セクションに対して選択するアクセス設定は、カスタムフォームが添付されるWorkfrontオブジェクトに対するユーザーの権限に直接関連付けられます。 ユーザがそのオブジェクトの表示、投稿、管理に対するアクセス権を持っているかどうかに基づいて、セクションの表示/非表示を切り替えることができます。 また、セクションを「管理者のみ」に設定して、システム管理者のアクセスレベルのユーザーのみがアクセスできるようにすることもできます。

オブジェクトに対する権限については、 [オブジェクトに対する共有権限の概要](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、 [フォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### カスタムフォームのセクションへのアクセスの作成と設定

1. カスタムフォームの作成または編集を開始し、フィールドを追加します ( [フォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. クリック **断面分割** をクリックし、キャンバス上の目的の位置にドラッグします。

1. 右側のパネルで、セクションに必要なオプションを設定します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ラベル</td> 
      <td> <p>（必須）セクションの上に表示する説明的なラベルを入力します。 ラベルはいつでも変更できます。</p> <p><b>重要</b>:このラベルでは特殊文字を使用しないでください。 レポートでは正しく表示されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>ユーザーにセクションの目的を説明する場合は、テキストを入力します。 これは、カスタムフォームのセクションのラベルの下に表示されます。</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>アクセスを許可</p> </td> 
      <td> <p> このセクションを表示し、そのフィールド値を編集するために、カスタムフォームが添付されるオブジェクトに対してユーザーが必要とする権限を選択します。 
       <p>以下の権限をで使用できます。 <b>オブジェクトにこのアクセス権を持つユーザーは、フィールド値を表示できます</b>:</p> 
         <ul>  
          <li><p><b>制限付き編集</b>:（オブジェクトがプロジェクト、タスク、タスク、タスクまたはユーザーの場合にのみ使用できます）。</p> 
          <p>プロジェクト、タスクまたはイシューの場合に、ユーザーがオブジェクトに投稿できるようにします。</p>
          <p>ユーザーがプロファイルを編集したり、オブジェクト（ユーザーの場合）に対するプロファイル権限を所有したりできます。</p></li> 
          <li><b>編集</b>:オブジェクトに対する権限の管理 </li> 
          <li><b>管理者のみ</b>:システム管理者のアクセスレベル</li> 
         </ul> </li> 
        <p>以下の権限をで使用できます。 <b>このオブジェクトへのアクセス権を持つユーザーは、フィールド値を編集できます</b>: </p> 
         <ul> 
          <li> <p><b>制限付き編集</b>:（オブジェクトがプロジェクト、タスク、タスク、タスクまたはユーザーの場合にのみ使用できます）。</p> 
           <p>オブジェクトがプロジェクト、タスク、またはイシューの場合は、この権限を持つユーザーがオブジェクトに貢献できます</p>
          <p>オブジェクトがユーザーの場合、この権限を持つユーザーは、プロファイルを編集したり、そのオブジェクトに対するプロファイル権限を所有したりできます。</p> 
          <li><b>編集</b>:オブジェクトに対する権限の管理 </li> 
          <li><b>管理者のみ</b>:システム管理者のアクセスレベル</li> 
         </ul> </li> 
       </ul> 
       <p>オブジェクトに対する権限については、 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>.</p> 
       <p><b>メモ</b>:  
       <ul> 
       <li> <p>ここで指定した権限を持たないユーザーは、セクションのカスタムフィールドとウィジェットを表示できません。 </p> <p>これは、フィールドの値をレポートに表示する場合や、テキストモードのレポートで計算フィールドで使用する場合にも当てはまります。</p> </li> 
       <li> <p>複数のオブジェクトタイプをフォームに関連付けると、これらの手順で使用できる表示および編集権限が変更される場合があります。 詳しくは、 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">複数のオブジェクトタイプが、カスタムフォームのセクション区切り権限に与える影響</a> 」を参照してください。</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 1 つ以上のカスタムフィールドまたはウィジェットを新しいセクションにドラッグまたは追加します。 これは、セクションを保存する前に必要です。

1. クリック **完了**.

   >[!TIP]
   >
   >次をクリックできます。 **適用** カスタムフォームの作成中はいつでも、変更内容を保存し、フォームを開いたままにすることができます。

### 複数のオブジェクトタイプが断面の分割権限に与える影響 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

カスタムフォームセクションの改ページに対する制限付き編集権限は、プロジェクト、タスク、問題、ユーザーの各オブジェクトタイプに対してのみ使用できます。

制限付き編集権限を持つセクション区切りを持つカスタムフォームでは、他のオブジェクトタイプ (Portfolio、プログラム、ドキュメント、会社、請求レコード、繰り返し、費用、グループ ) をフォームに追加すると、編集権限に切り替えます。

>[!INFO]
>
>**例：** Project オブジェクトの種類に関連付けられたカスタムフォームでは、セクション区切りは、制限付き編集権限を持つように設定されます。
>
>Portfolioオブジェクトの種類をフォームに追加すると、フォーム内のセクション区切りに対して「制限付き編集」権限オプションを使用できなくなります。
>
>画面上のメッセージで、[ 編集 ] 権限に切り替えるように求められます。この権限は、[ プロジェクト ] オブジェクトの種類と [Portfolio] オブジェクトの種類の両方に対応する最低レベルの権限です。


## カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置


1. カスタムフォームの作成または編集を開始します ( [フォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. カスタムフィールドとウィジェットを同じ行に配置するには、その間に行が表示されるまで、隣り合わせにドラッグします。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 以下を使用して、 **プレビュー** ボタンを使用して、カスタムフィールドとウィジェットがフォームでどのように表示されるかを確認できます。
>* ユーザーが表示しているときに使用可能な画面領域の量に応じて、カスタムフィールドとウィジェットがフォームで同じように表示されない場合があります。 例えば、横方向のスペースが制限されている場合、フィールドの行の 3 番目のフィールドは、次のフィールドの行に折り返されます。


1. （オプション）カスタムフィールドまたはウィジェットを別のフィールドの上または下に配置するには、項目の間に青い横線が表示されるまで、上または下にドラッグします。

1. 変更を保存するには、 **適用**

   または

   クリック **保存して閉じる**.

## カスタムフォームのプレビュー

1. カスタムフォームの作成または編集を開始し、フィールドを追加します ( [フォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. クリック **プレビュー** フォームが使用されたときにどのように表示されるかを確認するには、左上隅で **プレビューを終了** をクリックして、フォームの編集に戻ります。