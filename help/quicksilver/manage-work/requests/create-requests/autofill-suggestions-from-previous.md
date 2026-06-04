---
title: 以前のリクエストのデータを使用して、リクエストを自動補完します
content-type: reference
description: AIを活用して、以前のリクエストのデータを使用してリクエストフィールドを自動補完できます。
author: Alina
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EJR8tFVdc-sYRL5kXf-Ex9WExL0hcbkhQ1ZwEmpmU-s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 23%

---

# 以前のリクエストのデータを使用して、リクエストを自動補完します

AIは、過去のリクエストにもとづいてリクエストフィールドを自動補完するのに役立ちます。 リクエストを送信する前に、これらの提案を承認または却下できます。

オートコンプリートでは、既に入力したフィールドは上書きされません。

ユーザーは、他の方法ではアクセスできないデータの提案を受け取りません。

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
   <td> <p>コントリビューター以上</p>
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

## フォームの入力時に候補を表示する

オートコンプリート機能は、フォームへの入力中にフィールド値を提案する可能性があります。 リクエストフィールドに値を入力すると、Workfrontはこれらの値と以前のリクエストを比較します。 入力された値が以前のリクエストの同様のコンテキスト内の他のフィールド値と密接に相関している場合、Workfrontはこれらの値を提案します。

例えば、ある診療所が常に同じ請求コードを使用している場合、Workfrontは、クリニック名を入力するときに適切なフィールドに請求コードを入力するよう提案します。

以前のリクエストに基づいて提案を使用するには：

1. リクエストの作成を開始します。

   手順については、[ リクエストの作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

1. フィールドへの入力を開始します。

   フィールドに入力すると、他のフィールドに候補が表示される場合があります。

1. フィールドの候補ごとに、そのフィールドの&#x200B;**承諾**&#x200B;または&#x200B;**却下**&#x200B;を選択します。

   ![提案の承認または拒否](assets/accept-reject-suggestion.png)

   または

   ページの上部にある「**すべてを受け入れる**」または「**すべてを却下する**」を選択して、すべての提案を受け入れるか却下します。

   >[!NOTE]
   >
   >レビューされていない提案は、リクエストを送信すると自動的に承認されます。
