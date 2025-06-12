---
product-area: projects;templates
navigation-topic: manage-projects
title: プロジェクトをテンプレートとして保存
description: プロジェクトを「プロジェクトレベルでテンプレート templateSave として保存すると、ユーザーはそれを UI で確認できます。これにはリンクされている別の記事があり、より詳しく（段階的に）説明されています。この機能はプロジェクトとテンプレートの両方のエリアに存在する必要があります。）」
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 62%

---

# プロジェクトをテンプレートとして保存

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<div class="preview">

このページで強調表示されている情報は、まだ一般公開されていない機能を示しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 プレビューリリースから 1 週間後に、すべてのお客様の実稼動環境でも同じ機能が使用できるようになります。

詳しくは、[ インターフェイスの最新化 ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md) を参照してください。

</div>

プロジェクトが将来再び発生することが決定した場合は、その既存のプロジェクトからテンプレートを作成できます。次に、テンプレートを再度使用して、同様の情報を含む可能性がある、または既存のプロジェクトと同じタイムラインや割り当てを共有する可能性のある今後のプロジェクトを作成できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準 </p>
   または 
   <p>現在：プラン </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限またはそれ以上の権限 </p> <p>プロジェクトをテンプレートとして保存した後、テンプレートに対する管理権限を取得します。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## プロジェクトをテンプレートとして保存

プロジェクトをテンプレートとして保存する方法は、実稼動環境とプレビュー環境で異なります。

### 実稼動環境でプロジェクトをテンプレートとして保存する

1. テンプレートとして保存するプロジェクトに移動します。
1. **その他** メニュー ![ その他アイコン ](assets/qs-more-icon-on-an-object.png) をクリックしてから、**テンプレートとして保存** をクリックします。
1. テンプレートに次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>テンプレートの名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>テンプレートの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>はい</strong>：他のユーザーがテンプレートを見つけてプロジェクトに添付することができます。</p> </li> 
        <li><strong>いいえ</strong>：他のユーザーはテンプレートを見つけることができず、プロジェクトに添付できません。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>ドロップダウンリストを使用して、テンプレートに添付するカスタムフォームを選択します。カスタムフォームがすでにプロジェクトに関連付けられている場合は、それらのカスタムフォームのデータフィールドがすべて表示されます。<br>1 つのテンプレートに最大 10 個のカスタムフォームを含めることができます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**フォームの管理**」をクリックして、フォームを削除または並べ替えます。テンプレートのカスタムフォームを削除して並べ替える方法については、[カスタムフォーム](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)を参照してください。

   ![](assets/save-as-template-first-step-350x159.png)

1. 「**次の手順**」をクリックします。
1. 「**オプション**」セクションで、テンプレートから消去する情報の横にあるチェックボックスを選択します。

   ![](assets/save-as-template-options-step-350x109.png)

1. 「**次の手順**」をクリックします。
1. **除外**&#x200B;セクションで、プロジェクトから除外するタスクを選択します。

   ![](assets/save-as-template-exclude-350x205.png)

1. 「**完了してテンプレートを保存**」をクリックします。

   テンプレートが使用可能なテンプレートのリストに表示され、既存のプロジェクトに添付することも、新しいプロジェクトの作成に使用することもできます。


<div class="preview">

### プレビュー環境でプロジェクトをテンプレートとして保存する

1. テンプレートとして保存するプロジェクトに移動します。
1. **その他** メニュー ![ その他アイコン ](assets/qs-more-icon-on-an-object.png) をクリックしてから、**テンプレートとして保存** をクリックします。
1. **テンプレートとして保存** セクションで、テンプレートの次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">テンプレート名</td> 
      <td>テンプレートの名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>テンプレートの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>はい</strong>：他のユーザーがテンプレートを見つけてプロジェクトに添付することができます。</p> </li> 
        <li><strong>いいえ</strong>：他のユーザーはテンプレートを見つけることができず、プロジェクトに添付できません。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>ドロップダウンリストを使用して、テンプレートに添付するカスタムフォームを選択します。カスタムフォームがすでにプロジェクトに関連付けられている場合は、それらのカスタムフォームのデータフィールドがすべて表示されます。<br>1 つのテンプレートに最大 10 個のカスタムフォームを含めることができます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 左側のパネルで **カスタムForms** をクリックして、フォームを削除または並べ替えます。

   フォームを並べ替えるには、フォームを正しい順序でドラッグ&amp;ドロップします。
フォームを削除するには、フォームを選択して「**削除**」をクリックします。 **キャンセル** をクリックして、選択したフォームを削除します。

   ![ 「テンプレートとして保存」ボックスのカスタムフォーム領域 ](assets/custom-forms-ara-in-save-as-template-box.png)

1. 必要に応じて、添付されたカスタムフォームの情報を更新します。 情報がテンプレートに転送されます。

1. 左側のパネルセクションで **オプション** をクリックし、テンプレートに転送する情報の横にあるチェックボックスを選択します。 選択解除された項目は、テンプレートに転送されません。 デフォルトでは、すべてのオプションの選択は解除されています。

   ![ 「テンプレートとして保存」ボックスの「オプション」領域 ](assets/options-area-in-save-as-template-box.png)

1. 左側のパネルで **除外** をクリックし、プロジェクトから除外するタスクを選択します。 デフォルトでは、すべてのタスクの選択は解除されています。

   ![ 「テンプレートとして保存」ボックスの「除外」領域 ](assets/exclude-area-save-as-template-box.png)

1. 「**完了してテンプレートを保存**」をクリックします。

   テンプレートが使用可能なテンプレートのリストに表示され、既存のプロジェクトに添付することも、新しいプロジェクトの作成に使用することもできます。

</span>