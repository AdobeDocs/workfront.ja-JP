---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトをコピー
description: プロジェクトをゼロから作成する代わりにコピーできます。コピーできるプロジェクトは一度に 1 つだけです。プロジェクトを一括でコピーすることはできません。
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: ht
source-wordcount: '764'
ht-degree: 100%

---

# プロジェクトをコピー

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

プロジェクトをゼロから作成する代わりにコピーできます。コピーできるプロジェクトは一度に 1 つだけです。プロジェクトを一括でコピーすることはできません。

>[!IMPORTANT]
>
>次の項目は、既存のプロジェクトから新規プロジェクトにコピーされません。
>
>* イシュー
>* 請求レート
>* 請求記録
>* メモ
>* 時間
>* プロジェクト間先行タスク
>* 予算計上時間数
>
>次の項目は、常に既存のプロジェクトから新しいプロジェクトにコピーされます。
>
>* タスク
>* テンプレート
>* リスク
>* キューの設定情報
>* ポートフォリオとプログラム
>* スコアカード
>* タスクのデフォルト情報（タスクのデフォルトの承認プロセス、タスクのデフォルトのカスタムフォーム）
>
> プロジェクトの元のタスクの日付が、新しいプロジェクトにコピーされます。タスクの日付を更新するには、プロジェクトの開始日または完了日を（スケジュールモードに応じて）変更する必要があります。タスクの制限により、プロジェクトの日付を変更できない場合があります。

## アクセス要件

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront ライセンス*</p> </td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>プロジェクトの作成<span>とコピー</span>ができるプロジェクトへの編集アクセス</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>プロジェクトに対する表示権限以上</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 単一のプロジェクトをコピーする

プロジェクトをコピーすると、元のプロジェクトの情報が新しいプロジェクトにコピーされます。また、コピー処理中に新しいプロジェクトにコピーしない項目を指定することもできます。

プロジェクトをコピーするには

1. コピーするプロジェクトに移動し、プロジェクト名の右側にある&#x200B;**その他**&#x200B;アイコン ![](assets/qs-more-menu.png) をクリックします。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   または

   プロジェクトリストまたはレポートに移動してプロジェクトを選択し、リストの上部にある&#x200B;**その他**&#x200B;アイコン ![](assets/qs-more-menu.png) をクリックします。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 「**コピー**」をクリックします。

1. 新しいプロジェクトの名前を更新します。

   デフォルトでは、新しい名前は、**`<Original project name>` のコピー**&#x200B;です。

   ![](assets/copy-project-box-nwe-350x276.png)

1. 新規プロジェクト用の&#x200B;**ステータス**&#x200B;を選択します。

   デフォルトでは、**ステータス**&#x200B;は元のプロジェクトのものと一致します。

1. （オプション）新しいプロジェクトにコピーしない項目の選択を解除します。次の表は、項目を選択解除した場合の動作を示しています。


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべて選択</td> 
      <td> <p>すべてのオプションを選択し、新しいプロジェクトから一覧表示されるすべてのフィールドとオブジェクトをクリアします。</p> <p><b>ヒント</b>

   「<strong>すべて選択</strong>」を選択解除して、すべての項目の選択を解除します。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">割り当て</td> 
      <td>すべてのプロジェクトとタスクの割り当てを削除</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況</td> 
      <td>すべてのタスクの進行状況を削除し、「新規」と表示します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムデータ</td> 
      <td> <p>プロジェクトのカスタムフォームの情報と、次の項目に関連付けられているカスタムフォームの情報を削除します。</p> 
       <ul> 
        <li>タスク</li> 
        <li>費用</li> 
        <li> ドキュメント</li> 
       </ul> <p><b>メモ</b>

   カスタムフォームは、タスク、費用、ドキュメントおよびプロジェクトに添付されたままですが、フォームのカスタムフィールドの情報は、新しいプロジェクトにはコピーされません。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td> <p>ドキュメントのバージョン、リンクされたドキュメント、フォルダーなど、「ドキュメント」タブ内のすべての項目を削除します。</p> <p>デフォルトでは、ドキュメントのプルーフと承認は別のプロジェクトにコピーできません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての先行タスク</td> 
      <td> <p>プロジェクト上のタスク間の先行タスク関係をすべて削除します。 </p> <p><b>ヒント</b>

   プロジェクト間の先行タスクは、選択されているかどうかに関係なく、新しいプロジェクトに転送されることはありません。 </p> </td>
   </tr>

<tr> 
      <td role="rowheader">予算計上時間数</td> 
      <td> <p>プロジェクトのビジネスケースのリソース計画エリアの予算計上時間数を、コピーしたプロジェクトから削除します。</p>

<b>メモ</b>

新規プロジェクトはシナリオプランナーのイニシアチブにリンクされていないため、シナリオプランナーを使用して予算計上された時間数が新規プロジェクトにコピーされることはありません。詳しくは、<a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">シナリオプランナーを使用したビジネスケースの予算計上リソース</a>を参照してください。
</tr></td>
    <tr> 
      <td role="rowheader">財務情報</td> 
      <td> <p>以下のエリアの情報を削除します。 </p> 
       <ul> 
        <li>プロジェクトの「財務」サブタブ</li> 
        <li> ビジネスケースにおける予定利益</li> 
        <li>すべてのタスクの財務情報<br></li> 
       </ul> <p>プロジェクトの「財務」サブタブに関して詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">プロジェクトの財務エリアで情報を管理</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td>タスクやプロジェクトに関連付けられているすべての承認を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知</td> 
      <td> タスクやプロジェクトに関連付けられているリマインダー通知を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>タスクやプロジェクトに関連する費用を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">権限</td> 
      <td> タスクやプロジェクトのすべてのユーザーに対する権限を削除します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**コピー**」をクリックして、プロジェクトのコピーを作成します。

   これにより、コピーしたプロジェクトに似た新しいプロジェクトが作成されます。

   タスクの割り当てのレビューやタイムラインの調整など、新しくコピーされたプロジェクトに対する変更を開始できます。
