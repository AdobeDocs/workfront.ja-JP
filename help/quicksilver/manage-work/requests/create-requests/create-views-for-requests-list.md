---
product-area: requests
navigation-topic: create-requests
title: リクエストエリアでのビューの作成と管理
description: 新しいリクエストエクスペリエンスを使用している場合は、リクエスト領域のビューを作成して保存できます。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 10%

---


# リクエストエリアでのビューの作成と管理

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


Adobe Workfrontで新しいリクエストエクスペリエンスを使用している場合は、リクエスト領域のビューを作成して保存できます。 これらのビューには、フィルターと列の配置が含まれます。

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* この機能は、リクエスト領域の新しいリクエストエクスペリエンスでのみ使用できます。
>* ビュー設定は、ホームのマイリクエストウィジェットでも使用できます。 ただし、リクエスト領域のビューは、マイリクエストウィジェットのビューとは異なります。
>* リクエスト領域のリクエストリストでは、Workfrontの拡張リストが使用されます。 詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意のWorkfrontまたはWorkflow パッケージ</p>

<p>任意のWorkfront プランニングライセンス。リクエストリストでWorkfront プランニングリクエストを表示できます</p>
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

新しいリクエストエクスペリエンスを使用すると、Workfrontのリクエスト領域にビューを作成できます。

1. リクエストリストにアクセスするには：

   {{step1-to-requests}}

1. 「**新しいエクスペリエンスを使用**」設定がオンになっていることを確認します。

1. **リクエスト** リストで、**ビュー** ドロップダウンメニュー![&#x200B; ビューのドロップダウン &#x200B;](assets/view-icon-requests.png)をクリックし、**新しいビュー**&#x200B;をクリックします。

   ![新しいビュー](assets/create-new-view.png)

1. 新しいビューの名前を入力し、**作成**&#x200B;をクリックします。
1. 続行[&#x200B; リクエスト領域](#edit-a-view-in-the-requests-area)でビューを編集します。

## リクエストのビューの編集

Workfrontのリクエスト領域で作成したビューなど、既存のビューを編集できます。

リクエスト領域でビューを編集すると、ビューの次の要素を変更できます。

* 名前
* フィルター
* 列

ビューに加えた変更は、ビューを共有するすべてのユーザーに表示されます。

1. リクエスト内のリクエストのリストにアクセスするには、次の手順を実行します。

   {{step1-to-requests}}

1. 「**新しいエクスペリエンスを使用**」設定がオンになっていることを確認します。
1. **リクエスト** リストで、**ビュー** ドロップダウンメニュー![&#x200B; ビュー](assets/view-icon-requests.png)から編集するビューを見つけます。

1. **ビュー** ドロップダウン ![&#x200B; ビューのドロップダウン &#x200B;](assets/view-icon-requests.png)をクリックし、ビューの横にある3点メニューをクリックして、**名前を変更**&#x200B;を選択し、ビューの新しい名前を入力します。
1. Enter キーを押して、新しい名前を保存します。
1. **ビュー** ドロップダウン ![&#x200B; ビュー](assets/view-icon-requests.png)をクリックし、編集するビューを選択します。
1. フィールドを列として追加するには、リストの右上隅にある「**列を追加**」アイコン「![列を追加](assets/add-column.png)」をクリックします。

   **列マネージャー**&#x200B;が開きます。
1. ビューに列として追加するフィールドの横にあるプラスアイコンをクリックし、**保存**&#x200B;をクリックします。

   リスト内のオブジェクトに関連付けられたフィールドは、列として追加できます。<!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >列に追加するフィールドは、**列マネージャー**&#x200B;で使用可能になる前に存在する必要があります。

1. （オプション）「**列**」をクリックして、**フィールドの表示と注文** ボックスを開きます。
1. リストに表示する各フィールドの設定をオンにするか、オフにして非表示にするか、フィールドを別の順序でドラッグ&amp;ドロップします。

1. （オプション）「**フィルター**」をクリックし、表示するリクエストの条件の追加を開始します。

   次のリクエストフィールドでフィルタリングできます。

   * **Workspace**: リクエストフォームが関連付けられているワークスペース。
   * **オブジェクトタイプ**：リクエストフォームが関連付けられているレコードタイプ。
   * **エントリ日**：リクエストが送信された日付。
   * **リクエストフォーム**：リクエストの送信に使用されるリクエストフォームの名前。
   * **ステータス**: リクエストのステータス。
   * **入力者**：リクエストを追加したユーザーの名前。 リクエストがWorkfront以外のユーザーによって追加された場合、**入力者** フィールドには`N/A`が表示されます。

   ビューに表示されているオブジェクトについて、ビューに追加された任意のフィールドでフィルタリングすることもできます。

   **And**&#x200B;または&#x200B;**または**&#x200B;のいずれかによって複数のフィルターを結合できます。
フィルター条件を追加すると、リクエストリストは自動的にフィルタリングされます。


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * ビューの変更は自動的に保存されます。
> * ビューの変更は、そのビューを使用するユーザーに表示されます。
> * ユーザーを値として持つ任意のフィールドで、**Me （ログインユーザー）** フィルターワイルドカードを使用します。

## リクエストビューをレイアウトテンプレートに追加します。

Workfront管理者は、新しいビューをレイアウトテンプレートに追加できます。

手順については、[&#x200B; レイアウトテンプレートを使用したフィルター、ビュー、グループ化のカスタマイズ &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

## ビューを共有

作成したビューは、他のユーザー、チーム、またはグループと共有できます。

1. リクエスト内のリクエストのリストにアクセスするには、次の手順を実行します。

   {{step1-to-requests}}

1. 「**新しいエクスペリエンスを使用**」設定がオンになっていることを確認します。
1. **リクエスト** リストで、共有するビューを見つけます。
1. 共有するビューにマウスポインターを置き、ビュー名の右側にある3点メニューをクリックしてから、**共有**&#x200B;をクリックします。
1. **共有** ボックスで、ビューを共有するユーザー、チーム、役割、グループ、または会社を入力し、表示されたらリストから選択します。
1. 「**保存**」をクリックします。

   ビューは、指定したエンティティと共有されます。 共有する前に、ビュー用に編集した更新されたビュー要素を表示できます。 <span class="preview"> ユーザーがビューを更新すると、同じビューのコピーを作成し、変更内容を保存してからコピーを共有しない限り、変更内容は他のユーザーには表示されません。 詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。</span>
