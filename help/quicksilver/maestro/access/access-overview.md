---
title: アクセス権の概要
description: Adobe Workfront Planning を使用する場合は、ライセンスと共有の権限に関する制限があります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 7fe24704cead460762322b4f26bf37431e9744ca
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# アクセス権の概要

{{maestro-important-intro}}

Adobe Workfront Planning を使用する場合は、ライセンスと共有の権限に関する制限があります。

## アクセス要件

Adobe Workfront Planning を使用するには、次の設定が必要です。

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
<p>組織がAdobe Workfront Planning ベータプログラムに登録されている必要があります。 </p>
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
   現在：作業者以上
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセスレベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>作成していないワークスペースやビューに対して、編集、削除、共有、レコードの種類やレコードの作成、編集、削除を行う権限を付与します。</p>
    <p>システム管理者は、自分が作成しなかったワークスペースを管理できます。 </p>
    <p>システム管理者は、自分が作成しなかったビューを管理できません。 </p>
   <p>Workfront Planning オブジェクトの権限の共有については、  
   <a href="../access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューの「計画」領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、 <a href="/help/quicksilver/maestro/access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfrontのアクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## メインメニューの「計画」領域を他のユーザーと共有します。

<!--First, contact your account manager to obtain access to the current Workfront Planning closed beta program.-->

組織がWorkfront Planning ベータ・プログラムに登録されたら、レイアウト・テンプレートを使用して、すべてのユーザーのメイン・メニューに「計画」領域を追加できます。

1. にログインします。 **Workfront** Workfront管理者として。

1. 次を追加： **計画** アイコン ![](assets/maestro-icon.png) から **メインメニュー** の使用 **レイアウトテンプレート**.

   詳しくは、 [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Workfront Planning へのアクセス権を持つユーザーに、レイアウトテンプレートを割り当てます。

   詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

   テンプレートに割り当てられたすべてのユーザーが、メインメニューでWorkfront Planning にアクセスできるようになりました。

   ユーザーは、ワークスペース、レコードタイプ、レコード、およびフィールドの作成を開始できます。

## アクセスを許可

Workfront Planning のアクセス制御はありません。

任意の種類のライセンスを持つユーザーは、Workfront Planning にアクセスできます。

Workfrontでのアクセス権の付与について詳しくは、 [カスタムアクセスレベルの作成と変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 権限の付与

ユーザーがアクセスできるようにするには、作成したワークスペースとビューに対する権限をユーザーに与える必要があります。

詳しくは、 [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

Adobe Workfrontのライセンスの種類は、Workfront Planning の権限と組み合わせて、Workfront Planning オブジェクトの表示、投稿、管理に対するアクセス権を付与します。

ライセンスの種類がWorkfront Planning オブジェクトの権限レベルに与える影響については、 [Adobe Workfront Planning を使用する際のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).


