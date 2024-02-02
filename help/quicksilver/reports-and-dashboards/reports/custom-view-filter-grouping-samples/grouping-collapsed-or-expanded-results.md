---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「グループ化：テキストモードを使用してグループ化の結果を折りたたむか展開するかを指定」
description: 「グループ化：テキストモードを使用してグループ化の結果を折りたたむか展開するかを指定」
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '366'
ht-degree: 100%

---

# グループ化：テキストモードでグループ化の結果を折りたたむか展開するかを指定します

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

標準の Report Builder を使用することにより、リストまたはレポートでグループ化の結果を折りたたんで表示するか展開して表示するかを指定できます。グループ化の結果は、デフォルトでは展開して表示されます。グループ化の作成について詳しくは、[Adobe Workfront でのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* リストを表示するときにグループ化を手動で調整すると、ログアウトするまで Adobe Workfront に手動の設定が記憶されます。再度ログインすると、この設定に従ってリストが表示されます。
>* グループ化の結果は、グラフ要素からアクセスした後で常に展開表示されます。
>

グループ化を展開して表示するか、折りたたんで表示するかは、テキストモードを使用して指定することもできます。

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
   <td> <p>グループ化を変更するためのリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、ビュー、グループ化へのアクセス権を編集して、グループ化を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## テキストモードを使用してグループ化の結果を折りたたむか展開するかを指定

1. オブジェクトのリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで、「**新規グループ化**」を選択します。

1. グループ化を追加し、「**テキストモードに切り替える**」をクリックします。

   または

   グループ化が既にテキストモードの場合は、折りたたんで表示するグループ化レベルに次のコードを追加します。

   ```
   group.0.iscollapsed=true
   ```

1. （オプション）グループ化を展開して表示する場合は、該当するグループ化レベルに次のコードを追加します。

   ```
   group.0.iscollapsed=false
   ```

1. 「**完了**」、「**グループ化の保存**」の順にクリックします。
