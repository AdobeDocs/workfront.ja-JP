---
product-area: projects
navigation-topic: approvals
title: 承認を表示
description: 承認プロセスを使用すると、プロジェクト、タスクおよびイシューに対する複数手順の承認を柔軟に作成できます。 Adobe Workfront管理者は、システム全体で一貫性を保つための承認プロセスを定義します。
author: Courtney
feature: Work Management
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 承認を表示

承認プロセスを使用すると、プロジェクト、タスクおよびイシューに対する複数手順の承認を柔軟に作成できます。 Adobe Workfront管理者は、システム全体で一貫性を保つための承認プロセスを定義します。

承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Workfrontでの作業への承認の関連付けについて詳しくは、 [新規または既存の承認プロセスと作業の関連付け](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>承認に関連付けられたオブジェクトへの表示またはそれ以上のアクセス権</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>承認に関連付けられたオブジェクトに対する権限を表示するか、それ以上に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Adobe Workfrontで承認を検索

Workfrontの複数の領域で承認を表示または管理できます。 様々な領域で承認を管理する方法について詳しくは、 [作業の承認](../../review-and-approve-work/manage-approvals/approving-work.md).

次の領域で承認を表示または管理できます。

* ホームエリア内

   * [ すべて ] または [ 承認 ] を表示するように選択すると、[ ホーム ] 領域に、承認待ちのすべてのプロジェクト、タスク、タスク、タイムシート、ドキュメント、およびアクセスが表示されます。
   * 自分が送信した承認は、[ 作業リスト ] の [Approvals I&#39;ve Submitted] セクションの [Home] 領域にも表示されます。 詳しくは、 [ホームエリアでの承認用に提出する作業をレビュー](#review-work-you-submit-for-approval-in-the-home-area) 」の節を参照してください。
   * 関連するプロジェクト、タスクまたは問題が「解決済み」、「保留中」、「クローズ済み」または「キャンセル済み」とマークされると、承認はホーム領域から削除されます。

   ホームの使用については、 [ホームを使い始める](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* プロジェクトのヘッダー、タスク、タスク、イシュー、ドキュメントまたは配達確認
* （プロジェクト、タスクまたはイシューの承認セクション）
* レポート内

   >[!NOTE]
   >
   >レポートから承認を決定することはできません。

   承認情報を含むプロジェクト、タスク、タスク、イシューまたはドキュメントの承認レポートを作成できます。

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## ホームエリアでの承認用に提出する作業をレビュー {#review-work-you-submit-for-approval-in-the-home-area}

1. 次をクリック： **ホーム** アイコン ![](assets/home-icon-30x29.png) Adobe Workfrontの左上隅に

   >[!NOTE]
   >
   >Workfront管理者は、お使いの環境のホームアイコンに次の変更を加えることができます。
   >
   >* 組織を説明するようにカスタマイズされた画像に置き換えます。 この場合、この記事に示すアイコンは異なります。
   >* リンクされたページを別のページに置き換えます。 この場合、 **メインメニュー** ![](assets/main-menu-icon.png) ページの右上隅にある「 **ホーム**.


1. 選択 **作業用リスト**」、「 **フィルター** ドロップダウンメニューで「 」を選択します。 **承認**.
1. を展開します。 **送信した承認** 」セクションで、送信した承認を確認します。

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## オブジェクトの承認ステータスの表示

オブジェクトの以下のセクションで、オブジェクトの承認ステータスを確認できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">更新 </td> 
   <td> <p>承認ステータスが発生した場合に、すべて表示します。 承認ステータスは、他のステータスと共に「 <strong>更新</strong> 」セクションに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">承認</td> 
   <td> <p>承認プロセスの各ステージや、承認者が承認を許可したかどうかなど、承認プロセスに関する詳細情報を表示します。</p> </td> 
  </tr> 
 </tbody> 
</table>

* [「更新」領域を使用して、承認ステータスを表示します](#use-the-updates-area-to-view-an-approval-status)
* [「承認」領域を使用して、承認ステータスを表示します](#use-the-approvals-area-to-view-an-approval-status)

### 「更新」領域を使用して、承認ステータスを表示します {#use-the-updates-area-to-view-an-approval-status}

プロジェクト、タスクまたはイシューで承認が開始されると、ステータスが **更新** タブを使用して、承認ステータスを示します。 新しいステータスは、承認プロセスを通じてオブジェクトが遷移するたびに表示されます。 これには、次のイベントが含まれます。

* オブジェクトに対して承認プロセスが開始されます。 ステータスが変更されると、承認プロセスが開始されます。
* オブジェクトが却下されました
* オブジェクトが承認されました 

>[!TIP]
>
>タスクに承認を適用すると、承認の更新がタスクの [ 更新 ] タブに表示されます。タスクが存在するプロジェクトの [ 更新 ] タブには表示されません。

### 「承認」領域を使用して、承認ステータスを表示します {#use-the-approvals-area-to-view-an-approval-status}

現在作業中のタスクや問題が承認プロセスのどこにあるかを明確に把握できます。 次の情報が表示されます。

* 承認プロセスのフェーズ
* どの承認者が既に承認していますか。
* どの承認者がまだ承認していませんか。

タスクまたはイシューが承認プロセスの現在の状態を確認するには：

1. 承認が関連付けられているプロジェクト、タスク、またはタスクに移動します。
1. 左側のパネルで、 **承認**. 最初に **さらに表示**.

   「承認」タブには、過去のすべての承認パスおよびステージに関する完全な情報が表示されます。 誰が承認を決定したか、承認がチーム、ジョブの役割、ユーザーに対して設定されているかを正確に確認できます。

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
