---
title: 監査ログの表示と書き出し
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: システム内のすべての監査ログ、または特定のフィルタリング条件を満たす監査ログを表示できます。監査ログはエクスポートすることもできます。監査ログには、過去 90 日間にシステムでトリガーされたユーザーの変更がリストされます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 95%

---

# 監査ログの表示と書き出し

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

システム内のすべての監査ログ、または特定のフィルタリング条件を満たす監査ログを表示できます。監査ログはエクスポートすることもできます。

監査ログには、過去 90 日間にシステムでトリガーされたユーザーの変更がリストされます。

すべての監査ログのタイプとその生成内容については、[監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 監査ログの表示

{{step-1-to-setup}}

1. 左側のパネルで、**システム／監査ログ**&#x200B;をクリックします。
1. 「**ログタイプ**」ドロップダウンメニューで、表示する監査ログのタイプを選択します。

   デフォルトでは、「**すべてのログタイプ**」が選択されています。

   表示できるすべての監査ログタイプとそれらに含まれる情報のリストについては、[監査ログ](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)を参照してください。

1. （オプション）使用可能な任意のフィルターを設定します。

   >[!NOTE]
   >
   >「アクションタイプ」ドロップダウンメニューのオプションは、選択した監査ログによって異なります。

   ![監査ログ](assets/audit-logs.jpg)

1. 「**適用**」をクリックします。
1. （オプション）「**フィルターをクリア**」をクリックして、フィルターに加えられた変更をリセットします。

## 監査ログのエクスポート

{{step-1-to-setup}}

1. 左側のパネルで、**システム／監査ログ**&#x200B;をクリックします。

1. 「**ログタイプ**」ドロップダウンメニューで「監査ログ」を選択します。

   デフォルトでは「**すべてのログタイプ**」が選択されています。

1. 使用可能なフィルターのいずれかを設定し、「**適用**」をクリックします。

   >[!IMPORTANT]
   >
   >一度に 50,000 件を超えるログをエクスポートすることはできません。Workfront では、ページに表示されるログの数ではなく、設定したフィルターに基づいてログがエクスポートされます。フィルターされたログの合計数は、ページの右下に表示されます。

1. 「**エクスポート**」をクリックします。
