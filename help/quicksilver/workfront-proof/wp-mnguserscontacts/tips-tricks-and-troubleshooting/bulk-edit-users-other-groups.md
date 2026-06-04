---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: ユーザーのその他のグループを一括編集する
description: 一括編集時に、単一の「その他のグループ」を多数のユーザーに追加しようとしました。 変更を保存した後、既存の「その他のグループ」はすべて削除され、新しい「その他のグループ」のみが残りました。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 170
ht-degree: 55%

---

# ユーザーのその他のグループを一括編集する

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。 [!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

## 問題：

一括編集時に、1つの他のグループを多数のユーザーに追加しようとしました。
変更を保存した後、既存のその他のグループはすべて削除され、新しい他のグループのみが残りました。

## 回答：

結果の動作は、選択したユーザーの現在のグループメンバーシップによって異なります。

* 選択したユーザーの他のグループ メンバーシップがすべて一致する場合…
ユーザーを選択して[!UICONTROL edit]を選択すると、[!UICONTROL その他のグループ ] フィールドに完全なリストが表示されます
そのユーザーが属するすべてのグループのリストです。

* 選択したユーザーが他のグループのメンバーシップを持っている場合…
ユーザーを選択して[!UICONTROL 編集]をクリックすると、[!UICONTROL その他のグループ ] フィールドが空白になります。

「**[!UICONTROL 変更を保存]**」をクリックすると、「その他のグループ」フィールドに表示されている内容が保存されます。

フィールドの以前のコンテンツは上書きされます。
