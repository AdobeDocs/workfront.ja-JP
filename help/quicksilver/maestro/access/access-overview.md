---
title: アクセスの概要
description: 組織内のすべてのユーザは、AdobeMaestro にアクセスできます。 現在、Maestro には、ユーザや情報に関連するアクセスレベルや権限はありません。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 50e6b09d626325ee2836dc0ebaf79fc1e8cc9da9
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

# アクセスの概要

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro にアクセスするには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

AdobeMaestro に対するアクセスレベルの制限はありません。

組織内のすべてのユーザは、アクセスレベルに関係なく、Maestro にアクセスできます。

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

## アクセス要件

AdobeMaestro を使用するには、次の条件を満たす必要があります。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。  </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル</p></td>
   <td> <p>任意</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者は、メインメニューの Maestro 領域をレイアウトテンプレートに追加する必要があります。</p> 
   <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">レイアウトテンプレートを使用したメインメニューのカスタマイズ</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--After we enable permissions, replace the section content above with this:

There are license and sharing permission restrictions to use Adobe Maestro capabilities. (*********** this should be the intro right under the title; also update the metadata with this when live*******)

You must have the following settings to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement*</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p>
   To create workspaces, users must have the following license: 
   <ul><li><p>New: Standard</p> </li>
   <li><p>Current: Worker or higher</p> </li></ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Maestro objects</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to workspaces and views that you did not create to edit, delete, and share them</p>
    <p>System Administrators can manage workspaces and views they did not create </p>
   <p>For information about sharing permissions for Maestro objects, see  
   <a href="../access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Maestro</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in the Main Menu to your layout template.</p> 
   <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*To find out your Workfront plan, license, or access level, contact your Workfront administrator. 

-->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


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

## アクセスを許可

Maestro のアクセス制御はありません。

任意の種類のライセンスを持つユーザは、Maestro にアクセスできます。

## 権限の付与

Maestro オブジェクトに関連付けられた権限はありません。

Maestro が環境で有効になっているすべてのユーザは、他のユーザが Maestro に追加したすべての情報を表示、編集、および削除できます。

<!--
Take out the text above and replace with this: 

For more information, see [Access overview](/help/quicksilver/maestro/access/access-overview.md)-->


