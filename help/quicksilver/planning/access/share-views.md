---
title: ビューの共有
description: Adobe Workfront Planning を使用する際に、他のユーザーとビューを共有して、共同作業を確実に行えます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 28%

---


# ビューを共有

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning でレコードを操作する際に、他のユーザーとビューを共有して、共同作業を確実に行えます。

>[!IMPORTANT]
>
>* 他のユーザーにワークスペースの権限を付与しても、レコードタイプページのビューに対する権限は付与されません。他のユーザーと共有するには、レコードタイプのページ内の個々のビューに権限を付与する必要があります。
>
>* ビューに権限を付与しても、レコードを表示する権限は変更されません。 レコードの権限は、ワークスペースを共有することで付与されます。
>
>* ビューを共有すると、そのビューのすべての要素にアクセスする権限が他のユーザーに与えられます。 例えば、ビューに管理権限を付与すると、グループ化、フィルター、並べ替え、バーの外観を変更できます。


次のエンティティでビューを共有できます。

* 内部的には、Workfront ユーザー、グループ、<span class="preview"> チーム、会社、担当業務 </span>
* 公開（Workfront以外のユーザーを使用）

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>権限リクエストからビューに権限をリクエストし、付与できるようにするには、組織をAdobeの Unified Experience にオンボーディングする必要があります。 </p>
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
   <td>  <p>ビューに対する権限を管理</p>  
   <p>ビューを公開して共有できるのは、ワークスペースに対する管理権限を持つユーザーのみです。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<!--OLD: 

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
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

+++

## ビューを共有する際の考慮事項

* ビューに対する表示権限または管理権限を、Workfrontの内部ユーザーに付与できます。

* 管理権限を持つユーザーは、表示設定の変更、共有、複製、削除を行うことができます。

* パブリック リンクを使用して、組織外のユーザーとビューを共有できます。

* ビューを公開して共有した場合、リンクには、会社外のユーザーが限られた期間（有効期限が示す）アクセスできます。 共有ビューを表示するためにログインする必要はありません。

* ビューへのアクセス権を持つ組織外のユーザーは、他のビューの作成、共有ビューの編集、ビュー内のレコード情報の追加、削除、編集を行うことはできません。

## ビューへの権限を内部的に共有

作成したビュー、または管理権限を持つビューを、Workfrontでユーザー、グループ、<span class="preview"> チーム、会社、担当業務 </span> と共有できます。

>[!NOTE]
>
>システム管理者は、自分で作成しなかったビューは表示または共有できません。自分と共有されたビューのみにアクセスしたり、ビューのみを共有したりできます。
>
>システム管理者は、ビューに対する管理権限のみを持つことができます。

{{step1-to-planning}}

1. 共有するビューのワークスペースを開き、レコードタイプカードをクリックします。

   レコードタイプページが開きます。

1. ビュータブで、共有するビューにポインタを合わせ、ビュー名の右にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックしたあと、「**共有**」をクリックします。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   「**内部共有**」タブは、デフォルトで選択されている必要があります。

1. （オプション） **アクセスできるユーザー** 領域で、次のオプションから選択します。

   * **招待されたユーザーのみがアクセスできます**：ビューを共有するユーザー、グループ、<span class="preview"> チーム、会社または担当業務 </span> を指定する必要があります。 これはデフォルトのオプションです。
   * **ワークスペース内の全員が表示できます**：ワークスペースに対する表示以上の権限を持つすべてのユーザーが、ビューにアクセスできます。

1. 「**表示アクセス権の付与先**」フィールドに、ユーザー、グループ、<span class="preview"> チーム、会社または担当業務の名前の入力を開始し </span> リストに表示されたらクリックします。

   <div class="preview">

   ![](assets/sharing-a-view-ui-with-groups.png)

   </div>

1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

     システム管理者は、共有されたビューに対する管理権限を常に受け取ります。

1. 「**リンクをコピー**」をクリックして、ビューへのリンクをクリップボードにコピーします。
1. **保存**&#x200B;をクリックします。

   ビューが人物アイコン ![](assets/view-shared-with-others-people-icon.png) で更新され、ビューが他のユーザーと共有されたことを示します。

   >[!TIP]
   >
   >ユーザーまたはグローバル アイコンのないビューは、ユーザーが作成したビューであり、他のユーザーと共有されていません。 非共有ビューは、自分にのみ表示されます。

1. コピーしたリンクを他のユーザーと共有します。リンクを受け取ったユーザーが、レコードタイプのページにアクセスして、選択したビューで表示するには、ユーザーがアクティブユーザーであり、Workfront にログインしている必要があります。

## ビューに対する権限のパブリックへの共有

