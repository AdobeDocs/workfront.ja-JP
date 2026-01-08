---
product-area: requests
navigation-topic: create-requests
title: リクエスト エリアでのビューの作成と管理
description: 新しいリクエスト機能を使用する場合は、「リクエスト」領域のビューを作成して保存できます。
author: Becky
feature: Work Management
source-git-commit: 4061163b8b761bc3922bfb95da6c0110b6ee5871
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 10%

---

# リクエスト エリアでのビューの作成と管理

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

新しいリクエスト機能を使用する場合は、「リクエスト」領域のビューを作成して保存できます。 これらの表示には、フィルターと列の配置が含まれます。

ビューは、Workfrontの「リクエスト」領域で作成および管理できます。

>[!IMPORTANT]
>
>* この機能は、新しいリクエスト用エクスペリエンスでのみ使用できます。
>* ホームのマイリクエストウィジェットでは、表示設定は使用できません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>投稿者以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  <p>レイアウトテンプレートにビューを追加するには、Workfront管理者である必要があります</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 製品</td> 
   <td> <ul><li>Adobe Workfront</li><li>計画リクエストまたはリクエストフォームを表示するには、Adobe Workfront Planning が必要です。</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエスト エリアでのビューの作成

ビューは、Workfrontの「リクエスト」領域で作成できます。

1. リクエスト リストにアクセスするには：

   {{step1-to-requests}}

1. リクエストリストで「**表示**」ドロップダウン ![ 表示ドロップダウン ](assets/view-icon-requests.png) をクリックし、「**新しい表示**」を選択します。

   ![ 新規ビュー ](assets/create-new-view.png)

1. 新しいビューの名前を入力し、[**作成**] をクリックします。
1. [ リクエスト エリアでのビューの編集 ](#edit-a-view-in-the-requests-area) を続行します。

## 「リクエスト」領域でのビューの編集

作成したビューを含め、既存のビューを編集できます。

1. リクエスト リストにアクセスするには：

   {{step1-to-requests}}
1. [ 要求 ] ボックスの一覧で、編集するビューを見つけます。

1. （オプション）ビューの名前を変更するには、「**ビュー**」ドロップダウン ![ 「ビュー」ドロップダウン ](assets/view-icon-requests.png) をクリックし、ビューの横の「。..」メニューをクリックして「**名前を変更**」を選択し、ビューの新しい名前を入力します。
1. **表示** ドロップダウン ![ 表示ドロップダウン ](assets/view-icon-requests.png) をクリックし、編集する表示を選択します。
1. <span class="preview"> 列としてカスタムフィールドを追加するには、画面の右付近にある **列を追加** アイコン ![ 列を追加 ](assets/add-column.png) をクリックし、列としてビューに追加するカスタムフォームフィールドの横にあるプラスアイコンをクリックします。</span>

   <span class="preview"> リスト内のオブジェクトに添付されたフォームのカスタムフィールドは、列として追加できます。</span>

   >[!TIP]
   >
   >現在、実稼動環境で列を追加することはできません。
1. （任意）「**列**」をクリックして、リクエストリストの列の非表示、表示、並べ替えを行います。

   ![ 「列」ボックス ](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >現在、実稼動環境でこれ以上列を追加することはできません。

1. （任意）「**フィルター**」をクリックして、「計画」タブに表示する要求の条件の追加を開始します。

   ![ 「計画要求」タブでのフィルターの編集 ](assets/filters-editing-box-in-requests-planning-tab.png)

   次のフィールドでフィルタリングできます。

   * **Workspace**: リクエストフォームが関連付けられているワークスペース。
   * **レコードタイプ**：リクエストフォームが関連付けられているレコードタイプ。
   * **エントリ日**：リクエストが送信された日付。
   * **リクエストフォーム**：リクエストの送信に使用されるリクエストフォームの名前。
   * **ステータス**：リクエストのステータス。
   * **入力者**：リクエストを追加したユーザーの名前。 Workfront以外のユーザーがリクエストを追加した場合は、「入力者 **フィールドに** が表示さ `N/A` ます。

   <span class="preview"> プレビュー環境では、ビューに追加されたカスタムフィールドでフィルタリングすることもできます。</span>

   複数のフィルターを **And** または **Or** で結合できます。
フィルター条件を追加すると、リクエストリストが自動的にフィルタリングされます。



>[!IMPORTANT]
>
> * ビューの変更は自動的に保存されます。
> * ビューに対する変更は、そのビューを使用するすべてのユーザーに表示されます。

## レイアウト テンプレートにビューを追加します。

Workfront管理者は、新しいビューをレイアウトテンプレートに追加できます。

手順については、[ レイアウトテンプレートを使用したフィルター、ビュー、グループのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) を参照してください。

## ビューを共有

作成したビューは、他のユーザー、チームまたはグループと共有できます。

1. リクエスト リストにアクセスするには：

   {{step1-to-requests}}

1. [ 要求 ] ボックスの一覧で、共有するビューを見つけます。
1. 共有するビューの上にマウスポインターを置き、表示されたら 3 ドットメニューをクリックします。
1. 「**共有**」を選択します。
1. 開いたダイアログで、ビューを共有するユーザー、チーム、またはグループの名前を入力し、表示されたらリストから選択します。
1. 「**保存**」をクリックします。

