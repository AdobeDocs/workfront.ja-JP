---
title: クラシックレイアウトテンプレートの削除
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Classic Workfrontエクスペリエンスのレイアウトテンプレートは、Workfrontインターフェイスでは使用できなくなりましたが、Workfrontデータに影響が及ぶ場合があります。 これにより、レポートやダッシュボードのレイアウトテンプレート（「共有先」など）の影響を受けるフィールドに不整合が生じる可能性があります。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# レイアウトテンプレートの管理アクセス権の付与

Classic Workfrontエクスペリエンスのレイアウトテンプレートは、Workfrontインターフェイスでは使用できなくなりましたが、Workfrontデータに影響が及ぶ場合があります。 これにより、レポートやダッシュボードのレイアウトテンプレート（「共有先」など）の影響を受けるフィールドに不整合が生じる可能性があります。

クラシックレイアウトテンプレートを削除すると、これらの不整合を解決できます。 これらはWorkfrontインターフェイスでは使用できないので、を使用して削除するにはWorkfront API を使用する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p> </td> 
  </tr> 
 </tbody> 
</table>

## API 呼び出しを使用したクラシックレイアウトテンプレートの削除

ブラウザーの URL バーに API 呼び出しを入力し、Enter キーを押すことができます。 API 応答がブラウザーに表示されます。

>[!NOTE]
>
>グローバルレイアウトテンプレートとシステムレイアウトテンプレートは削除できません。

1. Workfrontにログインします。
1. 次の API 呼び出しを使用して、削除するレイアウトテンプレートを見つけます。
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 削除するレイアウトテンプレートの ID をメモしておきます。
1. 次の API 呼び出しを使用して、セッション ID を見つけます。
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >セッション ID を誰とも共有しないでください。

1. 以下の API 呼び出しに、レイアウトテンプレート ID とセッション ID を挿入します。
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 手順 4 の API 呼び出しをブラウザーの URL バーに貼り付け、Enter キーを押します。

   これにより、レイアウトテンプレートが削除されます。



