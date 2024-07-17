---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: ドキュメントの moveToFolder アクションが機能しない
description: Document moveToFolder/フォルダの移動アクションを使用すると、422 エラーが返されます。
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
source-git-commit: 53edc378e000e5b36fe0ce5750b8917fb13cfde1
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 2%

---

# ドキュメントの moveToFolder アクションが機能しない

## 問題

Document オブジェクトの `moveToFolder` アクションを使用すると、422 エラーが返されます。

または

Workfront Fusion のAdobe Authenticator モジュールを使用してこのアクションを使用した場合、ドキュメントは移動しませんが、エラーがあることを示す表示はありません。 エラーは同じですが、Adobe Authenticator モジュールに表示されません。

## ソリューション

このアクションで 422 エラーが発生する原因の 1 つは、アクションがリンクされたフォルダー内のドキュメントを別のリンクされたフォルダーに移動しようとしていることです。

移動するドキュメントが、リンクされたフォルダーにまだ存在していないことを確認します。
