---
title: アクセス権の概要
description: Adobe Workfrontの計画機能を使用する場合、ライセンスおよび共有権限に関する制限があります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 4c62b567fa1ebec37fc64831757eb67d4a048c1f
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# アクセス権の概要

{{maestro-important-intro}}

Adobe Workfrontの計画機能を使用する場合、ライセンスおよび共有権限に関する制限があります。

## アクセス要件

Adobe Workfrontの計画機能を使用するには、次の設定が必要です。

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
<p>組織は、Adobe Workfront Planning 機能クローズ済みベータプログラムに登録されている必要があります。 </p>
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
   <td> <p>計画機能オブジェクトに対するアクセス・レベル・コントロールはありません。</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>作成していないワークスペースやビューに対して、編集、削除、共有、レコードの種類やレコードの作成、編集、削除を行う権限を付与します。</p>
    <p>システム管理者は、自分が作成しなかったワークスペースを管理できます。 </p>
    <p>システム管理者は、自分が作成しなかったビューを管理できません。 </p>
   <p>機能オブジェクトの計画に関する権限の共有の詳細は、「  
   <a href="../access/sharing-permissions-overview.md">Adobe Workfrontの計画機能での共有権限の概要</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontの管理者を含むすべてのユーザーには、メインメニューの Maestro 領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、 <a href="/help/quicksilver/maestro/access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfrontのアクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## メインメニューの Maestro 領域を他のユーザと共有します。

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

組織がWorkfront Planning Capabilities Beta プログラムに登録されたら、レイアウトテンプレートを使用して、すべてのユーザーのメインメニューに Maestro 領域を追加できます。

1. にログインします。 **Workfront** Workfront管理者として。

1. 次を追加： **マエストロ** アイコン ![](assets/maestro-icon.png) から **メインメニュー** の使用 **レイアウトテンプレート**.

   詳しくは、 [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. レイアウトテンプレートを、Workfrontの計画機能にアクセスするユーザーに割り当てます。

   詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

   テンプレートに割り当てられたすべてのユーザは、メインメニューで Maestro にアクセスできるようになりました。

   ユーザーは、ワークスペース、レコードタイプ、レコード、およびフィールドの作成を開始できます。

## アクセスを許可

Workfrontの計画機能に対するアクセス制御はありません。

任意の種類のライセンスを持つユーザーは、 Workfront Planning 機能にアクセスできます。

Workfrontでのアクセス権の付与について詳しくは、 [カスタムアクセスレベルの作成と変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 権限の付与

ユーザーがアクセスできるようにするには、作成したワークスペースとビューに対する権限をユーザーに与える必要があります。

詳しくは、 [Adobe Workfrontの計画機能での共有権限の概要](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

Adobe Workfrontのライセンスの種類は、計画機能の権限と組み合わせて、計画機能のオブジェクトの表示、投稿、管理に対するアクセス権を付与します。

ライセンスの種類がプランニング機能オブジェクトの権限レベルに与える影響の詳細については、「 [Adobe Workfrontの計画機能を使用する際のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).


