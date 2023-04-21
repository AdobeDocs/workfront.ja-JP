---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 診断を使用して自動プロセスをトリガー化
description: 診断を使用して、時間ベースのスクリプト、再計算、電子メール通知など、自動化されたプロセスを手動でトリガーすることができます。
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 7%

---

# 診断を使用して自動プロセスをトリガー化

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

診断を使用して、時間ベースのスクリプト、再計算、電子メール通知など、自動化されたプロセスを手動でトリガーすることができます。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a> </td> 
   <td> <p>計画 </p>Workfront管理者である。 Workfront管理者について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</td> 
  </tr> 
 </tbody> 
</table>

## 診断を使用して自動プロセスをトリガー化

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **システム**&#x200B;を選択し、「 **診断**.
1. 次のいずれかのオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期限切れ通知の送信</td> 
      <td> <p>期限切れのタスクおよび問題に関する自動リマインダー通知を手動で送信します。 </p> <p>自動リマインダーの設定について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">自動リマインダーの設定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">早期通知の送信</td> 
      <td> <p>期限に近づいているタスクや問題に関する自動リマインダー通知を手動で送信します。</p> <p>自動リマインダーの設定について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">自動リマインダーの設定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダ通知の送信</td> 
      <td> <p>リマインダー通知を手動で送信します。 </p> <p>リマインダー通知の設定について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての POP アカウントを検査</td> 
      <td> <p>Workfrontにリンクされた POP アカウントに送信された新しい電子メールを確認します。 </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間の再計算</td> 
      <td> <p>ステータスが「現在」のWorkfront内のすべてのプロジェクトのタイムラインを再計算します。 </p> <p>自動または手動でプロジェクトのタイムラインを計算する方法の詳細については、「 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">プロジェクトタイムラインを再計算</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定の顧客報告書を復元</td> 
      <td>元々Workfrontで配信されていたレポートをデフォルトに戻し、 <strong>レポート</strong> 」セクションに表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートの生成</td> 
      <td>定期的なタイムシートプロファイルに基づいて、ユーザーのタイムシートを生成します。 このオプションを実行する必要があるのは、タイムシートプロファイルがユーザーに割り当てられた後に大幅に変更され、現在および将来のタイムシートが削除された後に限られます。</td> 
     </tr> 
    </tbody> 
   </table>
