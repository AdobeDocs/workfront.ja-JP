---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境促進のトラブルシューティング
description: 環境の昇格に関する一般的な問題のトラブルシューティング。
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 6eab0af720852fd74182e371ca08aa40157ec2af
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---

# 環境促進のトラブルシューティング

環境プロモーションパッケージが停止または失敗した場合は、次の操作を試します。

* パッケージインストールが 10～15 分後に停止する場合、またはパッケージインストールが失敗する場合は、既存のパッケージを再アセンブリするか、新しいパッケージを作成します。

* パッケージのインストールに失敗した場合は、1 つ以上のオブジェクトに問題がある可能性があります。 オブジェクトを特定し、問題の特定に役立つエラーメッセージを確認します。 オブジェクトの問題に対処したら、パッケージを再アセンブルし、インストールを再試行します。

* それでもインストールで問題が発生する場合は、別のターゲット環境でインストールのレプリケーションを試みます。 選択したオブジェクトやインストールアクションを含め、元のインストールにできるだけ近づけます。

* パッケージがアセンブリされた後は、パッケージの内容を常に確認して、期待するオブジェクトが含まれていることを確認することをお勧めします。
