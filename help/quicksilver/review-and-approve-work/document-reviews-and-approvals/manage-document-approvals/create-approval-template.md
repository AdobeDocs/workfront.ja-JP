---
product-area: documents
navigation-topic: approvals
title: ドキュメントの承認ワークフローテンプレートの作成
description: 承認テンプレートを作成すると、承認プロセスを効率化できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 32%

---

# ドキュメントの承認ワークフローテンプレートの作成

Workfrontの設定領域で、標準ライセンスを持つユーザーは、再利用可能な承認テンプレートを作成できます。 作成した承認テンプレートは、オブジェクトの「ドキュメント」領域のアセットに適用できます。
>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。 標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>従来のWorkfrontストレージを使用して承認を管理する、あらゆるWorkfrontパッケージ</p>
<p>Adobeのクラウドストレージを使用して承認を管理する任意のワークフローパッケージ</p> </td> 
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

テンプレートを作成したら、そのテンプレートをオブジェクトの「ドキュメント」領域のドキュメントに適用して、Workfrontで正式なレビューと承認プロセスを開始できます。



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
