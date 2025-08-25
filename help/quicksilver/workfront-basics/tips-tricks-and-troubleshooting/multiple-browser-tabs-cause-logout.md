---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 複数のブラウザータブが原因で、Workfrontがログアウトする
description: 複数のブラウザータブを開いている場合、Workfront は自動的にログアウトすることがあります。
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 30%

---

# 複数のブラウザータブが原因で、Workfrontがログアウトする

>[!IMPORTANT]
>
>この問題は、Adobe IMSにオンボーディングされた組織にのみ発生します。

## 問題

ユーザーが複数のブラウザータブを開き、しばらく非アクティブになっているタブをクリックすると、タブセッションの有効期限が切れます。 ユーザーが開いていたページは表示されず、代わりに次のメッセージが表示されます。

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## 理由

この動作は、組織が設定したセキュリティ対策であるポリシーベースの認証（PBA）が原因です。 タブが組織の PBA 設定で設定された制限時間を超えて非アクティブになっている場合、タブセッションは期限切れになります。

## ソリューション

解決策は、Workfrontにログインしている別のタブでアクティブになっているかどうかによって異なります。

* アクティブな Workfront タブが開いている場合は、期限切れのタブをリロードします。期限が切れる前に開いていたページに戻ります。

* アクティブな Workfront タブが開いていない場合は、もう一度 Workfront にログインします。
