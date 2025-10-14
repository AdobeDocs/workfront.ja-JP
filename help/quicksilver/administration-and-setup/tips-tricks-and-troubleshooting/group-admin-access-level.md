---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: グループ管理者は、管理対象よりも高いアクセス権が必要
description: グループ管理者が管理するアクセス レベルよりも低いアクセス レベルの権限を持っている場合、下位のアクセス レベルを表示、変更、割り当てることはできません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 59%

---

# グループ管理者には管理対象のユーザーより高いアクセス権が必要

グループ管理者が管理するアクセス レベルよりも低いアクセス レベルの権限を持っている場合、下位のアクセス レベルを表示、変更、割り当てることはできません。

## 問題

チームの表示権限を持つ変更済みのプランナーアクセスレベルがグループ管理者に割り当てられており、チームの編集権限を持つ作業者アクセスレベルが特定のユーザーに割り当てられている場合、グループ管理者は変更済みの作業者アクセスレベルを操作できません。

![&#x200B; グループ管理者の変更されたアクセス &#x200B;](assets/group-admin-modified-access.png)


>[!NOTE]
>
>このロジックは、設定の微調整ドロップダウンメニューにも当てはまります。どちらのアクセスレベルでも編集アクセス権を持つことができますが、設定の微調整ドロップダウンメニューについては、グループ管理者の設定をより高くしておく必要があります。
> ![設定を微調整する &#x200B;](assets/fine-tune-your-settings.png)

## ソリューション

グループ管理者には、アクセスレベルのすべての領域において、管理対象のユーザーよりも高い権限が必要です。
