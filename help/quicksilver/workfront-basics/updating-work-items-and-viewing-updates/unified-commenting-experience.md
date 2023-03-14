---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Unified Commenting Experience
description: 新しい Unified Commenting Experience は次のようになります
author: Nolan
feature: Get Started with Workfront
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 1%

---


# 新しいコメントエクスペリエンス

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Adobe Workfrontのコメントエクスペリエンスのアップデートは現在開発中です。 この更新には、新しいインターフェイス、新機能、および選択したオブジェクトの更新セクションのパフォーマンスの向上が含まれます。

<!--drafted for commenting experience on issues: 

>[!NOTE]
>
>The new commenting experience is not available for other areas of Workfront that displays updates. For example, the new experience is not availabe for the following areas:
>
>* Home
>* Summary panel in a list
>* Summary panel in a timesheet
>
>The new commenting experience is only available for the Updates section of select objects. 
>
>For information about what objects include the Updates section, see [Updates tab overview](../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md). 
-->

現在、Adobeの Workfont 目標でのみ実装されていますが、この新しいエクスペリエンスは、Workfrontの「更新」セクションを持つすべてのオブジェクトで徐々に使用できるようになり、後で他のAdobe Experience Cloudアプリケーションにも拡張されます。

<!--when we release to Preview for issues with a toggle, we need to remove the last sentence above and replace it with this: 

The new commenting experience is currently supported for the following objects in Workfront:

By default, in the Preview and Production environments for all customers: 

* Goals

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

    For more information about managing updates for goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md). 


<div class="preview">

By enabling the Beta toggle, in the Preview environment: 

* Issues

    For more information about managing updates for other objects, including issues, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

</div>

This new experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.
-->

## 機能

新しいコメントエクスペリエンスには、既存の更新ストリームの改善と変更が含まれます。

>[!IMPORTANT]
>以下に示す統合コメントエクスペリエンスの機能は、現在、Adobe Workfront目標でのみ使用できます。

* **コメントの作成**

   新しいコメントを作成し、リッチテキストで書式設定し、他のユーザーに通知するタグを付けることができます。 コメントの作成について詳しくは、 [目標のコメントを管理](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md).

* **コメントへの回答**

   コメントに対して「いいね！」を付けたり、新しいコメントをスレッド内で返信したりして、元のコメントとオブジェクトの所有者に通知できます。

* **システムアクティビティ**

   オブジェクトに対してシステムが生成した更新が、更新タブで行ったコメントとは別に表示されるようになりました。 システムアクティビティストリームの表示の詳細については、次のステップ 11 を参照してください： [目標のコメントを管理](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md).

<!-- When releasing this to Issues - preview with 23.2 - remove all the content above in the "Features" section and replace it with this: 

One of the main differences between the current and the new commenting experience is the separation of user-submitted comments and system activity updates with the introduction of the System Activity tab. There are no changes to the way system-generated activity updates function.

Among the improvements included in the new commenting experience are the following:

* Better, faster performance 
* Real-time updates
* Edit comments after submitting them. 

The following table illustrates the features that will be available in the new commenting experience as well as their availability now in areas where they are supported: 

<table>
  <tr>
   <td><strong>Feature </strong>
   </td>
   <td><strong>Exists in old commenting experience </strong>
   </td>
   <td><strong>Exists in Beta version of the new commenting experience </strong>
   </td>
   <td><strong>Will be introduced in the new commenting experience </strong>
   </td>
   <td><strong>When will be introduced in the new commenting experience </strong>
   </td>
   <td><strong>In research </strong>
   </td>
  </tr>
  <tr>
   <td>Create/read/reply/delete comments 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Rich text (exludes quoting and emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
 <tr>
   <td>Rich text (quoting and emojis)
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> Q2, 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>

   <td>React to comments (Like) 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Attach images to comments 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Tag people in comments 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Remove people from the thread 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Comments that are private to a company 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Undo posting of a comment 
   </td>
   <td>✓ 
   </td>
   <td>Replaced with edit comment 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Turn off system updates 
   </td>
   <td>✓ 
   </td>
   <td>Replaced with Activity tab 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Edit comments 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Saving comment drafts when navigating away from the page 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>See new comments in real time 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Log time 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Edit custom form 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Ability to edit status, condition, commit date while commenting 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Copy thread link 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copy comment link 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Quote comment text 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copy body text 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Resolve comments 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q3, 2023 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Search in comments 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q3, 2023 
   </td>
   <td>✓ 
   </td>
  </tr>
</table>

-->
