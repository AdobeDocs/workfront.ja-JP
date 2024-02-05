---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: ユーザー更新の環境設定の指定
description: ユーザーがオブジェクトの[!UICONTROL 更新]領域にコメントを追加する際に特定の機能にアクセスできるようにする設定を指定できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 92%

---

# ユーザー更新の環境設定の指定

ユーザーがオブジェクトの[!UICONTROL 更新]領域にコメントを追加する際に特定の機能にアクセスできるようにする環境設定を指定できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、[!UICONTROL System Administrator]のアクセスレベルが必要です。</p><p>グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーが更新で画像を追加できるようにする

デフォルトでは、ユーザーは更新に画像を追加できません。この環境設定を有効にすると、ユーザは更新に画像を添付できるようになります。この環境設定は、[!DNL Workfront] インスタンスのすべての領域のすべての更新に適用されます。

>[!NOTE]
>
>* 更新で保存された画像は、ドキュメントストレージ制限に考慮されます。詳しくは、[ドキュメントストレージ制限の確認ク](../../../documents/managing-documents/check-document-storage.md)を参照してください。
>* 画像には、 [!UICONTROL 更新] タブをクリックし、 [!UICONTROL ドキュメント] 下の領域 [!UICONTROL メインメニュー].
>

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、**[!UICONTROL 設定]**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。
1. 左パネルで、**[!UICONTROL インターフェイス]**／**[!UICONTROL フィードの更新]**&#x200B;を選択します。
1. 「**[!UICONTROL 環境設定]**」タブを選択します。

   ![フィードの更新のユーザー環境設定](assets/updatefeeds-preferences-350x137.png)

1. 「**[!UICONTROL ユーザーが更新で画像を追加できるようにする]**」チェックボックスを選択します。
1. 「**[!UICONTROL 保存]**」を選択します。

   この設定が有効になっている場合、いつでも無効にすることができます。更新で既に投稿された画像は、オブジェクトの[!UICONTROL 更新]領域に残ります。
