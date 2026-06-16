---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 従来のポートフォリオをAdobe クラウドストレージに変換
description: 既存の従来のWorkfront ストレージポートフォリオを、システム環境設定の「ストレージ環境設定」エリアからAdobe クラウドストレージに変換します。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 11%

---

# 従来のポートフォリオをAdobe クラウドストレージに変換

Workfront管理者は、既存の従来のWorkfront ストレージポートフォリオを、システム環境設定の「ストレージ環境設定」領域からAdobe クラウドストレージに変換できます。 ポートフォリオを変換すると、他のAdobe クラウドストレージポートフォリオと同じように動作します。

変換されたポートフォリオの動作と子オブジェクトの影響について詳しくは、[Adobe クラウドストレージ上のWorkfrontへの移行](/help/quicksilver/review-and-approve-work/workfront-storage.md)の[ オブジェクトポータビリティ ](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意のワークフローパッケージ</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ポートフォリオの変換前

従来のWorkfront ストレージポートフォリオを変換する前に、次の点を考慮してください。

* コンバージョンは、ポートフォリオ自体にのみ影響します。 従来のWorkfront ストレージを使用する子プロジェクトとプログラムは、従来のストレージに残ります。
  >[!NOTE]
  >
  >子レガシープログラムは、誰かが手動でAdobe クラウドストレージプロジェクトを追加した場合にのみ、Adobe クラウドストレージに自動的に変換されます。
* ポートフォリオ上のドキュメントとドキュメントフォルダーは、変換後も従来のWorkfront ストレージに残ります。
* 変換後、従来のWorkfront ストレージプロジェクトをポートフォリオに追加することはできません。

## 従来のポートフォリオをAdobe クラウドストレージに変換

1つ以上の従来のWorkfront ストレージポートフォリオをAdobe クラウドストレージに変換するには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。

1. 「**ストレージ環境設定**」セクションまでスクロールします。

1. 「**Adobe クラウドストレージに変換するポートフォリオを選択**」フィールドで、1つ以上のレガシーWorkfront ストレージポートフォリオを選択します。

1. 「**保存**」をクリックします。

   ポートフォリオが変換されたときに何が起こるかを説明する確認メッセージが表示されます。

   * 従来のWorkfront ストレージプロジェクトをポートフォリオに移動できなくなります。
   * ポートフォリオで作成されたすべての新規プロジェクトでは、Adobe クラウドストレージが使用されます。
   * Frame.ioは、ポートフォリオのAdobe クラウドストレージプロジェクトのドキュメントのビューアーです。
   * 従来のWorkfront ストレージを使用する子プロジェクトは、従来のストレージに残ります。
   * 子プログラムはレガシーストレージに残ります。

1. 「**変換**」をクリックして確定します。

   選択したポートフォリオは、Adobe クラウドストレージに変換されます。
