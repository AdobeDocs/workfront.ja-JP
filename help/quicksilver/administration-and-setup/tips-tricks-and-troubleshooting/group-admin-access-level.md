---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: グループ管理者は、管理しているグループ管理者よりも高いアクセス権を持っている必要があります
description: グループ管理者が、管理するアクセスレベルよりも低いアクセスレベルの権限を持っている場合、低いアクセスレベルの表示、変更、割り当てを行うことはできません。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# グループ管理者は、管理しているグループ管理者よりも高いアクセス権を持っている必要があります

グループ管理者が、管理するアクセスレベルよりも低いアクセスレベルの権限を持っている場合、低いアクセスレベルの表示、変更、割り当てを行うことはできません。

## 問題

グループ管理者にチームの表示権限を持つ変更済 Planner アクセス・レベルが割り当てられているが、特定のユーザーにチームの編集権限を持つ Worker アクセス・レベルが割り当てられている場合、グループ管理者は変更済 Worker アクセス・レベルを操作できません。

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>このロジックは、「設定を微調整」ドロップダウンメニューにも適用されます。 両方のアクセスレベルに編集アクセス権を持つことができますが、設定を微調整ドロップダウンメニューの設定は、グループ管理者にとってより高い値にする必要があります。
> ![](assets/fine-tune-your-settings.png)

## 解決策

グループ管理者は、管理している権限よりもアクセスレベルのすべての領域に対して、高い権限を持つ必要があります。