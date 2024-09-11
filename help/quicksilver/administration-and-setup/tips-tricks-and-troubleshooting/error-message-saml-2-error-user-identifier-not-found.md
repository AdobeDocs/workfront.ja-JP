---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：SAML 2.0 エラー：ユーザー識別子が見つかりません」
description: ADFS への接続が正常に確立できません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 86%

---

# エラーメッセージ：SAML 2.0 エラー：ユーザー識別子が見つかりません

## 問題

ADFS への接続が正常に確立できません。

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>正常なテスト接続を確立しても問題が発生する場合は、属性マッピングが正しくないか、連合 ID に問題が発生する可能性があります。ご質問は、カスタマーサポートにお問い合わせください。

## 原因：

ADFS サーバーの要求が正しくありません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

ADFS サーバーで、名前 ID の要求があることを確認します。

1. Windows の場合、**[!UICONTROL 開始]**／**[!UICONTROL 管理]**／**[!UICONTROL ADFS 2.0 管理]**&#x200B;をクリックします。\
   ADFS 2.0 管理ダイアログボックスが表示されます。

1. 左側のペインで&#x200B;**[!UICONTROL 信頼関係]**／**[!UICONTROL 証明書利用者の信頼]**&#x200B;を選択します。

1. Adobe Workfront に関連する証明書利用者の信頼を右クリックし、「**[!UICONTROL 要求ルールを編集]**」を選択します。
1. 要求に&#x200B;**[!UICONTROL 名前 ID]** の&#x200B;**[!UICONTROL 送信する要求のタイプ]**&#x200B;があることを確認します。

![1.png](assets/1-350x287.png)
