---
product-area: documents
navigation-topic: approvals
title: ドキュメントの承認ワークフローテンプレートの作成
description: 承認テンプレートを作成すると、承認プロセスを効率化できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 40%

---

# ドキュメントの承認ワークフローテンプレートの作成

Workfrontの設定領域で、標準ライセンスを持つユーザーは、再利用可能な承認テンプレートを作成できます。 作成した承認テンプレートは、プロジェクト、タスクまたはイシューのドキュメントエリアにあるアセットに適用できます。

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
ß

## 承認テンプレートの作成

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
   <td>ステージ名を追加します。 名前は、<em>初期審査</em>や<em>最終承認</em>などのより分かりやすいものに変更できます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1つの決定が必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限日までの勤務日</strong></td>
   <td>ステージがアクティブ化された後に承認の期限が切れるまでの作業日数を選択します。</td>
   </tr>
   </table>

1. （オプション）前の手順を繰り返して、必要に応じてステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で進みます。 必要な決定がすべて行われると、次のステージが始まり、前のステージがロックされます。

   ![&#x200B; ドキュメントの詳細](assets/new-stage.png)

1. 「**保存**」をクリックします。

テンプレートを作成したら、プロジェクト、タスクまたはイシューの「ドキュメント」エリアのドキュメントに適用して、Workfrontで正式なレビューと承認プロセスを開始できます。



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
