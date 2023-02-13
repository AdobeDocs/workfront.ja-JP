---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: ユーザー名は既に使用されています
description: ユーザー名が既に使用されているというエラーが表示されたら、これらのヒントをお読みください。
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# ユーザー名は既に使用されています

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL システム管理者 ]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 質問

新しいユーザーを作成する場合、 [!UICONTROL おっと] ユーザー名が既に使用されていることを示すエラーが表示されます。 システム内にこの電子メールが存在しません。 これが表示される理由

## 解決策

これは、現在の [!DNL Adobe Workfront] インスタンス。 ユーザーは、同じユーザー名または電子メールアドレスを別々のインスタンスで持つことができます。 例えば、ユーザー A は以下の電子メールアドレスを [!DNL Workfront] アカウント：usera@company1.comおよびusera@company2.com.

>[!NOTE]
>
>プライマリ [!DNL Workfront] 同じクラスター上の別のWorkfrontインスタンスに存在する場合、管理者は同じユーザー名または電子メールアドレスを持つことはできません。
>
>インスタンスが異なるクラスター上にある場合、プライマリ管理者は同じユーザー名または E メールアドレスを持つことができます。 インスタンスが存在するクラスターを表示できます [!UICONTROL 設定] > [!UICONTROL システム] > [!UICONTROL 顧客情報].

### ユーザー名がインスタンス内で一意であるかどうかを確認します。

ユーザー名と電子メールアドレスが現在の [!DNL Workfront] インスタンス：

1. を [!DNL Workfront] 管理者、 **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ユーザー]**.
1. ユーザーのリストで、 **[!UICONTROL 電子メール]** 列を使用して、重複する E メールがないことを確認します。
1. ユーザー名の列をビューに追加します。

   1. 内 **[!UICONTROL 表示]** ドロップダウンメニューで、 **[!UICONTROL 表示をカスタマイズ]**.
   1. クリック **[!UICONTROL 列を追加]**.
   1. 検索フィールドに、「 *[!UICONTROL ユーザー名]*.
   1. 選択 **[!UICONTROL ユーザー]** > **[!UICONTROL ユーザー名]**.
   1. ビューを保存します。\
      これにより、重複を検索できるユーザー名がビューに表示されます。

1. ユーザーのリストで、 **[!UICONTROL ユーザー名]** 列を使用して、重複するユーザー名がないことを確認します。
