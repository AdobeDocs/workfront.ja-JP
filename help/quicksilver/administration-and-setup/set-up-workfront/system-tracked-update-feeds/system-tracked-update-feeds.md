---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: システムで追跡された更新
description: Adobe Workfrontは、特定のオブジェクトの [!UICONTROL 更新] 領域。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 6%

---

# システムで追跡された更新

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] は、オブジェクトの [!UICONTROL 更新] 領域。

The [!UICONTROL 更新] 領域には、次の更新のタイプが含まれます。

* **ユーザーの更新：** ユーザーが手動で入力した。 コメント、返信、メモとも呼ばれます。

  ユーザーの更新の設定について詳しくは、 [ユーザーの更新の環境設定を構成する](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **システムの更新：** システムによって自動的に作成されます。 システム更新には、アイテムに発生した変更の種類を説明する簡単なメモが含まれています。

  システム更新フィードとそれらを有効にする方法について詳しくは、 [システム更新の構成](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## システムで追跡される更新に関する考慮事項

[ 更新 ] 領域を持つすべてのオブジェクトに対して、システムで追跡された更新を利用できるわけではありません。

* The [!UICONTROL 更新] 領域は、次のオブジェクトに対して使用できます。

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

     In [!DNL Workfront]ストーリーはタスクです。
   * [!UICONTROL 反復]
   * [!UICONTROL 目標]

     へのアクセス権を持つには、追加のライセンスが必要です。 [!UICONTROL 目標] 領域。 詳しくは、 [Workfront目標の使用要件](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL カード] 板の上で

     カードの更新について詳しくは、 [ボードでの接続済みカードの使用](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] は、次のオブジェクトのシステム更新を追跡しません。

   * [!UICONTROL チーム]
   * [!UICONTROL テンプレート]
   * [!UICONTROL テンプレート タスク]
   * アドホック [!UICONTROL カード]
   * [!UICONTROL イテレーション]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 新しいコメントエクスペリエンスと従来のコメントエクスペリエンスの違いを次に示します。

   * 新しいコメントエクスペリエンスを使用する場合、ユーザーの更新が「コメント」タブに表示され、システムの更新が「システムアクティビティ」タブに表示されます。

     新しいコメントエクスペリエンスについて詳しくは、 [新しいコメントエクスペリエンス](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * 従来のコメントエクスペリエンスを使用する場合、システムとユーザーの更新は 1 つの連続したフィードに表示されます。

   * 従来のコメントエクスペリエンスを使用する場合、ユーザーはデフォルトでシステムの更新を表示したり、表示しないように選択したりできます。 新しいコメントエクスペリエンスを使用する場合、システムの更新を無効にすることはできません。

     システム更新の表示を無効にする方法については、「 [システム更新を有効または無効にする](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) 記事内 [作業を更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfrontは、次のオブジェクトに関するシステム追跡された更新を記録しますが、表示を無効にするオプションはありません。

   * [!UICONTROL ポートフォリオ]
   * [!UICONTROL プログラム]
   * [!UICONTROL 反復]

* [!DNL Workfront] 管理者は、システムで追跡する必要のある変更の種類を [!UICONTROL 更新] 領域。 次のアイテムを持たないオブジェクトが存在する： [!UICONTROL 更新] 領域も設定可能 [!UICONTROL 更新] フィード。 次のオブジェクトには [!UICONTROL 更新] システムが追跡する更新フィードを取り込むが、設定可能な更新フィードを持たない領域：

   * [!UICONTROL ドキュメント]
   * [!UICONTROL タイムシート]
   * [!UICONTROL 反復]
   * [!UICONTROL 目標]


