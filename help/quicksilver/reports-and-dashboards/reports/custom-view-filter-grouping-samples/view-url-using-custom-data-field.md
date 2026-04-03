---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: ビュー：カスタムデータフィールドを使用した外部URL
description: タスクビューで「カスタム URL」という名前の計算済みカスタムフィールドを使用して、内部カスタム URL へのリンクを表示できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 78%

---

# ビュー：カスタムデータフィールドを使用する外部 URL

<!--Audited: 11/2024-->

**タスクビュー**&#x200B;で「カスタム URL」という名前の&#x200B;**計算済みカスタムフィールド**&#x200B;を使用して、内部カスタム URL へのリンクを表示できます。

これにより、ビューの特定のオブジェクトからアプリケーションの特定のエリアへ、レポートから直接リンクするのに役立ちます。

計算済みカスタムフィールドを作成する場合は、まずフィールドを作成してから、ビューを作成する必要があります。

次のセクションは、タスクの計算済みカスタムフィールドの例です。カスタムフィールドはカスタム URL と呼ばれます。カスタムビューには、フィールドの値およびタスクの「**URL**」フィールドが表示されます。

同じ手順を使用して、カスタムフォームを持つシステム内のすべてのオブジェクトに対して、類似した計算済みカスタムフィールドとカスタムビューを作成できます。

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
   <p>ビューを変更するコントリビューターまたはリクエスト </p>
   <p>レポートを修正する標準または計画</p>
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

## 「カスタム URL」計算済みカスタムフィールドの作成

計算カスタムフィールドの作成について詳しくは、[計算フィールドをフォームに追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)を参照してください。

カスタムフォームを作成するアクセス権がある場合は、「カスタム URL」と呼ばれるタスクの計算済みカスタムフィールドを作成できます。このフィールドは、「**タスクの詳細**」タブ内の「**概要**」サブタブに直接リンクします。

1. 計算済みカスタムフィールドを作成します。
1. 「計算」フィールドに、次のコードを入力します。

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. 「`<domain>`」を、角括弧なしで実際のドメイン名に置き換えます。 このURLの`/overview`部分は、タスクの左側のパネルにある&#x200B;**概要** セクションへのリンクを指示します。

1. **計算済みカスタムフィールド**&#x200B;の作成後、このフィールドと&#x200B;**カスタムフォーム**&#x200B;を新しいビューに表示する Adobe Workfront の複数のタスクに添付します。

## タスクの「カスタム URL」フィールドと「URL」フィールドを表示するビューの作成

以下の例のタスク&#x200B;**ビュー**&#x200B;では、「カスタム URL」と呼ばれる&#x200B;**計算済みカスタムフィールド**&#x200B;が「**詳細**」タブ内の「**概要**」サブタブおよびタスクの「**URL**」フィールドへの直接リンクとして表示されます。

（assets/task-view-with-custom-url-field-quicksilver-350x70.png）

このビューをカスタマイズするには、次の手順に従います。

1. タスクのリストに移動します。
1. タスクリストの上部にある&#x200B;**ビュー**&#x200B;のドロップダウンを展開します。
1. 「**ビューをカスタマイズ**」をクリックします。
1. 最初の列を除くビュー内のすべての列を削除します。
1. 最初の列のヘッダーをクリックします。
1. **テキストモードに切り替え**/**テキストモードを編集**&#x200B;をクリックします。
1. 「**テキストモードを編集**」ボックスのテキストを削除し、次のコードに置き換えます。


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   この例では、「column.1」です。行には、タスクの&#x200B;**Overview** セクション、「column.2」へのリンクとして、「カスタム URL」フィールドの値が表示されます。 タスクの **URL フィールド**&#x200B;に保存された値が表示されます。

1. **完了** / **ビューを保存**&#x200B;をクリックします。
