---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：列の内容を非表示にする'
description: ビューの列で情報を非表示にしたい場合があります。 これを行うには、列のテキストモードを変更します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 表示：列の内容を非表示にする

ビューの列で情報を非表示にしたい場合があります。 これを行うには、列のテキストモードを変更します。

>[!TIP]
>
>* 非表示の列を使用して、ビューに表示したくない特定のオブジェクトで並べ替えることができます。\
   >  たとえば、タスクビューで Task Number で並べ替え、ビューで Task Number 情報を非表示にすることができます。 この場合、列で参照されるオブジェクトはビューの並べ替えに役立ちますが、そのオブジェクトの情報はビューに表示されません。
>* 列を非表示にする場合、列の情報は非表示になりますが、その列はビューに表示されたままです。
>


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 例：タスクビューのタスク番号列の並べ替えと非表示：

1. タスクのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、 **新しいビュー**.

1. クリック **列を追加** をクリックし、 **この列に表示** フィールドを選択し、リストに表示されるタイミングで選択します。

1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>列を非表示にする、このコードでの重要な変更点は次のとおりです。

   ```
   displayname
   ```

   この行は空白にする必要があります。

   ```
   valuefield
   ```

   これは、 *値*、およびは空白にする必要があります。

   ```
   width
   ```

   :フィールドに応じて、の値が必要です。 *0* または *1*.

1. クリック **保存**&#x200B;を、 **ビューを保存**.
