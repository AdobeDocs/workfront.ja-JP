---
product-area: projects;templates
navigation-topic: manage-projects
title: プロジェクトをテンプレートとして保存する
description: プロジェクトをテンプレートとして保存プロジェクトレベルで「テンプレートとして保存」すると、ユーザーは UI でその内容を確認できます。このリンク先の別の記事がありますが、この記事の詳細はステップバイステップで説明します。 この機能は、プロジェクトとテンプレートの両方の領域にとどまる必要があります )」
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# プロジェクトをテンプレートとして保存する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

将来、プロジェクトが再び発生すると判断した場合は、その既存のプロジェクトからテンプレートを作成できます。 次に、テンプレートを再び使用して、類似の情報を含む将来のプロジェクトを作成したり、同じタイムラインや割り当てを既存のプロジェクトと共有したりできます。

## アクセス要件

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or 
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>テンプレートへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限以上 </p> <p>プロジェクトをテンプレートとして保存した後、テンプレートに対する管理権限を取得します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトをテンプレートとして保存する

1. テンプレートとして保存するプロジェクトに移動します。
1. 次をクリック： **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png)を、 **テンプレートとして保存**.
1. テンプレートの次の情報を指定します。

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
        <li> <p><strong>はい</strong>:他のユーザーは、テンプレートを見つけてプロジェクトに添付できます。</p> </li> 
        <li><strong>いいえ</strong>:他のユーザーはテンプレートを見つけられず、プロジェクトに添付できません。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>ドロップダウンリストを使用して、テンプレートに添付するカスタムフォームを選択します。 カスタムフォームが既にプロジェクトに関連付けられている場合は、それらのカスタムフォームのすべてのデータフィールドが表示されます。<br>1 つのテンプレートに最大 10 個のカスタムフォームを組み込むことができます。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **Formsを管理** フォームを削除または並べ替えるには テンプレート上のカスタムフォームの削除と並べ替えの方法について詳しくは、 [カスタムフォーム](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![](assets/save-as-template-first-step-350x159.png)

1. クリック **次のステップ。**
1. 内&#x200B;**オプション** 「 」セクションで、テンプレートから消去する情報の横にあるチェックボックスを選択します。

   ![](assets/save-as-template-options-step-350x109.png)

1. クリック **次のステップ。**
1. 内 **除外** 「 」セクションで、プロジェクトから除外するタスクを選択します。

   ![](assets/save-as-template-exclude-350x205.png)

1. クリック **テンプレートを終了して保存します。**

   テンプレートが使用可能なテンプレートのリストに表示され、既存のプロジェクトに添付したり、新しいテンプレートの作成に使用したりできます。
