---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：カスタムデータフィールドを使用した外部 URL」
description: タスクビューで「カスタム URL」という名前の計算済みカスタムフィールドを使用して、内部カスタム URL へのリンクを表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '693'
ht-degree: 100%

---

# ビュー：カスタムデータフィールドを使用する外部 URL

**タスクビュー**&#x200B;で「カスタム URL」という名前の&#x200B;**計算済みカスタムフィールド**&#x200B;を使用して、内部カスタム URL へのリンクを表示できます。

これにより、ビューの特定のオブジェクトからアプリケーションの特定のエリアへ、レポートから直接リンクするのに役立ちます。

計算済みカスタムフィールドを作成する場合は、まずフィールドを作成してから、ビューを作成する必要があります。

次のセクションは、タスクの計算済みカスタムフィールドの例です。カスタムフィールドはカスタム URL と呼ばれます。カスタムビューには、フィールドの値およびタスクの「**URL**」フィールドが表示されます。

同じ手順を使用して、カスタムフォームを持つシステム内のすべてのオブジェクトに対して、類似した計算済みカスタムフィールドとカスタムビューを作成できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>表示の変更をリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 「カスタム URL」計算済みカスタムフィールドの作成

計算済みカスタムフィールドの作成について詳しくは、[計算データのカスタムフォームへの追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)の記事を参照してください。

カスタムフォームを作成するアクセス権がある場合は、「カスタム URL」と呼ばれるタスクの計算済みカスタムフィールドを作成できます。このフィールドは、「**タスクの詳細**」タブ内の「**概要**」サブタブに直接リンクします。

1. 計算済みカスタムフィールドを作成します。
1. 「計算」フィールドに、次のコードを入力します。

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. 「`<domain>`」を括弧を除いた実際のドメイン名と置き換えます。

   この

   ```
   /overview
   ```

   URL の一部は、タスクの左側のパネルの「**概要**」セクションに直接リンクします。

1. **計算済みカスタムフィールド**&#x200B;の作成後、このフィールドと&#x200B;**カスタムフォーム**&#x200B;を新しいビューに表示する Adobe Workfront の複数のタスクに添付します。

## タスクの「カスタム URL」フィールドと「URL」フィールドを表示するビューの作成

以下の例のタスク&#x200B;**ビュー**&#x200B;では、「カスタム URL」と呼ばれる&#x200B;**計算済みカスタムフィールド**&#x200B;が「**詳細**」タブ内の「**概要**」サブタブおよびタスクの「**URL**」フィールドへの直接リンクとして表示されます。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

このビューをカスタマイズするには、次の手順に従います。

1. タスクのリストに移動します。
1. タスクリストの上部にある&#x200B;**ビュー**&#x200B;のドロップダウンを展開します。
1. 「**ビューをカスタマイズ**」をクリックします。
1. 最初の列を除くビュー内のすべての列を削除します。
1. 最初の列のヘッダーをクリックします。
1. インターフェイスの上右隅にある「**テキストモードに切り替え**」をクリックします。
1. 「**クリックするとテキストを編集できます**」をクリックします。
1. 以下のテキストモードを 1 つの列に貼り付けます。\
   この例では、「column.1」です。タスクの&#x200B;**概要**&#x200B;へのリンクとして「カスタム URL」フィールドが表示されます。「列 2」タスクの **URL フィールド**&#x200B;に保存された値が表示されます。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(Custom URL)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(Custom URL)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=Custom URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 「**ビューを保存**」をクリックします。
