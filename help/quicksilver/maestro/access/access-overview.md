---
title: アクセス権の概要
description: Adobe Workfront Planning を使用する場合、ライセンスと共有権限に制限があります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 7fe24704cead460762322b4f26bf37431e9744ca
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 33%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# アクセス権の概要

{{maestro-important-intro}}

Adobe Workfront Planning を使用する場合、ライセンスと共有権限に制限があります。

## アクセス要件

Adobe Workfront Planning を使用するには、次の設定が必要です：

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
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning ベータ版プログラムに登録されている必要があります。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス*</p></td>
   <td>
   <p>任意</p>
   <p>ワークスペースを作成するには、次のライセンスが必要です。</p>
   <ul>
   <li>
   新規：標準
   </li>
   <li>
   現在：Worker 以上
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセス レベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>自分が作成していないワークスペースやビューを編集、削除、共有したり、レコードタイプやレコードを作成、編集、削除したりするには、Contribute 以上の権限が必要です。</p>
    <p>システム管理者は、自分が作成しなかったワークスペースを管理できます。 </p>
    <p>システム管理者は、自分が作成していないビューを管理できません。 </p>
   <p>Workfront Planning オブジェクトのアクセス許可の共有については、次を参照してください：  
   <a href="../access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、<a href="/help/quicksilver/maestro/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


## メインメニューの計画エリアを他のユーザーと共有

<!--First, contact your account manager to obtain access to the current Workfront Planning closed beta program.-->

Workfront Planning ベータプログラムに登録したら、レイアウトテンプレートを使用して、すべてのユーザーのメインメニューに計画エリアを追加できます。

1. Workfront 管理者として **Workfront** にログインします。

1. を追加 **計画** アイコン ![](assets/maestro-icon.png) に **メインメニュー** の使用 **レイアウトテンプレート**.

   詳しくは、[レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)を参照してください。

1. Workfront Planning へのアクセス権を付与するユーザーにレイアウトテンプレートを割り当てます。

   詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

   これで、テンプレートに割り当てられたすべてのユーザーが、メインメニューからWorkfront Planning にアクセスできます。

   ユーザーは、ワークスペース、レコードタイプ、レコード、フィールドの作成を開始できます。

## アクセスを許可

Workfront Planning にはアクセス制御はありません。

あらゆるタイプのライセンスを持つユーザーは、Workfront Planning にアクセスできます。

オブジェクトへのアクセス権の付与について詳しくは、[カスタムアクセスレベルの作成と変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

## 権限の付与

作成したワークスペースおよびビューにユーザーがアクセスできるようにするには、それらのワークスペースおよびビューに対する権限をユーザーに付与する必要があります。

詳しくは、を参照してください [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

お使いのAdobe Workfrontのライセンスタイプは、Workfront Planning の権限と組み合わせて機能し、Workfront Planning オブジェクトの表示、投稿、管理へのアクセス権を付与します。

ライセンスの種類がWorkfront Planning オブジェクトのアクセス許可レベルに与える影響については、を参照してください。 [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).


