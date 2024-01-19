---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：列の幅を永久的に編集'
description: 余白をドラッグ&ドロップして目的の幅に合わせて一時的に列の幅を変更できます。 詳細については、「列の幅と順序を変更する」を参照してください。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 表示：列の幅を永続的に編集する

<!-- Audited: 1/2024 -->

余白をドラッグ&amp;ドロップして目的の幅に合わせて一時的に列の幅を変更できます。 詳しくは、 [列の幅と順序を変更する](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

ビューの任意の列の幅を永久的に変更するには、ビューの編集時に、列のテキストモードを使用する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> <p>新規：<ul><li>ビューを変更する寄稿者</li><li>レポートを変更するための標準</li></ul></p><p>または</p>現在：<ul><li>ビューの変更をリクエスト</li><li>レポートを変更する計画</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートに対する権限の管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 列の幅を永続的に編集する

>[!IMPORTANT]
>
>列の幅を手動で変更する場合は、「 」の項を参照してください。 [列の幅と順序を一時的に変更する](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) 記事内 [列の幅と順序を変更する](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 列の幅を永久的に変更した後は、手動でのサイズ変更に従って列の幅が保持されます。 この場合、以下の手順に従って更新された列の幅が上書きされます。 キャッシュをクリアした後、または別のブラウザーからログインした後、次の手順で定義した幅に従って列を表示できます。
>
>テキストモードインターフェイスを使用する際の列の幅のカスタマイズに関する詳細は、 [Adobe Workfrontの用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. オブジェクトのリストに移動します。
1. 次から： **表示** ドロップダウンメニューで、 **新しいビュー**.

1. クリック **列を追加** をクリックして新しい列を追加します。

   または

   既存の列の列見出しをクリックします。

1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 次のコードを列のテキストモードに追加します。

   ```
   width=200
   usewidths=true
   ```

   の **幅** 行には、列を表示するビューの幅を表す任意の数値（ピクセル単位）を指定します。

1. クリック **保存**&#x200B;を、 **ビューを保存**.


