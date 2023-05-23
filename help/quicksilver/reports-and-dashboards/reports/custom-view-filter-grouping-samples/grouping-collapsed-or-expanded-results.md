---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''グループ化：グループ化の結果をテキストモードで折りたたむか展開するかを指定します'
description: '''グループ化：グループ化の結果をテキストモードで折りたたむか展開するかを指定します'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# グループ化：グループ化の結果をテキストモードで折りたたむか展開するかを指定します

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

標準の Report Builder を使用すると、リストまたはレポートでグループ化の結果を折りたたんだり展開したりするかどうかを指定できます。 その結果、デフォルトでグループ化表示が展開されます。 グループ化の作成について詳しくは、 [Adobe Workfrontでのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* リスト表示時にグループを手動で調整すると、Adobe Workfrontでは、ログアウトするまで手動の設定が記憶されます。 再度ログインすると、この設定に従ってリストが表示されます。
>* グループ化の結果は、グラフ要素からアクセスした後で常に展開表示されます。
>


また、テキストモードを使用して、グループ化を展開または折りたたむかどうかを指定することもできます。

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
   <td> <p>グループ化を変更するリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してグループ化を変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## テキストモードを使用してグループ化の結果を折りたたむか展開するかを指定します

1. オブジェクトのリストに移動します。
1. 次の **グループ化**&#x200B;ドロップダウンメニューで、「 **新しいグループ化**.

1. グループを追加し、 **テキストモードに切り替え**.

   または

   グループ化が既にテキストモードの場合は、折りたたまれて表示するグループ化レベルに次のコードを追加します。

   ```
   group.0.iscollapsed=true
   ```

1. （オプション）グループを展開して表示する場合、次のコードを適切なグループ化レベルに追加します。

   ```
   group.0.iscollapsed=false
   ```

1. クリック **完了**&#x200B;を、 **グループ化を保存**.
