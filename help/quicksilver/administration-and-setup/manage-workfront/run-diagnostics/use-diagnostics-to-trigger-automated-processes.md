---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 診断を使用して自動プロセスをトリガー
description: 診断を使用すると、時間ベースのスクリプト、再計算、メール通知など、自動化されたプロセスを手動でトリガーできます。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 379772f6bd1ed9448e6fd5feee956a931f65f69e
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 90%

---

# 診断を使用して自動プロセスをトリガー

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

診断を使用すると、時間ベースのスクリプト、再計算、メール通知など、自動化されたプロセスを手動でトリガーできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 診断を使用して自動プロセスをトリガー

1. Adobe Workfrontの右上隅にある **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**設定** ![ 歯車設定アイコン ](assets/gear-icon-settings.png) をクリックします。

1. **システム**&#x200B;を展開し、「**診断**」をクリックします。
1. 次のいずれかのオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期限切れ通知を送信</td> 
      <td> <p>期限切れのタスクおよびイシューに関する自動リマインダー通知を手動で送信します。 </p> <p>自動リマインダーの設定について詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">自動リマインダーを設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">早期通知を送信</td> 
      <td> <p>期限に近づいているタスクやイシューに関する自動リマインダー通知を手動で送信します。</p> <p>自動リマインダーの設定について詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">自動リマインダーを設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知を送信</td> 
      <td> <p>リマインダー通知を手動で送信します。 </p> <p>リマインダー通知の設定について詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知を設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての POP アカウントを確認</td> 
      <td>Workfront にリンクされた POP アカウントに送信された新規メールを確認します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムラインを再計算</td> 
      <td> <p>ステータスが「現在」の Workfront 内のすべてのプロジェクトのタイムラインを再計算します。 </p> <p>プロジェクトのタイムラインを一度に 1 プロジェクトずつ自動または手動で計算する方法について詳しくは、<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">プロジェクトタイムラインを再計算</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">デフォルトの顧客レポートを復元</td> 
      <td>Workfront で最初に配信されたデフォルトのレポートを復元し、すべてのユーザーの「<strong>レポート</strong>」セクションに表示されるようにします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートを生成</td> 
      <td>定期タイムシートプロファイルに基づいて、ユーザーのタイムシートを生成します。このオプションを実行する必要があるのは、タイムシートプロファイルがユーザーに割り当てられた後に大幅に変更され、現在および将来のタイムシートが削除された後に限られます。</td> 
     </tr> 
    </tbody> 
   </table>
