---
title: 監査ログの表示と書き出し
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: システム内のすべての監査ログ、または特定のフィルタリング条件を満たす監査ログを表示できます。監査ログはエクスポートすることもできます。監査ログには、過去 90 日間にシステムでトリガーされたユーザーの変更がリストされます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '322'
ht-degree: 100%

---

# 監査ログの表示と書き出し

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

システム内のすべての監査ログ、または特定のフィルタリング条件を満たす監査ログを表示できます。監査ログはエクスポートすることもできます。

監査ログには、過去 90 日間にシステムでトリガーされたユーザーの変更がリストされます。

すべての監査ログのタイプとその生成内容については、[監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>プラン </p> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 監査ログの表示

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン![](assets/main-menu-icon.png)、**設定**![](assets/gear-icon-settings.png)の順にをクリックします。

1. 左側のパネルで、**システム／監査ログ**&#x200B;をクリックします。
1. 「**ログタイプ**」ドロップダウンメニューで、表示する監査ログのタイプを選択します。

   デフォルトでは、「**すべてのログタイプ**」が選択されています。

   表示できるすべての監査ログタイプとそれらに含まれる情報のリストについては、[監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)を参照してください。

1. （オプション）使用可能な任意のフィルターを設定します。

   >[!NOTE]
   >
   >「アクションタイプ」ドロップダウンメニューのオプションは、選択した監査ログによって異なります。

   ![](assets/audit-logs.jpg)

1. 「**適用**」をクリックします。
1. （オプション）「**フィルターをクリア**」をクリックして、フィルターに加えられた変更をリセットします。

## 監査ログのエクスポート

1. Adobe Workfront の右上にある&#x200B;**メインメニュー**&#x200B;アイコン（![](assets/main-menu-icon.png)）をクリックし、**設定**&#x200B;アイコン（![](assets/gear-icon-settings.png)）をクリックします。

1. 左側のパネルで、**システム／監査ログ**&#x200B;をクリックします。

1. 「**ログタイプ**」ドロップダウンメニューで「監査ログ」を選択します。

   デフォルトでは「**すべてのログタイプ**」が選択されています。

1. 使用可能なフィルターのいずれかを設定し、「**適用**」をクリックします。

   >[!IMPORTANT]
   >
   >一度に 50,000 件を超えるログをエクスポートすることはできません。Workfront では、ページに表示されるログの数ではなく、設定したフィルターに基づいてログがエクスポートされます。フィルターされたログの合計数は、ページの右下に表示されます。

1. 「**エクスポート**」をクリックします。
