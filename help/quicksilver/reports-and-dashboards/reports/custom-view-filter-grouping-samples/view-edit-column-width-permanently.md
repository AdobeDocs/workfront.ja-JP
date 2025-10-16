---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：列の幅を永続的に編集
description: 余白をドラッグ＆ドロップして、目的の幅に合わせて一時的に列の幅を変更できます。詳しくは、列の幅と順序を変更を参照してください。
author: Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 87%

---

# ビュー：列の幅を永続的に編集

<!-- Audited: 11/2024 -->

余白をドラッグ＆ドロップして、目的の幅に合わせて一時的に列の幅を変更できます。詳しくは、[列の幅と順序を変更](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)を参照してください。

ビューの列の幅を恒久的に変更するには、ビューの編集時に列でテキストモードを使用する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>ビューの投稿者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 列の幅を恒久的に編集

>[!IMPORTANT]
>
>列の幅を完全に変更した後で、[列の幅と順序を変更](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)の記事の[幅と順序を一時的に変更](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily)の節で説明されているように、列の幅を手動で変更すると、列の幅は手動で変更したサイズに従って保持されます。この場合、以下の手順に従って更新された列の幅は上書きされます。キャッシュをクリアするか、別のブラウザーからログインすると、次の手順で定義した幅に従って列を表示できます。
>
>テキストモードインターフェイスを使用する際の列の幅のカスタマイズについて詳しくは、[Adobe Workfront の用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

1. オブジェクトのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックして新しい列を追加します。

   または

   既存の列の列ヘッダーをクリックします。

1. 「**テキストモードに切り替え**」をクリックします。
1. **テキストモードを編集**.T をクリックします
1. 列のテキストモードに次のコードを追加します。

   ```
   width=200
   usewidths=true
   ```

   **幅**&#x200B;の行で、ビューで表示する列の幅を表す任意の数値（ピクセル単位）を指定します。

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。


