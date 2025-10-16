---
product-area: requests
navigation-topic: create-requests
title: リクエスト エリアでのビューの作成
description: 新しいリクエスト機能を使用する場合は、「リクエスト」領域のビューを作成して保存できます。
author: Becky
feature: Work Management
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 5%

---

# リクエスト エリアでのビューの作成または編集


新しいリクエスト機能を使用する場合は、「リクエスト」領域のビューを作成して保存できます。 これらの表示には、フィルターと列の配置が含まれます。

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

{{step1-to-requests}}

1. （オプションおよび条件付き）以下の項目が組織とWorkfront インスタンスに当てはまる場合は、画面の右上にある「**新しいエクスペリエンスに切り替え**」設定を選択してください。

   * Workfront パッケージを購入している
   * 組織がAdobe統合エクスペリエンスにオンボーディングされました。
   * 管理者から、Workfront Planning へのアクセス権を付与されています
   * Workfront Planning Workspace に対して少なくとも表示権限がある

   詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの発行 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) を参照してください

1. **表示** ドロップダウン ![&#x200B; 表示ドロップダウン &#x200B;](assets/view-icon-requests.png) をクリックし、「**新しい表示**」を選択します。

   ![&#x200B; 新規ビュー &#x200B;](assets/create-new-view.png)

1. 新しいビューの名前を入力し、[**作成**] をクリックします。
1. [&#x200B; リクエスト エリアでのビューの編集 &#x200B;](#edit-a-view-in-the-requests-area) を続行します。

## 「リクエスト」領域でのビューの編集

作成したビューを含め、既存のビューを編集できます。

{{step1-to-requests}}

1. （オプションおよび条件付き）以下の項目が組織とWorkfront インスタンスに当てはまる場合は、画面の右上にある「**新しいエクスペリエンスに切り替え**」設定を選択してください。

   * Workfront パッケージを購入している
   * 組織がAdobe統合エクスペリエンスにオンボーディングされました。
   * 管理者から、Workfront Planning へのアクセス権を付与されています
   * Workfront Planning Workspace に対して少なくとも表示権限がある

   詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの発行 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md)1 を参照してください。

1. （オプション）ビューの名前を変更するには、「**ビュー**」ドロップダウン ![&#x200B; 「ビュー」ドロップダウン &#x200B;](assets/view-icon-requests.png) をクリックし、ビューの横の「。..」メニューをクリックして「**名前を変更**」を選択し、ビューの新しい名前を入力します。
1. **表示** ドロップダウン ![&#x200B; 表示ドロップダウン &#x200B;](assets/view-icon-requests.png) をクリックし、編集する表示を選択します。
1. （任意）「**フィルター**」をクリックして、「計画」タブに表示する要求の条件の追加を開始します。

   ![&#x200B; 「計画要求」タブでのフィルターの編集 &#x200B;](assets/filters-editing-box-in-requests-planning-tab.png)

   次のフィールドでフィルタリングできます。

   * **Workspace**: リクエストフォームが関連付けられているワークスペース。
   * **レコードタイプ**：リクエストフォームが関連付けられているレコードタイプ。
   * **エントリ日**：リクエストが送信された日付。
   * **リクエストフォーム**：リクエストの送信に使用されるリクエストフォームの名前。
   * **ステータス**：リクエストのステータス。
   * **入力者**：リクエストを追加したユーザーの名前。 Workfront以外のユーザーがリクエストを追加した場合は、「入力者 **フィールドに** が表示さ `N/A` ます。

   複数のフィルターを **And** または **Or** で結合できます。
フィルター条件を追加すると、リクエストリストが自動的にフィルタリングされます。

1. （任意）「**列**」をクリックして、リクエストリストの列の非表示、表示、並べ替えを行います。

   ![&#x200B; 「列」ボックス &#x200B;](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >これ以上列を追加することはできません。

>[!IMPORTANT]
>
> * ビューの変更は自動的に保存されます。
> * ビューに対する変更は、そのビューを使用するすべてのユーザーに表示されます。

## レイアウト テンプレートにビューを追加します。

Workfront管理者は、新しいビューをレイアウトテンプレートに追加できます。

手順については、[&#x200B; レイアウトテンプレートを使用したフィルター、ビュー、グループのカスタマイズ &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) を参照してください。
