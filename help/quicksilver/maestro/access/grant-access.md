---
title: AdobeMaestro へのアクセスを許可
description: アクセス権を付与し、情報を共有する方法をAdobeMaestro で学びます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 90c730bbab2e62bcc60bee37272edb1219b2afb4
workflow-type: tm+mt
source-wordcount: '301'
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

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

現在、以下の前提条件が満たされている場合、組織内のすべてのユーザーが Maestro にアクセスできます。

* 組織がAdobeMaestro クローズ済みベータプログラムに登録されています。

  この新しいオファーについては、アカウント担当者にお問い合わせください。


Maestro を使用するために必要なアクセスについては、 [Adobeマエストロアクセスの概要](../access/access-overview.md).

>[!NOTE]
>
>Maestro には、ユーザや情報に関連するアクセスレベルや権限がありません。 Maestro が環境で有効になっているすべてのユーザは、他のユーザが Maestro に追加したすべての情報を表示、編集、および削除できます。

## Workfrontインスタンスのユーザーに対して Maestro を有効にします

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

組織が Maestro ベータプログラムに登録された後、レイアウトテンプレートを使用して、他のユーザー用の Maestro 領域を追加できます。

レイアウトテンプレートを使用して Maestro 領域を共有するには：

1. にログインします。 **Workfront** Workfront管理者として。

1. 次を追加： **マエストロ** アイコン ![](assets/maestro-icon.png) から **メインメニュー** の使用 **レイアウトテンプレート**.

   詳しくは、 [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Maestro にアクセスするユーザにレイアウトテンプレートを割り当てます。

   詳しくは、 [レイアウトテンプレートにユーザーを割り当てる](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   テンプレートに割り当てられたすべてのユーザは、メインメニューで Maestro にアクセスできるようになりました。

   ユーザーは、ワークスペース、レコードタイプ、レコード、およびフィールドの作成を開始できます。

<!--
## Share permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group, then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********) add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->