---
product-area: requests
navigation-topic: create-requests
title: リクエストエリアでのビューの作成と管理
description: 新しいリクエスト機能を使用する場合は、「リクエスト」領域のビューを作成して保存できます。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: 78ad910e8d121dda38c9a7da27b0b338e0e1dcda
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 10%

---


# リクエストエリアでのビューの作成と管理

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


Adobe Workfrontで新しいリクエスト機能を使用する場合は、「リクエスト」領域のビューを作成して保存できます。 これらの表示には、フィルターおよび列の配置が含まれます。

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* この機能は、「リクエスト」領域の新しいリクエストエクスペリエンスでのみ使用できます。
>* 表示設定は、ホームのマイリクエスト ウィジェットでも使用できます。 ただし、「リクエスト」領域のビューと「マイリクエスト」ウィジェットのビューは別になっています。
>* 「リクエスト」領域のリクエスト リストは、Workfrontの拡張リストを使用します。 詳しくは、[ 拡張リストの使用 ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意のWorkfrontまたはワークフローパッケージ</p>

<p>リクエストリストでWorkfront Planning リクエストを表示するための Workfront Planning ライセンス</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>コントリビューター以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  <p>レイアウトテンプレートにビューを追加するには、Workfront管理者である必要があります</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストのビューの作成

新しいリクエスト エクスペリエンスを使用する場合、Workfrontの「リクエスト」領域でビューを作成できます。

1. リクエスト リストにアクセスするには：

   {{step1-to-requests}}

1. **新しいエクスペリエンスを使用** 設定がオンになっていることを確認します。

1. **リクエスト** リストで「**表示**」ドロップダウンメニュー ![ 表示ドロップダウン ](assets/view-icon-requests.png) をクリックし、「**新しい表示**」をクリックします。

   ![ 新規ビュー ](assets/create-new-view.png)

1. 新しいビューの名前を入力し、[**作成**] をクリックします。
1. [ リクエスト エリアでのビューの編集 ](#edit-a-view-in-the-requests-area) を続行します。

## リクエストのビューの編集

Workfrontのリクエスト エリアで作成したビューを含め、既存のビューを編集できます。

「要求」領域でビューを編集すると、ビューの次の要素を変更できます。

* 名前
* フィルター
* 列

ビューに加えた変更は、ビューを共有するすべてのユーザーに表示されます。

1. リクエストのリストにアクセスするには、次を行います。

   {{step1-to-requests}}

1. **新しいエクスペリエンスを使用** 設定がオンになっていることを確認します。
1. **リクエスト** リストで、**表示** ドロップダウンメニュー ![ 表示ドロップダウン ](assets/view-icon-requests.png) から編集する表示を見つけます。

1. **表示** ドロップダウン ![ 表示ドロップダウン ](assets/view-icon-requests.png) をクリックし、表示の横の「。..」メニューをクリックして **名前を変更** を選択し、表示の新しい名前を入力します。
1. Enter キーを押して、新しい名前を保存します。
1. **表示** ドロップダウン ![ 表示ドロップダウン ](assets/view-icon-requests.png) をクリックし、編集する表示を選択します。
1. フィールドを列として追加するには、リストの右上隅にある **列を追加** アイコン ![ 列を追加 ](assets/add-column.png) をクリックします。

   **列マネージャー** が開きます。
1. ビューに列として追加するフィールドの横にあるプラスアイコンをクリックし、「**保存**」をクリックします。

   リスト内のオブジェクトに関連付けられているフィールドは、列として追加できます。<!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >列に追加するフィールドは、**列マネージャー** で使用する前に存在している必要があります。


1. （省略可能） **[ 列 ]** をクリックして、[F **フィールドの表示と順序** ボックスを開きます。
1. リストに表示する各フィールドの設定をオンにするか、オフにして非表示にするか、フィールドを別の順序でドラッグ&amp;ドロップします。

1. （任意）「**フィルター**」をクリックして、表示するリクエストの条件の追加を開始します。

   次のリクエストフィールドでフィルタリングできます。

   * **Workspace**: リクエストフォームが関連付けられているワークスペース。
   * **オブジェクトタイプ**：リクエストフォームが関連付けられているレコードタイプ。
   * **エントリ日**：リクエストが送信された日付。
   * **リクエストフォーム**：リクエストの送信に使用されるリクエストフォームの名前。
   * **ステータス**：リクエストのステータス。
   * **入力者**：リクエストを追加したユーザーの名前。 Workfront以外のユーザーがリクエストを追加した場合は、「入力者 **フィールドに** が表示さ `N/A` ます。

   また、ビューに表示されている任意のオブジェクトについて、ビューに追加された任意のフィールドでフィルタリングすることもできます。

   複数のフィルターを **And** または **Or** で結合できます。
フィルター条件を追加すると、リクエストリストが自動的にフィルタリングされます。


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * ビューの変更は自動的に保存されます。
> * ビューに対する変更は、そのビューを使用するすべてのユーザーに表示されます。
> * ユーザーを値として持つ任意のフィールドで、**Me （ログイン中のユーザー）** フィルターワイルドカードを使用します。

## 要求ビューをレイアウトテンプレートに追加します。

Workfront管理者は、新しいビューをレイアウトテンプレートに追加できます。

手順については、[ レイアウトテンプレートを使用したフィルター、ビュー、グループのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) を参照してください。

## ビューを共有

作成したビューは、他のユーザー、チームまたはグループと共有できます。

1. リクエストのリストにアクセスするには、次を行います。

   {{step1-to-requests}}

1. **新しいエクスペリエンスを使用** 設定がオンになっていることを確認します。
1. **要求** 一覧で、共有するビューを見つけます。
1. 共有するビューにポインタを合わせて、ビュー名の右側にある「。..」メニューをクリックし、「**共有**」をクリックします。
1. **共有** ボックスに、ビューを共有するユーザー、チーム、役割、グループまたは会社を入力し、表示されたらリストから選択します。
1. 「**保存**」をクリックします。

   指定したエンティティでビューが共有されます。 共有する前にビューに対して編集した更新済みビュー要素を表示できます。 <span class="preview"> ビューを更新すると、同じビューのコピーを作成し、コピーを共有する前に変更を保持しない限り、変更は他のユーザーには表示されません。 詳しくは、[ 拡張リストの使用 ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md) を参照してください。</span>
