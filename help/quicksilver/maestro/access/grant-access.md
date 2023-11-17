---
title: AdobeMaestro へのアクセスを許可
description: アクセス権を付与し、情報を共有する方法をAdobeMaestro で学びます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 937498a68a994d19b0005d518d7e313c48961672
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# AdobeMaestro へのアクセスを許可

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro にアクセスするには、Workfrontのお客様である必要があります
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

次の前提条件が満たされている場合、組織内のすべてのユーザが Maestro にアクセスできます。

<!--the first requisite will be removed when we go to GA-->

* 組織がAdobeMaestro クローズ済みベータプログラムに登録されています。
* システム管理者は、レイアウトテンプレートを使用して [Maestro] 領域を [ メインメニュー ] に追加する必要があります。

  システム管理者を含むすべてのユーザに対して、Maestro はデフォルトでメインメニューに表示されません。

  詳しくは、 [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>Maestro には、ユーザや情報に関連するアクセスレベルや権限がありません。 Maestro が環境で有効になっているすべてのユーザは、他のユーザが Maestro に追加したすべての情報を表示、編集、および削除できます。

## メインメニューの Maestro 領域を他のユーザと共有します。

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

組織が Maestro ベータプログラムに登録された後、レイアウトテンプレートを使用して、すべてのユーザのメインメニューに Maestro 領域を追加できます。

1. にログインします。 **Workfront** Workfront管理者として。

1. 次を追加： **マエストロ** アイコン ![](assets/maestro-icon.png) から **メインメニュー** の使用 **レイアウトテンプレート**.

   詳しくは、 [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Maestro にアクセスするユーザにレイアウトテンプレートを割り当てます。

   詳しくは、 [レイアウトテンプレートにユーザーを割り当てる](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   テンプレートに割り当てられたすべてのユーザは、メインメニューで Maestro にアクセスできるようになりました。

   ユーザーは、ワークスペース、レコードタイプ、レコード、およびフィールドの作成を開始できます。

<!--

## Share permissions to a workspace

Only system administrators can access all workspaces in Maestro. As a system administrator, you must share a workspace with other users for them to view, manage, or contribute to it. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->