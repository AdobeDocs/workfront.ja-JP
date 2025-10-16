---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: システムで追跡される更新の概要
description: Adobe Workfront は、オブジェクトの[!UICONTROL 更新]エリアのステータス情報をログに記録することで、特定のオブジェクトに対して行われるアクティビティを記録します。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 54%

---

# システムで追跡される更新の概要

<!-- Audited: 08/2025-->

[!DNL Adobe Workfront] は、オブジェクトの「[!UICONTROL &#x200B; 更新 &#x200B;] セクションにステータス情報を記録することで、特定のオブジェクトで発生しているアクティビティをキャプチャします。

「更新」セクションについて詳しくは、「[&#x200B; 更新」セクションの概要 &#x200B;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md) を参照してください。

[!UICONTROL 更新]エリアには、次のタイプの更新が含まれます。

* **ユーザー更新：**&#x200B;ユーザーが手動で入力したもの。コメント、返信、メモとも呼ばれます。 ユーザーの更新は、オブジェクトの「更新」セクションの「コメント」タブと「すべて」タブに表示されます。

  ユーザーの更新の設定について詳しくは、[ユーザー更新の環境設定の指](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)を参照してください。

  ![アップデート](assets/updates-qs-350x125.png)

* **システム更新：** システムによって自動的に行われたもの。システムの更新には、アイテムにどのような変更が発生したかを説明する簡単なメモが含まれます。 システムの更新は、「システム」アクティビティと、オブジェクトの「更新」セクションの「すべて」タブに表示されます。

  システム更新フィードおよびそれらを有効にする方法について詳しくは、[システム更新の設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)を参照してください。

  ![&#x200B; システム更新の例 &#x200B;](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## システムで追跡された更新に関する考慮事項

システムで追跡された更新は、更新エリアを持つすべてのオブジェクトで利用できるわけではありません。

* [!UICONTROL 更新]エリアは、次のオブジェクトで使用できます。

   * [!UICONTROL プロジェクト]
   * [!UICONTROL タスク]
   * [!UICONTROL イシュー]
   * [!UICONTROL ポートフォリオ]
   * [!UICONTROL プログラム]
   * [!UICONTROL ユーザー]
   * [!UICONTROL テンプレート]
   * [!UICONTROL テンプレート タスク]
   * [!UICONTROL チーム]
   * [!UICONTROL ドキュメント]
   * [!UICONTROL タイムシート]
   * [!UICONTROL ストーリー]

     [!DNL Workfront]では、ストーリーはタスクです。
   * [!UICONTROL 反復]
   * [!UICONTROL 目標]

     すべてのWorkfront パッケージにWorkfront Goals が含まれているわけではありません。 詳しくは、[Workfront Goals の使用要件](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md)を参照してください。
   * ボード上の[!UICONTROL カード]

     カードの更新について詳しくは、[ボードでの接続されたカードの使用](../../../agile/get-started-with-boards/connected-cards.md)を参照してください。

* [!DNL Workfront] は、次のオブジェクトに関するシステム更新を追跡しません。

   * [!UICONTROL チーム]
   * [!UICONTROL テンプレート]
   * [!UICONTROL テンプレート タスク]
   * アドホック[!UICONTROL カード]
   * [!UICONTROL イテレーション]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* ユーザーの更新は「コメント」タブに表示され、システムの更新は「システムアクティビティ」タブと「すべて」タブに表示されます。

  「システム」アクティビティまたは「すべて」のタブを持たないオブジェクトのリストについては、「[&#x200B; 更新」セクションの概要を参照してください &#x200B;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* システムの更新に返信を追加することはできません。 ただし、2024 年 4 月 11 日（PT）より前の従来のコメントエクスペリエンスのシステムアクティビティレコードに対して行われた返信は、読み取り専用として「システムアクティビティ」タブに入力されます。

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* [!DNL Workfront] 管理者は、[!UICONTROL 更新]エリアでシステムで追跡する必要のある変更の種類を定義できます。[!UICONTROL 更新]エリアを持つすべてのオブジェクトに、設定可能な[!UICONTROL 更新]フィードがあるとは限りません。次のオブジェクトには[!UICONTROL 更新]エリアがあり、システムで追跡された更新フィードを記録しますが、設定可能な更新フィードはありません。

   * [!UICONTROL ドキュメント]
   * [!UICONTROL タイムシート]
   * [!UICONTROL イテレーション]
   * [!UICONTROL 目標]


