---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: ドキュメントの moveToFolder アクションが機能しない
description: Document moveToFolder/フォルダの移動アクションを使用すると、422 エラーが返されます。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 2%

---


# ドキュメントの moveToFolder アクションが機能しない

## 問題

Document オブジェクトの使用時 `moveToFolder` アクションを実行すると、422 エラーが返されます。

または

Workfront Fusion のAdobe Authenticator モジュールを使用してこのアクションを使用した場合、ドキュメントは移動しませんが、エラーがあることを示す表示はありません。 エラーは同じですが、Adobe Authenticator モジュールに表示されません。

## ソリューション

このアクションで 422 エラーが発生する原因の 1 つは、アクションがリンクされたフォルダー内のドキュメントを別のリンクされたフォルダーに移動しようとしていることです。

移動するドキュメントが、リンクされたフォルダーにまだ存在していないことを確認します。
