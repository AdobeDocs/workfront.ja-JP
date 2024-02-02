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
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: ht
source-wordcount: '187'
ht-degree: 100%

---

# ユーザーのその他のグループを一括編集する

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

## 問題：

一括編集時に、単一の「その他のグループ」を多数のユーザーに追加しようとしました。
 変更を保存した後、既存の「その他のグループ」はすべて削除され、新しい「その他のグループ」のみが残りました。

## 回答：

結果の動作は、選択したユーザーの現在のグループメンバーシップによって異なります。

* 選択したユーザーのすべてが「その他のグループ」メンバーシップと完全に一致する場合…
ユーザーを選択して「[!UICONTROL 編集]」を選択すると、「[!UICONTROL その他のグループ]」フィールドには、これらのユーザーが属するすべてのグループの完全なリストが表示されます。


* 選択したユーザーが異なる他のグループメンバーシップを持っている場合…
ユーザーを選択して「[!UICONTROL 編集]」を選択すると、「[!UICONTROL その他のグループ]」フィールドは空白になります。

「**[!UICONTROL 変更を保存]**」をクリックすると、「その他のグループ」フィールドに表示されている内容が保存されます。

フィールドの以前のコンテンツは上書きされます。
