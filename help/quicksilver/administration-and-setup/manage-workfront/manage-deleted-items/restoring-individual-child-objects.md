---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 個々の子オブジェクトの復元
description: ここでは、Adobe Workfrontの実稼動環境またはプレビュー環境から削除されてから 30 日未満である個々の子オブジェクトを復元する方法について説明します。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 88%

---

# 個々の子オブジェクトの復元

ここでは、Adobe Workfrontの実稼動環境またはプレビュー環境から削除されてから 30 日未満である個々の子オブジェクトを復元する方法について説明します。

Workfront 管理者は、各 Workfront インスタンスでプロジェクト、タスク、イシューおよびドキュメントを復元できます。詳しくは、[削除した項目を復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。ただし、タスク、イシュー、ドキュメント、カスタムフォーム、時間、メモなどのオブジェクトを、親オブジェクトから独立して復元できるのは、Workfront データベースチームだけです。

実稼働環境のデータは、サンドボックスのプレビューで最大 7 日間使用できます。つまり、次の方法で、サンドボックスプレビュー環境からスタンドアロンデータを書き出すことができます。

* キックスタート
* レポートの作成と結果の書き出し

Workfront からのデータの書き出しについて詳しくは、[データを書き出し](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)を参照してください。

書き出したデータは、次の方法で読み込むことができます。

* 手動（書き出したレポートを使用する場合）
* 一括（キックスタートを使用している場合）

  キックスタートを使用して Workfront にデータを読み込む方法について詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込み](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

サンドボックスプレビュー環境は、週末のメンテナンス期間中に更新されます。

サンドボックスプレビュー環境のメンテナンス期間について詳しくは、[Adobe のステータスサイト](https://status.adobe.com/ja)を参照してください。

>[!IMPORTANT]
>
>ドキュメントは、このような復元方法の例外となります。プレビュー環境から手動でダウンロードし、実稼動環境に再度アップロードすることができます。ドキュメントを一括でダウンロードおよびアップロードする場合は、Workfront からのデータの復元をリクエストする必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## データの復元に必要な情報

削除したオブジェクトをデータベースチームが復元する必要があると判断した場合は、そのオブジェクトに関する情報を収集します。データベース管理者がオブジェクトを検索し、復元を開始するには、次の情報が必要です。

* オブジェクト名
* オブジェクトタイプ（タスク、イシュー、プロジェクトなど）
* 削除の推測日時
* オブジェクト GUID（可能な場合）

  オブジェクトの GUID を検索する際は、次の情報を参照してください。

   * GUID は、オブジェクトの操作でトリガーされるメール通知（割り当て、コメントなど）を参照することで見つかります。
   * URL の末尾で GUID を確認する例：`yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

この情報を収集したら、またはサポートが必要な場合は、カスタマーサポートチーム 844-306-HELP（4357）にお電話いただくか、チケットをオンラインで送信してください。

## データの復元プロセス

1. カスタマーサポートチームがお客様の情報を受け取った後、カスタマーサポートチームに情報がエスカレーションされます。
1. カスタマーサポートチームがデータベースチームに連絡します。
1. データベースチームが復元されるデータを確認できれば、ETA に関するより正確な見積もりを提供できます。リストアには通常 3 日かかりますが、復元するデータの種類と量によっては、これより長い時間がかかる場合があります。
1. データベースチームは、情報をサンドボックスプレビュー環境に復元します。この環境で、復元したデータを確認することができます。カスタマーサポートチームは、サンドボックスプレビューでデータが見つかったらお知らせします。
1. サンドボックスでの復元で問題がなければ、カスタマーサポートチームに連絡します。カスタマーサポートチームがデータベースチームに連絡して、実稼動環境にデータを復元できることを通知します。
1. リクエストがクローズされる前に、復元されたデータを確認することができます。
