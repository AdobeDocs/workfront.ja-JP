---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: グループ管理者は、管理するユーザーよりも高いアクセス権を持っている必要があります
description: グループ管理者が管理するアクセスレベルよりも低い権限を持っている場合、低いアクセスレベルを表示、変更、割り当てることはできません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 157
ht-degree: 47%

---

# グループ管理者には管理対象のユーザーより高いアクセス権が必要

グループ管理者が管理するアクセスレベルよりも低い権限を持っている場合、低いアクセスレベルを表示、変更、割り当てることはできません。

## 問題

チームの表示権限を持つ変更済みのプランナーアクセスレベルがグループ管理者に割り当てられており、チームの編集権限を持つ作業者アクセスレベルが特定のユーザーに割り当てられている場合、グループ管理者は変更済みの作業者アクセスレベルを操作できません。

![ グループ管理者がアクセスを変更しました](assets/group-admin-modified-access.png)


>[!NOTE]
>
>このロジックは、設定の微調整ドロップダウンメニューにも適用されます。両方のアクセスレベルで編集アクセス権を持つことができますが、グループ管理者の場合は、設定の微調整ドロップダウンメニューの設定を高くする必要があります。
> ![設定を微調整](assets/fine-tune-your-settings.png)

## ソリューション

グループ管理者には、アクセスレベルのすべての領域において、管理対象のユーザーよりも高い権限が必要です。
