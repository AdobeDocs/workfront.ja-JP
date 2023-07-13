---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトからテンプレートを作成
description: 既存のプロジェクトをテンプレートとして保存する際に、テンプレートを作成できます。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# プロジェクトからテンプレートを作成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

既存のプロジェクトをテンプレートとして保存する際に、テンプレートを作成できます。

既存のプロジェクトをテンプレートとして保存した後、新しいテンプレートを使用して新しいプロジェクトを作成できます。 これにより、プロジェクト作成プロセスが簡素化され、迅速に実行されます。

>[!NOTE]
>
>プロジェクトをテンプレートとして保存する場合、タスクの実際の日付とプロジェクトの実際の日付は、テンプレートに対して保存されません。
>
>テンプレートとそのタスクには、実際の日付は含まれず、タスクの開始日と終了日（将来のプロジェクトが開始する日から）を示します。 テンプレートを使用して将来のプロジェクトを作成する場合、プロジェクトは実際の日付を受け取ります。 詳しくは、 [プロジェクトの作成](../create-projects/create-project.md).

## アクセス要件

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
   <td> <p>テンプレートへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限以上 </p> <p>テンプレートの作成後、テンプレートに対する管理権限を取得します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトからテンプレートを作成

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

 
