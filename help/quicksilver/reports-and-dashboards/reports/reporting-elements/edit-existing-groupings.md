---
title: 既存のグループを編集
description: 既存のグループを編集
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 既存のグループを編集

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

最初に作成した既存のグループまたは自分と共有されていた既存のグループをカスタマイズできます。 次に、新しいグループとして保存できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートのグループ化を編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>レポートのグループ化を編集するための、レポートに対する権限の管理</p> <p>グループに対する権限の管理 </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

グループを編集する前に、グループを作成する必要があります。

グループ化の作成について詳しくは、 [Adobe Workfrontでのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## ハウツー手順

1. カスタマイズするグループ化を含むオブジェクトのリストに移動します。
1. 次をクリック： **グループ化** アイコン
1. カスタマイズするグループを選択し、 **編集** アイコン

   ![編集アイコンを選択します。](assets/customizegrouping-nwe-standard-350x291.png)

   グループ化をカスタマイズするためのインターフェイスビルダーが開きます。

1. 内 **グループ化プレビュー** セクションで、 **グループを追加** を使用して、レポート内の情報の整理方法を定義します。 レポートでのグループ化の表示のプレビューを次に示します。

1. レポート内の情報を整理する方法を表すフィールドの名前を入力し、ドロップダウンリストに表示されたらクリックします。
1. （オプションおよび条件付き）更新されたリストを表示する場合、 **デフォルトでこのグループ化を折りたたむ** を指定します。 この設定はデフォルトでは無効になっており、グループ化の結果は常に展開されたリストに表示されます。

   更新リストと従来のリストについて詳しくは、この記事の「更新済みリストと従来のリストの違い」の節を参照してください。 [Adobe Workfrontのリストの概要](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* リスト表示時にグループを手動で調整すると、Workfrontでは、ログアウトするまで手動の設定が記憶されます。 再度ログインすると、この設定に従ってリストが表示されます。
   >* グループ化の結果は、グラフ要素または従来のリストからアクセスした後は常に展開されて表示されます。 この場合、この設定は無視されます。


1. 手順 4、5、6 を繰り返して、追加のグループを定義します。\
   情報を整理するために、最大 3 つのグループを定義できます。 マトリックスレポートを作成すると、最大 4 つのグループに分けて情報を整理できます。 マトリックスレポートの詳細については、 [マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. クリック **新しいグループとして保存** 現在のグループを変更で置き換えます。
