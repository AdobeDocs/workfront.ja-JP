---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 複数のブラウザータブが原因で、Workfront からログアウトされる
description: 複数のブラウザータブを開いている場合、Workfront は自動的にログアウトすることがあります。
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 440640f5b916b76096c99eed8253236de477a02a
workflow-type: tm+mt
source-wordcount: '164'
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

* アクティブな Workfront タブが開いている場合は、期限切れのタブをリロードします。期限が切れる前に開いていたページに戻ります。

* アクティブな Workfront タブが開いていない場合は、もう一度 Workfront にログインします。
