---
title: ビューの共有
description: Adobe Workfront Planning を使用する際に、他のユーザーとビューを共有して、共同作業を確実に行えます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 58d2bf9f14b9a3adf4bacfad58f1b9862aeaf247
workflow-type: tm+mt
source-wordcount: '1871'
ht-degree: 16%

---


# ビューを共有

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning でレコードを操作する際に、他のユーザーとビューを共有して、共同作業を確実に行えます。

>[!IMPORTANT]
>
>* 他のユーザーにワークスペースの権限を付与しても、レコードタイプページのビューに対する権限は付与されません。他のユーザーと共有するには、レコードタイプのページ内の個々のビューに権限を付与する必要があります。
>
>* ビューに権限を付与しても、レコードを表示する権限は変更されません。 レコードの権限は、ワークスペースを共有することで付与されます。
>
>* ビューを共有すると、そのビューのすべての要素にアクセスする権限が他のユーザーに与えられます。 例えば、ビューに管理権限を付与すると、グループ化、フィルター、並べ替え、バーの外観を変更できます。


<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>ユーザーが権限リクエストに基づいてビューに対する権限をリクエストおよび付与できるようにするには、組織がAdobe統合エクスペリエンスにオンボーディングされている必要があります。 </p>
<p>Workfront Planning ビューへの権限を取得するには、ユーザーをAdobe Admin Consoleに追加する必要があります。</p>
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

</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ビューを共有する際の考慮事項

* ビューは、次の方法で共有できます。

   * 内部的には、Workfront ユーザー、グループ、チーム、会社、担当業務と連携します
   * 公開（Workfront以外のユーザーを使用）
   * ビューへのリンクをコピーして共有する
   * Excel または CSV ファイルに書き出す。 ファイルにエクスポートできるのは、テーブル表示のみです。 詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

* Adobe Workfront Planning でのオブジェクトの共有の一般的な情報については、[Workfront Planning での共有権限の概要 ](/help/quicksilver/planning/access/sharing-permissions-overview.md) も参照してください。
* ビューに対する表示権限または管理権限を、Workfrontの内部ユーザーに付与できます。

* 管理権限を持つユーザーは、表示設定の変更、共有、複製、削除を行うことができます。

* パブリック リンクを使用して、組織外のユーザーとビューを共有できます。

* ビューを公開して共有した場合、リンクには、会社外のユーザーが限られた期間（有効期限が示す）アクセスできます。 共有ビューを表示するためにログインする必要はありません。

* ビューへのアクセス権を持つ組織外のユーザーは、他のビューの作成、共有ビューの編集、ビュー内のレコード情報の追加、削除、編集を行うことはできません。

## ビューへの権限を内部的に共有

自分が作成したビュー、または管理権限を持つビューを、Workfront Planning のユーザー、グループ、チーム、会社、担当業務と共有できます。

>[!NOTE]
>
>システム管理者は、自分で作成しなかったビューは表示または共有できません。自分と共有されたビューのみにアクセスしたり、ビューのみを共有したりできます。
>
>システム管理者は、ビューに対する管理権限のみを持つことができます。

{{step1-to-planning}}

1. 共有するビューのワークスペースを開き、レコードタイプカードをクリックします。

   レコードタイプページが開きます。

1. 「表示」タブで、次のいずれかの操作を行います。

   * 共有するビューのタブ名にポインタを合わせて、ビュー名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、「**共有**」をクリックします。

     ![ ビューの詳細メニュー ](assets/more-menu-for-views-expanded-with-share-option.png)

   * **共有**/**現在のビューを共有** をクリックします

     ![ レコードタイプとビュー共有オプションを含む共有ボタン ](assets/share-button-with-record-type-and-view-sharing-options.png)

   **共有ビュー** ボックスが開き、**内部共有** タブがデフォルトで選択されています。

1. （オプション） **アクセスできるユーザー** 領域で、次のオプションから選択します。

   * **招待されたユーザーのみがアクセスできます**：ビューを共有するユーザー、グループ、チーム、会社または担当業務を指定する必要があります。 これはデフォルトのオプションです。

   >[!NOTE]
   >
   >チーム、グループ、会社、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。 Workfrontのみのユーザーを追加することはできません。 詳しくは、[Adobe Admin Consoleでのユーザーの管理 ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。


   * **ワークスペース内の全員が表示できます**：ワークスペースに対する表示以上の権限を持つすべてのユーザーが、ビューにアクセスできます。

1. 「**このビューへのアクセスを許可**」フィールドに、ユーザー、グループ、チーム、会社または担当業務の名前の入力を開始し、リストに表示されたらクリックします。

   ![ グループとのビューの共有 ](assets/sharing-a-view-ui-with-groups.png)

1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

     システム管理者は、共有されたビューに対する管理権限を常に受け取ります。

1. **保存**&#x200B;をクリックします。

   ビューが人物アイコン ![ 他のユーザーと共有されたビューのアイコン ](assets/view-shared-with-others-people-icon.png) で更新され、ビューが他のユーザーと共有されたことを示します。

   ビューを共有したユーザーには、権限に関するアプリ内通知とメール通知の両方が届きます。

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

1. 「表示」タブで、次のいずれかの操作を行います。

   * 共有するビューのタブ名にポインタを合わせて、ビュー名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、「**共有**」をクリックします。

   ![ 共有オプションを使用して展開されたビューの詳細メニュー ](assets/more-menu-for-views-expanded-with-share-option.png)
   * **共有**/**現在のビューを共有** をクリックします

   **ビューを共有** ボックスが開きます。

