---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: ホームワークリストに重複した承認プロセスが表示されます
description: ホームワークリストに同じ承認が複数表示されます。
feature: Get Started with Workfront
exl-id: 01e22849-2601-4c2a-b1cf-193a484bfc0b
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---

# 重複した承認プロセスが [!UICONTROL ホームの作業リスト]

## 問題

同じ承認が [!UICONTROL ホームの作業リスト].

## 原因

個々のユーザーとして、またチームのメンバーとして承認に割り当てられている。

![](assets/stages-approval-350x208.png)

## 解決策

承認プロセスを設定するユーザーは、承認プロセスに追加する個々のユーザーが、承認プロセスに割り当てられたチームのメンバーでないことを確認する必要があります。

個々のユーザーとして、またチームの一部として割り当てられ、承認が 2 回表示される場合は、エントリの 1 つに対してのみ決定する必要があります。
