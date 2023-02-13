---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'エラーメッセージ：SAML 2.0 エラー：ユーザー識別子が見つかりません'
description: ADFS への接続が正常に確立できません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 1%

---

# エラーメッセージ：SAML 2.0 エラー：ユーザー識別子が見つかりません

## 問題

ADFS への接続が正常に確立できません。

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>正常なテスト接続を確立しても問題が発生する場合は、属性マッピングが正しくないか、フェデレーション ID に問題が発生する可能性があります。 ご質問は、カスタマーサポートにお問い合わせください。

## 原因：

ADFS サーバーの要求が正しくありません

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

ADFS サーバーで、名前 ID の要求があることを確認します。

1. Windows の場合、 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0 管理]**.\
   [ADFS 2.0 管理 ] ダイアログボックスが表示されます。

1. 選択 **[!UICONTROL 信頼関係]** > **[!UICONTROL 証明書利用者信託]** をクリックします。

1. Adobe Workfrontに関連する証明書利用者の信頼を右クリックし、「 」を選択します。 **[!UICONTROL 要求ルールの編集]**.
1. 要求に **[!UICONTROL 送信する要求の種類]** / **[!UICONTROL 名前 ID]**.

![1.png](assets/1-350x287.png)
