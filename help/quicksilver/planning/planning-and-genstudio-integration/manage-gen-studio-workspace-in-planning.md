---
title: Adobe Workfront Planning でのGenStudio Workspaceの管理
description: 会社が両方の製品を購入し、GenStudio for Performance MarketingのインスタンスがAdobe Workfrontの会社のインスタンスと統合されている場合、Workfront Workspace はGenStudio Planning で使用できます。 Planning からGenStudioワークスペースを表示し、両方のシステムで情報を更新できます。
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 36cd1c23dfb6e01dc1016a6a12ae47e4f9172d20
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 17%

---

# Adobe Workfront Planning でのGenStudio Workspace の管理

<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

会社が両方の製品を購入し、GenStudio for Performance MarketingのインスタンスがAdobe Workfrontの会社のインスタンスと統合されている場合、Workfront Workspace はGenStudio Planning で使用できます。 Planning からGenStudioワークスペースを表示し、両方のシステムで情報を更新できます。

GenStudio for Performance Marketingの使用方法については、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront Planning でのGenStudio Workspace の管理に関する考慮事項

* Workfront Planning でAdobe GenStudio for Performance Marketing Workspace を表示するには、GenStudioを購入する必要があります。

  GenStudioについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

  GenStudioとWorkfrontの統合について詳しくは、[Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ ](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。

* Workfront ユーザーがWorkfront Planning でGenStudio Workspace を表示するには、GenStudioにアクセスできる必要があります。


## Workfront Planning でのGenStudio Workspace の管理

>[!NOTE]
>
>GenStudio Workspace を管理する前に、[Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ ](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。


1. システム管理者としてWorkfrontにログインします。
1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックして、「**[!UICONTROL Planning]**」をクリックします。

   Workfront計画のランディングページが開きます。

1. **その他のワークスペース** をクリックし、システムによって作成され、カードにGenStudio タグが付いているという表示を持つワークスペースを見つけます。

   ![ タグ付きGenStudio Workspace カード ](assets/genstudio-card-with-tag-highlighted.png)

1. **GenStudio Workspace カード** をクリックして、Workfront Planning でGenStudio Workspace を開きます。
1. デフォルトでは、次のGenStudio レコードタイプが作成され、Workfront Planning から表示されます。

   * キャンペーン
   * 製品
   * アクティベーション
   * チャネル
   * 地域

   GenStudioのレコードタイプには、最初にGenStudioで作成されたことを示す表示があります。

   ![ タグ付きGenStudio レコードタイプカード ](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. レコードタイプカードのいずれかをクリックして、そのタイプのレコードを表示します。

1. 次のいずれかの操作を行います。

   * **共有** をクリックし、**ビューリンクをコピー** をクリックしてレコードタイプへのリンクを共有するか、**現在のビューをエクスポート** をクリックしてファイルにエクスポートします。 書き出すことができるのは、テーブルビューのみです。

   * 「**+ ビュー**」をクリックして、GenStudio レコードタイプのビューを作成します。

   * 任意のビューからビュー要素を管理します。

     例えば、ビューのフィルター、グループ化、並べ替え、設定がある場合はそれを変更できます。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * テーブル表示またはタイムライン表示でレコードを追加します。

     レコードを作成するには、最初から作成するか、CSV ファイルまたは Excel ファイルを読み込む必要があります。

     詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

     レコードは、WorkfrontとGenStudioの両方から表示されます。

   * テーブル表示でレコードを削除します。

     削除されたレコードは、Workfrontから削除された場合、Workfront Planning のテーブルビューのごみ箱から復元できます。 詳しくは、[ 削除されたレコードの復元 ](/help/quicksilver/planning/records/restore-deleted-records.md) を参照してください
