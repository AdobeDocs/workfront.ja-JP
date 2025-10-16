---
title: 以前のリクエストのデータを使用したリクエストのオートコンプリート
content-type: reference
description: AI を使用し、以前のリクエストのデータを使用して、リクエストフィールドをオートコンプリートできます。
author: Becky
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
source-git-commit: 1b7964b533093c4eee20d69a74512a145e207e29
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 18%

---

# 以前のリクエストのデータを使用したリクエストのオートコンプリート

AI は、以前のリクエストに基づいてリクエストフィールドをオートコンプリートするのに役立ちます。 リクエストを送信する前に、これらの提案を承認または却下できます。

オートコンプリートによって、既に入力済みのフィールドが上書きされることはありません。

ユーザーは、アクセス権のないデータの候補を受け取ることはありません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>投稿者以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  </td> 
  </tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td><p>リクエストキューにリクエストを追加するためのアクセス権</p> <p>既存のリクエストに対する表示またはそれ以上の権限</p> <p>リクエストキューの設定について詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>を参照してください。 </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## フォームに入力する際に候補を表示する

オートコンプリートは、フォームの入力中にフィールド値を提案できます。 リクエストフィールドに値を入力すると、Workfrontはそれらの値を以前のリクエストと比較します。 入力した値が以前のリクエストの同様のコンテキストにある他のフィールド値と密接に関連している場合、Workfrontはこれらの値を提案します。

例えば、あるクリニックが常に同じ請求コードを使用している場合、Workfrontは、クリニック名を入力する際に、適切なフィールドに請求コードを提案します。

以前のリクエストに基づいて候補を使用するには：

1. リクエストの作成を開始します。

   手順については、[&#x200B; リクエストの作成と送信 &#x200B;](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) を参照してください。

1. フィールドへの入力の開始。

   フィールドに入力すると、他のフィールドに候補が表示される場合があります。

1. フィールドの提案ごとに、そのフィールドに対して「**確定**」または **却下** を選択します。

   ![&#x200B; 提案を承認または却下 &#x200B;](assets/accept-reject-suggestion.png)

   または

   ページの上部で「**すべて承認**」または **すべて拒否** を選択して、すべての提案を承認または拒否します。

   >[!NOTE]
   >
   >レビューされていない提案は、リクエストを送信すると自動的に受け入れられます。