自分が作成したビューや、管理権限を持つビューを、Workfront ライセンスを持たず、組織外の可能性があるユーザーと共有できます。

>[!IMPORTANT]
>
>ワークスペースのビューを公開して共有できるのは、ワークスペースに対する管理権限を持つユーザーのみです。


Workfront Planning でビューをパブリックに共有するには、次の手順に従います。

{{step1-to-planning}}

1. 共有するビューのワークスペースを開き、レコードタイプカードをクリックします。

   レコードタイプページが開きます。

1. ビュータブで、共有するビューにポインタを合わせ、ビュー名の右にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックしたあと、「**共有**」をクリックします。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. **公開共有** をクリックします。

   ![](assets/public-sharing-tab-for-views.png)

1. **公開リンクを作成** 設定を有効にします。

   リンクが使用可能になります。 これは公開リンクです。 共有すると、組織外のユーザーを含め、リンクを持つすべてのユーザーがレコードタイプページにアクセスし、ページ上のレコードとフィールドを表示できます。

1. **リンクをコピー** アイコン ![](assets/copy-link-view.png) をクリックして、リンクをクリップボードにコピーします。

1. 手動で日付を入力するか、「**有効期限をリンク**」フィールドのカレンダーを使用して、公開リンクの有効期限を選択します。 選択した日付を過ぎるとレコードページビューにアクセスできなくなります。

1. **保存**&#x200B;をクリックします。

   ビューが更新され、グローバルアイコン ![](assets/public-shared-view-icon-highlighted.png) が表示されます。これは、ビューが公開されて共有されていることを示します。

   >[!TIP]
   >
   >ユーザーまたはグローバル アイコンのないビューは、ユーザーが作成したビューであり、他のユーザーと共有されていません。 非共有ビューは、自分にのみ表示されます。


1. （任意）コピーしたリンクを、メール、チャットメッセージ、ドキュメントまたはWorkfrontのコメントに貼り付けて、他のユーザーと共有します。

## 権限リクエストからビューに権限を付与する

アクセス権のないビューへのリンクにアクセスするユーザーは、ビューに対する権限をリクエストできます。 ビューに対する管理権限を持つすべてのユーザーは、権限リクエストを受け取り、権限を付与または拒否できます。

1. （条件付き）ビューの管理者は、次の領域で別のユーザーからビューにアクセスするリクエストを受け取る場合があります。

   * アプリ内通知
     ![](assets/in-app-notification-for-access-request-for-view.png)
   * メール通知
     ![](assets/in-app-notification-for-access-request-for-view.png)
1. （条件付き）Workfrontの通知領域で、アプリ内通知をクリックします
または
メール通知で「**すべての通知を表示**」をクリックし、リスト内の通知をクリックします。

   **保留中のアクセスリクエスト** ボックスが表示されます。

   ![](assets/notifications-list-approval-box.png)
1. （オプション）権限を承認するユーザーについて、ユーザー名の右側にあるドロップダウンメニューから次のいずれかのオプションを選択します。
   * **表示**
   * **管理**
1. 権限を承認または拒否するユーザーを選択し、「**すべて承認**」または「**すべて拒否** をクリックします。
1. **保留中のアクセスリクエスト** の左側にある左向き矢印をクリックし、「**保存**」をクリックします。

   要求を承認すると、ユーザーはビューの共有ボックスに追加されます。 権限をリクエストするユーザーに、リクエストが承認されたことを示すメールが届きます。<!--will they also get an in-app notification??-->

## ビューに対する権限を削除

{{step1-to-planning}}

1. 共有を停止するビューのワークスペースを開き、レコードタイプのカードをクリックします。 レコードタイプページが開きます。
1. 共有を削除するビューのタブ名にポインタを合わせ、[ 詳細 **] メニュー ![](assets/more-menu.png) ージをクリックしてから**[ 共有 **] をクリックし** す。
1. ビューの内部共有を削除するには、次の操作を行います。

   1. 「**内部共有**」タブが選択されていることを確認します。
   1. ユーザー、グループ、<span class="preview"> チーム、会社、担当業務 </span> 削除する内容を見つけ、ビューを共有するエンティティの名前の右側にある権限ドロップダウンメニューを展開して、「**削除**」をクリックします。

1. ビューの公開共有を削除するには、次の手順を実行します。

   1. 「**公開共有**」タブをクリックします。
   1. 「**公開リンクを作成**」オプションの選択を解除します。

1. **保存**&#x200B;をクリックします。

   ユーザーは、ビューにアクセスできなくなります。 ビューへのアクセスを削除されたユーザーに対しては、アクセス権がなくなったことを示す通知はありません。
