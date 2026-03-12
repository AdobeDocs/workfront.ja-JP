---
product-area: documents
navigation-topic: approvals
title: ドキュメント用の承認ワークフローテンプレートの作成
description: 承認テンプレートを作成すると、承認プロセスを効率化できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
source-git-commit: 6d6ac026bb2aa10ba3e678fb7e0f32dc95d0405f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 47%

---

# ドキュメント用の承認ワークフローテンプレートの作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

Workfrontの「設定」領域で、Standard ライセンスを持つユーザーは、再利用可能な承認テンプレートを作成できます。 作成した承認テンプレートは、プロジェクト、タスクまたはイシューのドキュメントエリアにあるアセットに適用できます。

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>プラン</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++




## 実稼動環境での承認テンプレートの作成

{{step-1-to-setup}}

1. 左パネルで&#x200B;**レビューと承認**／**承認テンプレート**&#x200B;をクリックします。
1. ページの右側で「**新規テンプレート**」をクリックします。
1. 次の情報を指定します。

   | テンプレート名 | このテンプレートの名前を入力していきます。 |
   |----------------------------|---|
   | **（オプション）期間** | 期間を日数で入力します。承認期限は、テンプレートがアセットに適用された後で、このフィールドから計算されます。 |
   | **承認者またはレビュアーの追加** | ユーザーまたはチームの名前を入力していき、それらをレビュアーまたは承認者として指定します。 |

1. 「**保存**」をクリックします。



<div class="preview">

## プレビュー環境での承認テンプレートの作成

{{step-1-to-setup}}

1. 左パネルで&#x200B;**レビューと承認**／**承認テンプレート**&#x200B;をクリックします。
1. ページの右側で「**新規テンプレート**」をクリックします。

1. 次の詳細を入力します。

   <table>
     <tr>
   <td><strong>テンプレート名</strong></td>
   <td>テンプレート名を追加します。 </td>
   </tr>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、「最初のレビュー」や「<em> 最終承認 </em> など、よりわかりやすい名前 <em> 変更 </em> きます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>ユーザー名またはチーム名の入力を開始して、承認者またはレビュアーとして追加します。 レビュー担当者のみが存在する場合、レビュー担当者に通知され、レビューを完了するオプションが提供されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1 つの決定が必要（オプション）</strong></td>
   <td>最初に決定を行ったユーザーがステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限日までの勤務日</strong></td>
   <td>ステージをアクティブ化してから承認の期限が切れるまでの作業日数を選択します。</td>
   </tr>
   </table>

1. （オプション）必要に応じて、前の手順を繰り返して追加のステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で続行されます。 必要な決定がすべて行われると、次のステージが開始され、前のステージがロックされます。

   ![&#x200B; ドキュメントの詳細 &#x200B;](assets/new-stage.png)

1. 「**保存**」をクリックします。

作成したテンプレートは、プロジェクト、タスクまたはイシューの「ドキュメント」領域のドキュメントに適用して、Workfrontでの正式なレビューと承認プロセスを開始できます。

</div>


<!-- Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)-->
