---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 複数のブラウザータブが原因で、Workfront からログアウトされる
description: 複数のブラウザータブを開いている場合、Workfront は自動的にログアウトすることがあります。
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 42%

---

# 複数のブラウザータブが原因で、Workfront からログアウトされる

## 問題

ユーザーが複数のブラウザータブを開き、しばらく非アクティブだったタブをクリックすると、タブセッションの有効期限が切れます。 ユーザーは開いているページを見ることができず、代わりに次のメッセージが表示されます。

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## 理由

この動作は、組織で設定されたセキュリティ対策であるポリシーベース認証（PBA）によるものです。 タブが組織のPBA設定で設定された時間制限を超えて非アクティブになっている場合、タブセッションは期限切れになります。

## ソリューション

解決策は、Workfrontにログインしている別のタブでアクティブになっているかどうかによって異なります。

* アクティブな Workfront タブが開いている場合は、期限切れのタブをリロードします。 期限が切れる前に開いていたページに戻ります。

* アクティブな Workfront タブが開いていない場合は、もう一度 Workfront にログインします。