1. **公開共有** をクリックします。

   ![ ビューの「公開共有」タブ ](assets/public-sharing-tab-for-views.png)

1. **公開リンクを作成** 設定を有効にします。

   リンクが使用可能になります。 これは公開リンクです。 共有すると、組織外のユーザーを含め、リンクを持つすべてのユーザーがレコードタイプページにアクセスし、ページ上のレコードとフィールドを表示できます。

1. **リンクをコピー** アイコン ![ リンクビューをコピー ](assets/copy-link-view.png) をクリックして、リンクをクリップボードにコピーします。

1. 手動で日付を入力するか、「**有効期限をリンク**」フィールドのカレンダーを使用して、公開リンクの有効期限を選択します。 選択した日付を過ぎるとレコードページビューにアクセスできなくなります。

1. **保存**&#x200B;をクリックします。

   ビューが更新され、グローバルアイコン ![ 公開共有ビューアイコンがハイライト表示 ](assets/public-shared-view-icon-highlighted.png) が表示されます。これは、ビューが公開されて共有されていることを示します。

   >[!TIP]
   >
   >ユーザーまたはグローバル アイコンのないビューは、ユーザーが作成したビューであり、他のユーザーと共有されていません。 非共有ビューは、自分にのみ表示されます。


1. （任意）コピーしたリンクを、メール、チャットメッセージ、ドキュメントまたはWorkfrontのコメントに貼り付けて、他のユーザーと共有します。

## ビューへのリンクのコピー

ビューへのリンクをクリップボードにコピーして、別のアプリケーションに含めたり、他のユーザーと共有したりできます。

公開されているビューへのリンクをコピーするには、この記事の「[ ビューへの権限を公開で共有 ](#share-permissions-to-a-view-publicly) の節を参照してください。

このセクションでは、ビューを内部的に共有する方法について説明します。

>[!IMPORTANT]
>
>まず、ユーザーがビューを表示できるように、ビューへのリンクを共有する前に、ビューを共有する必要があります。


{{step1-to-planning}}

1. リンクをコピーして共有するビューのワークスペースを開き、レコードタイプのカードをクリックします。

   レコードタイプページが開きます。

1. ビューのタブで、次のいずれかの操作を行います。

   * 共有するビューのタブの上にマウスポインターを置き、ビュー名の右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックして、「ビューを共有 **ボックスの** 共有 **/** リンクをコピー **&#x200B;**&#x200B;をクリックします。
   * **ビューを共有** ボックスで **共有**/**ビューリンクをコピー**/**リンクをコピー** をクリックします。

   ビューへのリンクがクリップボードにコピーされ、画面の下部に確認が表示されます。

   別のアプリケーションにリンクを貼り付けたり、他のユーザーに送信したりできるようになりました。

## 権限リクエストからビューに権限を付与する

アクセス権のないビューへのリンクにアクセスするユーザーは、ビューに対する権限をリクエストできます。 ビューに対する管理権限を持つすべてのユーザーは、権限リクエストを受け取り、権限を付与または拒否できます。

1. （条件付き）ビューの管理者は、次の領域で別のユーザーからビューにアクセスするリクエストを受け取る場合があります。

   * アプリ内通知

     ![ 表示のアクセスリクエストのアプリ内通知 ](assets/in-app-notification-for-access-request-for-view.png)
   * メール通知

     ![ 表示のアクセスリクエストのアプリ内通知 ](assets/in-app-notification-for-access-request-for-view.png)
1. （条件付き）Workfrontの通知領域で、アプリ内通知をクリックします
または
メール通知で「**すべての通知を表示**」をクリックし、リスト内の通知をクリックします。

   **保留中のアクセスリクエスト** ボックスが表示されます。

   ![ 通知リストの承認ボックス ](assets/notifications-list-approval-box.png)
1. （オプション）権限を承認するユーザーについて、ユーザー名の右側にあるドロップダウンメニューから次のいずれかのオプションを選択します。
   * **表示**
   * **管理**
1. 権限を承認または拒否するユーザーを選択し、「**すべて承認**」または「**すべて拒否** をクリックします。
1. **保留中のアクセスリクエスト** の左側にある左向き矢印をクリックし、「**保存**」をクリックします。

   要求を承認すると、ユーザーはビューの共有ボックスに追加されます。 権限をリクエストするユーザーに、リクエストが承認されたことを示すメールが届きます。<!--will they also get an in-app notification??-->

## ビューに対する権限を削除

{{step1-to-planning}}

1. 共有を停止するビューのワークスペースを開き、レコードタイプのカードをクリックします。 レコードタイプページが開きます。
1. 「表示」タブで、次のいずれかの操作を行います。

   * 共有するビューのタブ名にポインタを合わせて、ビュー名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、「**共有**」をクリックします。

   * **共有**/**現在のビューを共有** をクリックします

   **ビューを共有** ボックスが開きます。
1. ビューの内部共有を削除するには、次の操作を行います。

   1. 「**内部共有**」タブが選択されていることを確認します。
   1. 削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、ビューを共有するエンティティの名前の右側にある権限ドロップダウンメニューを展開して、「**削除**」をクリックします。

1. ビューの公開共有を削除するには、次の手順を実行します。

   1. 「**公開共有**」タブをクリックします。
   1. 「**公開リンクを作成**」オプションの選択を解除します。

1. **保存**&#x200B;をクリックします。

   ユーザーは、ビューにアクセスできなくなります。 ビューへのアクセスを削除されたユーザーに対しては、アクセス権がなくなったことを示す通知はありません。
