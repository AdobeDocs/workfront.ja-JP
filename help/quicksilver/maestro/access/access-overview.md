---
title: アクセスの概要
description: AdobeMaestro 機能を使用するためのライセンスと共有の許可制限があります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# アクセスの概要

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro にアクセスするには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](/help/quicksilver/maestro/maestro-overview.md).

AdobeMaestro 機能を使用するためのライセンスと共有の許可制限があります。

## アクセス要件

AdobeMaestro を使用するには、次の設定が必要です。

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
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>任意</p>
   ワークスペースを作成するには、ユーザーは次のライセンスを持っている必要があります。 
   <ul><li><p>新規：標準</p> </li>
   <li><p>現在：作業者以上</p> </li></ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Maestro オブジェクトに対するアクセスレベルコントロールはありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクトの権限</p></td>
   <td>
   <p>編集、削除、共有するために作成しなかったワークスペースやビューに、権限を付与するか、それ以上の権限を付与する</p>
    <p>システム管理者は、自分が作成しなかったワークスペースと表示を管理できます </p>
   <p>Maestro オブジェクトに対する権限の共有については、  
   <a href="../access/sharing-permissions-overview.md">AdobeMaestro での共有権限の概要</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>システム管理者は、メインメニューの Maestro 領域をレイアウトテンプレートに追加する必要があります。</p> 
   <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">レイアウトテンプレートを使用したメインメニューのカスタマイズ</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfrontのアクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


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

システム管理者以外のユーザーがアクセスできるようにするには、作成したワークスペースと表示に対して、システム管理者権限を付与する必要があります。

詳しくは、 [共有権限の概要 (AdobeMaestro)](/help/quicksilver/maestro/access/sharing-permissions-overview.md).


