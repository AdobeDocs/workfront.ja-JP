---
product-area: reporting
navigation-topic: reporting-elements
title: ユーザーベースのワイルドカードを使用してレポートを一般化する
description: 特定のレポート要素を作成する際に、特定の情報ではなくワイルドカードを使用して、レポートを一般化できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# ユーザーベースのワイルドカードを使用してレポートを一般化する

特定のレポート要素を作成する際に、特定の情報ではなくワイルドカードを使用して、レポートを一般化できます。 例えば、特定のユーザーに割り当てられたタスクを示すレポートを作成する場合は、フィルターの「割り当て先」フィールドでユーザーの名前を使用できます。 ただし、ログインしたユーザーに割り当てられたタスクを表示するレポートを作成する場合は、そのユーザーが誰であるかに関係なく、そのユーザーに関する情報を表示するワイルドカードを使用できます。 この方法では、レポートを 1 回作成しますが、フィルターにワイルドカードを使用するので、他のユーザーが読み取るたびに異なる結果が生成されます。

次のレポート要素を作成する際に、ユーザーベースのワイルドカードを使用できます。

* フィルター
* カスタムプロンプト
* 列のルールを追加する際に表示

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
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートのレポート要素を編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>レポートのレポート要素を編集するためのレポートに対する権限の管理</p> <p>ビューまたはフィルターに対する権限を管理して編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ワイルドカード変数を追加する前に、レポートを作成する必要があります。

レポートの作成手順については、 [レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## ハウツー手順

ユーザーベースのワイルドカードをレポートに挿入するには、次の手順に従います。

1. ユーザーベースのワイルドカードを挿入するレポートに移動します。
1. クリック **レポートのアクション**&#x200B;を、 **編集**.

1. 次をクリック： **フィルター** タブをクリックします。
1. クリック **フィルタールールを追加**.
1. フィルターに使用するフィールドの名前を入力します。\
   ユーザーオブジェクトまたはユーザーに関する情報を参照するフィールドを入力する必要があります。
1. 選択 **次と等しい** （フィルター変数のドロップダウンメニュー）を使用します。

   >[!TIP]
   >
   >常に **次と等しい** Adobe Workfrontでワイルドカードを使用する場合のフィルター変数

1. 内 **名前の入力を開始…** ボックス、タイプ： `$$USER.ID` または `$$USER.name` レポートに、ログインしたユーザーの名前に基づく情報を表示する場合。 ログインしたユーザーのグループ、チーム、会社、その他の情報を参照する他のワイルドカードを挿入できます。

   ユーザーベースのワイルドカードの完全なリストについては、 [ワイルドカードフィルター変数](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. 「**保存して閉じる**」をクリックします。

## 追加情報

関連項目：

* [基本レポート作成プログラム](https://one.workfront.com/s/basic-report-creation-program)
* [ワイルドカードフィルター変数](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Adobe Workfrontでフィルターを作成または編集](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [レポートにプロンプトを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [ビューでの条件付き書式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
