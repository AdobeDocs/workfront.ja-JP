---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: ユーザーアップデートの環境設定を行う
description: ユーザーがオブジェクトの[!UICONTROL 更新]領域にコメントを追加する際に特定の機能にアクセスできるようにする設定を指定できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 71%

---

# ユーザー更新の環境設定の指定

<!--Audited: 08/2025-->

ユーザーがオブジェクトの[!UICONTROL 更新]領域にコメントを追加する際に特定の機能にアクセスできるようにする環境設定を指定できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>システム管理者：これらの手順をシステムレベルで実行します。 </p>
   <p>プランナー：グループのマネージャーであることに加え、そのグループに対してこれらの手順を実行します。</p></td>
  </tr> 
 </tbody> 
</table>

*このテーブルの詳細については、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## ユーザーが更新で画像を追加できるようにする

デフォルトでは、ユーザーは更新に画像を追加できません。この環境設定を有効にすると、ユーザは更新に画像を添付できるようになります。この環境設定は、[!DNL Workfront] インスタンスのすべての領域のすべての更新に適用されます。

>[!NOTE]
>
>* 更新で保存された画像は、ドキュメントストレージ制限に考慮されます。詳しくは、[ドキュメントストレージ制限の確認ク](../../../documents/managing-documents/check-document-storage.md)を参照してください。
>* 画像は、オブジェクト上の[!UICONTROL 更新]タブからアクセスでき、[!UICONTROL メインメニュー]の[!UICONTROL ドキュメント]エリアでも使用できます。
>

1. **[!UICONTROL の右上隅にある]** メインメニュー ![&#x200B; アイコン &#x200B;](assets/main-menu-icon.png) メインメニューアイコン [!DNL Adobe Workfront] をクリックし、**[!UICONTROL 設定]**![&#x200B; 歯車設定アイコン &#x200B;](assets/gear-icon-settings.png) をクリックします。
1. 左パネルで、**[!UICONTROL インターフェイス]**／**[!UICONTROL フィードの更新]**&#x200B;を選択します。
1. 「**[!UICONTROL 環境設定]**」タブを選択します。

   ![フィードの更新のユーザー環境設定](assets/updatefeeds-preferences-350x137.png)

1. 「**[!UICONTROL ユーザーが更新で画像を追加できるようにする]**」チェックボックスを選択します。
1. 「**[!UICONTROL 保存]**」を選択します。

   この設定が有効になっている場合、いつでも無効にすることができます。更新で既に投稿された画像は、オブジェクトの[!UICONTROL 更新]領域に残ります。
