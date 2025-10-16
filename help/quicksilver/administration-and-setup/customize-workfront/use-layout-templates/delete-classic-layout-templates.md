---
title: Classic レイアウトテンプレートの削除
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Classic Workfront エクスペリエンスのレイアウトテンプレートは、Workfront インターフェイスでは使用できなくなりましたが、Workfront データに影響が及ぶ場合があります。これにより、レポートやダッシュボードのレイアウトテンプレート（共有先など）によって影響するフィールドに不整合が生じる可能性があります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 93%

---

# クラシックレイアウトテンプレートの削除

Classic Workfront エクスペリエンスのレイアウトテンプレートは、Workfront インターフェイスでは使用できなくなりましたが、Workfront データに影響が及ぶ場合があります。これにより、レポートやダッシュボードのレイアウトテンプレート（共有先など）によって影響するフィールドに不整合が生じる可能性があります。

Classic レイアウトテンプレートを削除すると、これらの不整合を解決できます。これらは Workfront のインターフェイスでは使用できないので、Workfront API を使用して削除する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## API 呼び出しを使用した Classic レイアウトテンプレートの削除

API 呼び出しは、ブラウザーの URL バーに入力して Enter を押すことでが実行できます。API 応答がブラウザーに表示されます。

>[!NOTE]
>
>グローバルレイアウトテンプレートおよびシステムレイアウトテンプレートは削除できません。

1. Workfront にログインします。
1. 次の API 呼び出しを使用して、削除するレイアウトテンプレートを見つけます。
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 削除するレイアウトテンプレートの ID をメモしておきます。
1. 次の API 呼び出しを使用して、セッション ID を見つけます。
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >セッション ID を誰とも共有しないでください。

1. 次の API 呼び出しに、レイアウトテンプレート ID とセッション ID を挿入します。
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 手順 4 の API 呼び出しをブラウザーの URL バーに貼り付け、Enter キーを押します。

   これにより、レイアウトテンプレートが削除されます。
