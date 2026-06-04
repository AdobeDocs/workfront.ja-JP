---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトのコピー
description: プロジェクトをゼロから作成する代わりにコピーできます。 コピーできるプロジェクトは一度に 1 つだけです。 プロジェクトを一括でコピーすることはできません。
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/u2Ifl47l4tOd-g-WC-8Io96xmV8ut4RLvwzxyFBwmeA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d3382524-5489-431b-bde9-271ab257bc37id: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 755
ht-degree: 59%

---

# プロジェクトをコピー

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

ゼロからプロジェクトを作成するのではなく、既存のプロジェクトからプロジェクトをコピーできます。これにより、時間を節約できます。

プロジェクトを一括でコピーすることはできません。

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
> 元のプロジェクトのタスクの日付は、新しいプロジェクトにコピーされます。 タスクの日付を更新するには、プロジェクトの開始日または完了日を（スケジュールモードに応じて）変更する必要があります。 タスクの制限により、プロジェクトの日付を変更できない場合があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。
この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront パッケージ</p> </td>  
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront プラン</p> </td> 
   <td> <p>標準</p> 
   <p>プラン</p>
      </td> 
  </tr> 
     <td>アクセスレベル設定 </td> 
   <td> <p>プロジェクトの作成とコピー機能を使用したプロジェクトへのアクセス権の編集</p> </td> 
  </tr>

<td> <p>オブジェクト権限 </p> </td> 
   <td> <p>プロジェクトに対する表示権限以上</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
 Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## 考慮事項

* プロジェクトをコピーする場合、5分の処理制限があります。 プロジェクトに多数のドキュメントが添付されていて、コピーできない場合は、一部のドキュメントを削除して、もう一度試す必要がある場合があります。

## 単一のプロジェクトをコピーする

プロジェクトをコピーすると、元のプロジェクトの情報が新しいプロジェクトにコピーされます。 また、コピー処理中に新しいプロジェクトにコピーしない項目を指定することもできます。

プロジェクトをコピーするには

{{step1-to-projects}}

1. プロジェクト リストからコピーするプロジェクトを選択し、プロジェクト名の右側にある&#x200B;**詳細** アイコン ![詳細メニュー](assets/more-icon.png)をクリックします。

   または

   プロジェクトのリストまたはレポートに移動してプロジェクトを選択し、リストの上部にある&#x200B;**詳細** アイコン ![詳細メニュー](assets/more-icon.png)をクリックします。

1. **詳細** ドロップダウンメニューで、**コピー**&#x200B;をクリックします。 「[ プロジェクト名&#x200B;]**のコピー」ダイアログボックスが表示されます。**

1. （オプション） **プロジェクト名**&#x200B;を更新します。 デフォルトでは、新しい名前は&#x200B;**元のプロジェクト名[のコピー]**&#x200B;です。

   ![ プロジェクトボックスをコピー](assets/copy-of-project-box.png)

1. **ステータス**&#x200B;を選択します。 デフォルトでは、元のプロジェクトのステータスが選択されています。

1. （オプション）新しいプロジェクトにコピーしない項目の選択を解除します。 次の表は、項目を選択解除した場合の動作を示しています。


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべて選択</td> 
      <td> <p>すべてのオプションを選択し、新しいプロジェクトから一覧表示されるすべてのフィールドとオブジェクトをクリアします。 </p>

   <p> このオプションの選択を解除すると、すべての項目が選択解除されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">割り当て</td> 
      <td>プロジェクトとタスクのすべての割り当てを削除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況</td> 
      <td>すべてのタスクの進行状況を削除し、新規として表示します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムデータ</td> 
      <td> <p>プロジェクトのカスタムフォームの情報と、次の項目に関連付けられているカスタムフォームの情報を削除します。</p> 
       <ul> 
        <li>タスク</li> 
        <li>費用</li> 
        <li> ドキュメント</li> 
       </ul> 
      <p>カスタムフォームは、タスク、費用、ドキュメント、プロジェクトに添付されたままですが、フォームのカスタムフィールド内の情報は新しいプロジェクトにコピーされません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td> <p>ドキュメントのバージョン、リンクされたドキュメント、フォルダーなど、「ドキュメント」タブのすべての項目を削除します。</p> <p>デフォルトでは、ドキュメントのプルーフと承認は別のプロジェクトにコピーできません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての先行タスク</td> 
      <td> <p>プロジェクト上のタスク間の先行タスク関係をすべて削除します。 </p> <p>

   プロジェクト間の先行タスクは、選択されているかどうかに関係なく、新しいプロジェクトに転送されることはありません。 </p> </td>
   </tr>

<tr> 
      <td role="rowheader">予算計上時間数</td> 
      <td> <p>プロジェクトのビジネスケースのリソース計画エリアの予算計上時間数を、コピーしたプロジェクトから削除します。</p> 
    <p>
   新規プロジェクトはシナリオプランナーのイニシアチブにリンクされていないため、シナリオプランナーを使用して予算計上された時間数が新規プロジェクトにコピーされることはありません。 詳しくは、<a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">シナリオプランナーを使用したビジネスケースの予算計上リソース</a>を参照してください。</p>
   </tr></td>
    <tr> 
      <td role="rowheader">財務情報</td> 
      <td> <p>以下のエリアの情報を削除します。 </p> 
       <ul> 
        <li>プロジェクトの「財務」サブタブ</li> 
        <li> ビジネスケースにおける予定利益</li> 
        <li>すべてのタスクの財務情報<br></li> 
       </ul> <p>プロジェクトの財務サブタブについて詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref"> プロジェクトの財務エリアの情報の管理</a>を参照してください。</p> </td> 
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

1. 「**プロジェクトをコピー**」をクリックします。 コピーされたプロジェクトが作成されます。
