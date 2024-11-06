---
title: 既存のグループを編集
description: 既存のグループを編集
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 86%

---

# 既存のグループを編集

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

最初に作成した既存のグループ化または自分と共有された既存のグループ化をカスタマイズできます。次に、新規グループ化として保存できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>投稿者以上</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>リクエスト以上</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>報告書、ダッシュボード、カレンダーへのアクセスを編集して、報告書のグループ化を編集します</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>レポートへの管理権限でレポート内のグループ化を編集</p> <p>グループ化への管理権限</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 前提条件

編集する前に、グループ化を作成する必要があります。

グループ化の作成について詳しくは、[Adobe Workfront でのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)を参照してください。

## 操作手順

1. カスタマイズしたいグループ化を含むオブジェクトのリストに移動します。
1. **グループ化**&#x200B;アイコンをクリックします。
1. カスタマイズするグループ化を選択し、**編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

   ![編集アイコンを選択します。](assets/customizegrouping-nwe-standard-350x291.png)

   グループ化をカスタマイズするためのインターフェイスビルダーが開きます。

1. 「**グループ化プレビュー**」セクションで、「**グループ化を追加**」をクリックして、レポート内の情報の整理方法を定義します。レポート内のグループ化の表示についてプレビューを次に示します。

1. レポート内の情報を整理する方法を表すフィールドの名前を入力し、ドロップダウンリストに表示されたらクリックします。
1. （オプションおよび条件付き）更新されたリストの表示で、グループ化の結果を展開するよりも折りたたんだ状態で表示させたい場合は、**デフォルトでこのグループ化を折りたたむ**&#x200B;を選択します。この設定はデフォルトでは無効になっており、グループ化の結果は常に展開されたリストで表示されます。

   更新されたリストと従来のリストについて詳しくは、「更新されたリストと従来のリストの違い」の記事の [Adobe Workfront でのリストの概要](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)の節を参照してください。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* リストを表示しているときにグループ化を手動で調整すると、ログアウトするまで Workfront に手動の設定が記憶されます。再度ログインすると、この設定に従ってリストが表示されます。
   >* グループ化の結果は、グラフ要素または従来のリストからアクセスした後で常に展開されて表示されます。この場合、この設定は無視されます。

1. 手順 4、5、6 を繰り返して、追加のグループ化を定義します。\
   情報を整理するために、最大 3 つのグループを定義できます。マトリックスレポートを作成すると、最大 4 つのグループに分けて情報を整理できます。マトリックスレポートについて詳しくは、[マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)を参照してください。

1. **グループ化を保存** をクリックして、現在のグループ化を自分の変更に置き換えます。
