---
product-area: projects
navigation-topic: use-the-home-area
title: マイ更新エリアの使用
description: '[!UICONTROL マイ更新]エリアを使用して、決定を待っている承認や、参加している会話をすぐにレビューできます。'
author: Lisa
feature: Get Started with Workfront
exl-id: 809605a0-8c24-4873-b98f-504a158be022
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: ht
source-wordcount: '765'
ht-degree: 100%

---

# [!UICONTROL マイ更新]エリアの使用

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: there is a similar article like this in the "My Work" folder that is conditioned for Classic only)</p>
-->

[!UICONTROL マイ更新]エリアを使用して、決定を待っている承認や、参加している会話をすぐにレビューできます。

[!UICONTROL レビュー]ライセンスを持つユーザーの場合、[!UICONTROL マイ更新]エリアはデフォルトで[!UICONTROL メインメニュー]に表示され、[!UICONTROL マイ更新]エリアがデフォルトのランディングページになります。

[!DNL Adobe Workfront] ライセンスについて詳しくは、[[!DNL Adobe Workfront] ライセンスの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)を参照してください。

レビューとは異なるライセンスタイプを持つ場合、[!DNL Workfront] またはグループ管理者は、[!UICONTROL マイ更新]エリアをレイアウトテンプレートに追加して、メインメニューに表示する必要があります。詳しくは、[レイアウトテンプレートを使用した[!UICONTROL メインメニュー]のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>会話でタグ付けされたオブジェクトまたは承認の解決が必要なオブジェクト（プロジェクト、タスク、イシュー、ドキュメント）に対する表示権限またはそれ以上の権限</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>会話でタグ付けされたまたは承認の解決が必要なプロジェクト、タスク、イシュー、ドキュメントに対する [!UICONTROL View] 権限またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトのアクセスのリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプ、またはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

開始する前に、次の条件を満たす必要があります。

* [!UICONTROL レビュー]以外の [!DNL Workfront] ライセンスを持つ場合、[!DNL Workfront] またはグループ管理者は、レイアウトテンプレートを使用して[!UICONTROL マイ更新]エリアを[!UICONTROL メインメニュー]に追加し、ユーザーをそのテンプレートに割り当てる必要があります。

* レビューライセンスのユーザーは、デフォルトで[!UICONTROL メインメニュー]の[!UICONTROL マイ更新]エリアを表示できます。

## [!UICONTROL マイ更新]エリアへのアクセス

1. **[!UICONTROL メインメニュー]**&#x200B;で、**[!UICONTROL マイ更新]**&#x200B;をクリックします。

   ![](assets/access-my-updates-from-main-menu-reviewer-user-nwe-350x294.png)

   [!UICONTROL マイ更新]エリアが開きます。

   自分に割り当てられているアクセスの承認とリクエストは、ページの前半部の「マイ更新」の下に一覧表示されます。

   ![](assets/my-updates-mentions-for-reviwers-nwe-350x418.png)

1. （オプション）[!UICONTROL マイ更新]エリアの一番下までスクロールし、右向きの矢印をクリックすると、追加のページに表示される承認がさらに表示されます。

   >[!TIP]
   >
   >デフォルトでは、最初の 5 つの承認またはアクセスのリクエストが表示されます。その他のページには、残りの承認が表示されます。[!UICONTROL マイ更新]エリアには、最大 2000 件の承認を表示できます。

   ![](assets/pagination-for-my-updates-page-highlighted-nwe-350x78.png)

1. （オプション）「**[!UICONTROL マイ更新]**」セクションの右上隅にある&#x200B;**[!UICONTROL フィルター]**&#x200B;ドロップダウンメニュー![](assets/filter-nwepng.png)を展開し、以下から選択します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>自分に送信された、または別のユーザーによってデリゲートされた承認。承認のデリゲーションについて詳しくは、<a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">承認リクエストのデリゲート</a>を参照してください。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated Approvals]</strong></td> 
      <td>別のユーザーによってデリゲートされた承認。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Approvals]</strong></td> 
      <td> <p>自分に送信された承認。 </p> <p>アイテムの承認について詳しくは、<a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">作業の承認</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 承認前にアイテムを承認または却下したり、ドキュメントに対する変更を提案したりするには、次の手順を実行します。

   1. （オプション）承認決定の横にある&#x200B;**ドロップダウン**&#x200B;アイコン ![](assets/down-arrow-blue.png) （**[!UICONTROL 承認]**、**[!UICONTROL 変更]**、**[!UICONTROL 却下]**）をクリックし、コメントを追加して、「**[!UICONTROL 追加]**」をクリックします。

      または

      コメントを入力しない場合、「**[!UICONTROL スキップ]**」をクリックします。

      ![](assets/approval-decision-buttons-in-my-updates-with-comment-box-nwe-350x183.png)

      >[!NOTE]
      >
      >「[!UICONTROL 変更]」オプションは、ドキュメント承認の場合にのみ表示されます。

      選択したドロップダウンアイコンに応じて、アイテムは承認または却下されます。ドキュメントの承認の場合は、追加の変更を行うリクエストとともに承認されます。

      >[!TIP]
      >
      >決定にコメントを追加しない場合は、「**[!UICONTROL 承認]**」、「**[!UICONTROL 拒否]**」、または「**[!UICONTROL 変更]**」ボタンをクリックし、承認の決定を即座に行うことができます。
      >
      >
      >![](assets/approval-decision-buttons-in-my-updates-nwe-350x169.png)      >

      作業の承認について詳しくは、[作業の承認](../../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

1. **[!UICONTROL アクセス権の付与]**&#x200B;をクリックして、送信されたアクセスリクエストを付与

   または

   **[!UICONTROL アクセス権を変更]**&#x200B;ドロップダウンメニューを展開して、付与する前にリクエストされたアクセス権を変更します。

   ![](assets/grant-access-button-in-my-updates-nwe-350x224.png)

1. （オプション）「**[!UICONTROL 無視]**」をクリックすると、付与なしで承認リストからアクセスリクエストをクリアできます。
1. 承認の決定を下すことができない場合、「**[!UICONTROL 自分の承認をデリゲート]**」をクリックして送信された承認をデリゲートします。承認のデリゲートについて詳しくは、[承認リクエストのデリゲート](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)を参照してください。
1. 承認の下にある&#x200B;**[!UICONTROL メンション]**&#x200B;エリアまでスクロールします。ここでは、会話に含まれたすべての項目を表示できます。

   ![](assets/mentions-area-for-reviewers-nwe-350x191.png)

   >[!TIP]
   >
   >最初の 50 件のメンションがデフォルトで表示されます。

1. （オプション）「**[!UICONTROL 更新をさらに表示]**」をクリックして、さらに多くのメンションを表示します。
1. （オプション）「**[!UICONTROL 返信]**」をクリックし、コメントに返信し、回答を入力して、再び「**[!UICONTROL 返信]**」をクリックします。

   アイテムの更新について詳しくは、[作業の更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

1. （オプション）「**[!UICONTROL 現在のページをピン留め]**」をクリックして、[!UICONTROL マイ更新]エリアを上部ナビゲーションにピン留めします。
