---
title: Adobe Workfront Planning でのリスト表示の管理
description: Adobe Workfront Planning のレコードの「接続されたレコード」ページでオブジェクトとそのフィールドにアクセスすると、リスト・ビューでオブジェクトとそのフィールドを表示できます。 この記事では、レコードの接続されたレコード ページでリスト表示を作成または編集する方法について説明します。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 2%

---


# Adobe Workfront Planning でのリスト ビューの管理

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning のレコードの「接続されたレコード」ページでオブジェクトとそのフィールドにアクセスすると、リスト・ビューでオブジェクトとそのフィールドを表示できます。

この記事では、レコードの [ 接続されたレコード ] ページでリスト ビューを作成または編集する方法と、ビュー内のオブジェクトを編集する方法について説明します。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontと任意の Planning パッケージ</p>
<p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p> ビューを作成および削除するための標準</p>
   <p>ビュー要素を更新する投稿者以上</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ビューに対する権限を管理</p>  
   <p>ビュー設定を一時的に変更したり、複製したりするためのビューへのアクセス許可を表示します</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++ 

## リスト表示に関する考慮事項

* リスト表示では、レコードタイプページのレコードを表示できません。 以下のオブジェクトは、レコードの [ 接続されたレコード ] ページで表示した場合にのみ、リスト ビューで表示できます。

   * Workfront プロジェクト

  接続レコード ページを作成する方法については、[&#x200B; レコードに接続レコード ページを追加する &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) を参照してください。
* レコードの接続済みレコードページでリストビューを表示する前に、Workfront プロジェクトを Planning レコードタイプに関連付ける必要があります。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* リスト表示は、拡張リストに似ています。 詳しくは、[&#x200B; 拡張リストの使用 &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md) を参照してください。


## リスト表示の管理 {#manage-a-list-view}

Workfrontでのリストビューの管理について詳しくは、[&#x200B; 拡張リストの使用 &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md) を参照してください。

{{step1-to-planning}}

1. ワークスペースカードをクリックし、レコードタイプのカードをクリックします。
1. 任意の表示でレコードの名前をクリックして、レコードのプレビューまたは詳細ページを開きます。
1. **レコードへの接続されたレコード ページの追加** の記事で説明されているように、接続されたプロジェクトに [&#x200B; 接続されたレコード ページ &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) を追加します。

   接続されたレコード ページには、リスト表示でレコードに接続されたプロジェクトが表示されます。

   ![&#x200B; リスト表示の接続されたレコードページのプロジェクト &#x200B;](assets/projects-on-connected-records-page-list-view.png)

1. （オプション）次のいずれかの操作を行って、リスト表示を変更します。

   1. リストの右上隅にあるドロップダウンビューメニューを展開して別のビューを選択するか、「**新規ビュー**」をクリックして別のビューを作成します。

      ビューは、システム全体で共有されます。 あるレコードタイプに対してプロジェクト ビューを作成すると、接続されたプロジェクトを表示する他のレコードタイプで表示できます。

   1. 既存のビューの名前にポインタを合わせて **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックし、次のいずれかをクリックします。
      * **名前を変更**：ビューに新しい名前を付けます。
      * **共有**：他のユーザーとビューを共有します
      * **削除**：ビューを削除します。

      >[!NOTE]
      >
      >ビューを編集、共有、削除するには、そのビューに対する管理権限が必要です。
      >
      >システム・ビューは変更できません。
      >
   1. **フィルター** アイコン ![&#x200B; フィルターアイコン &#x200B;](assets/filter-icon.png) をクリックして、ビューにフィルターを追加します。 結果は、リスト内で直ちにフィルタリングされます。 フィルターを保存して名前を付けることはできません。 フィルターは、今後ページにアクセスしたときに記憶されるもので、共有ビューの一部です。
   1. **列** アイコン ![&#x200B; 列アイコン &#x200B;](assets/columns-icon.png) をクリックして、表示する列またはビューで非表示にする列を選択します。
   1. 列名にポインタを合わせ、列名の左にある下向き矢印をクリックして、次のいずれかをクリックします。
      * **名前を変更**：列に **カスタムラベル** を追加します。 Workfrontの元のフィールドの名前は変更されません。
      * **並べ替え**：選択したフィールドでリストを並べ替えます。 並べ替えの方向を示す並べ替えアイコンが列ヘッダーに追加されます。
   1. リストの右上隅にある「**+**」アイコンをクリックして、リストに列を追加または削除し、「**保存**」をクリックします。

      **列マネージャー** が開きます。

      リスト表示に追加できるのは、既存のフィールドのみです。
リスト表示で、最初の列に表示されるプライマリフィールドは削除できません。
1. （オプション）リストの右上隅にある検索ボックスにキーワードを追加して、項目を検索します。

   検索語句に一致する項目がリストでハイライト表示されます。
1. （オプション）リストにさらに項目を追加し、選択したレコードにそれらを自動的に接続するには、次のいずれかの操作を行います。

   * 既存の項目を追加するには、リストの右上隅にある「**レコードを接続**」をクリックします。
   * リストの下部にある「**新しい行**」をクリックして、新しい項目を追加します。
1. リストで接続された項目の名前をクリックすると、別のブラウザータブでその項目が開きます。
1. リストのセル内をダブルクリックしてフィールドの情報を編集し、Enter キーを押して変更を保存します。

   読み取り専用のフィールドがあります。 例えば、プロジェクトの完了率は、システムによって計算されたフィールドであり、手動で編集することはできません。

1. リスト内の項目の名前にポインタを合わせ、「**詳細**」メニュー [&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、「**表示**」をクリックして別のタブでプロジェクトを開きます

   または

   1 つ以上の項目を選択し、リストの下部にあるアクションバーに注目して、次のいずれかをクリックします。

   * **削除**：プロジェクトを削除します。 プロジェクトを削除すると、レコードから切断され、Workfrontのごみ箱に移動されます。 Workfront管理者は、削除されたプロジェクトを、削除されてから最大 30 日後まで復元できます。
   * **切断**：レコードからプロジェクトを切断します。 プロジェクトの接続を解除すると、プロジェクトとその参照フィールドのすべての値が現在のレコードから削除されます。

   ![&#x200B; 接続されたレコードページのリストビューのアクションバー &#x200B;](assets/actions-bar-connected-records-page-list-view.png)

