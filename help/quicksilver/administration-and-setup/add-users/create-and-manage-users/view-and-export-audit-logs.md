---
title: 監査ログの表示と書き出し
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: システム内のすべての監査ログ、または特定のフィルタリング条件を満たす監査ログを表示できます。 監査ログを書き出すこともできます。 監査ログは、過去 90 日間にシステムでトリガーされたユーザーの変更をリストします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 監査ログの表示と書き出し

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

システム内のすべての監査ログ、または特定のフィルタリング条件を満たす監査ログを表示できます。 監査ログを書き出すこともできます。

監査ログは、過去 90 日間にシステムでトリガーされたユーザーの変更をリストします。

すべての監査ログのタイプと、その生成内容について詳しくは、 [監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> <p>計画 </p> <p>Workfront管理者である。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 監査ログの表示

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **システム/監査ログ**.
1. 内 **ログタイプ** ドロップダウンメニューから、表示する監査ログのタイプを選択します。

   **すべてのログタイプ** はデフォルトで選択されています。

   表示できるすべての監査ログの種類とそれらに含まれる情報の一覧については、 [監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. （オプション）使用可能な任意のフィルターを設定します。

   >[!NOTE]
   >
   >Action Type ドロップダウンメニューのオプションは、選択した監査ログによって異なります。

   ![](assets/audit-logs.jpg)

1. クリック **適用**.
1. （オプション）「 **フィルターをクリア** ：フィルターに加えた変更をリセットします。

## 監査ログの書き出し

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **システム/監査ログ**.

1. 内 **ログタイプ** ドロップダウンメニューから、監査ログを選択します。

   **すべてのログタイプ** はデフォルトで選択されています。

1. 使用可能なフィルターのいずれかを設定し、「 **適用**.

   >[!IMPORTANT]
   >
   >一度に 50,000 件を超えるログを書き出すことはできません。 Workfrontは、ページに表示されるログの数ではなく、設定したフィルターに基づいてログを書き出します。 フィルター済みログの合計数をページの右下隅に表示できます。

1. クリック **書き出し**.
