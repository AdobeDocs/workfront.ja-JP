---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''エラーメッセージ：SAML 2.0 エラー：プライマリStatusCode`'
description: ADFS への接続が正常に確立できません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# エラーメッセージ：SAML 2.0 エラー：プライマリStatusCode

## 問題

ADFS への接続が正常に確立できません。

![SAML_2.0_Error_Error_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>正常なテスト接続を確立しても問題が発生する場合は、属性マッピングが正しくないか、フェデレーション ID に問題が発生する可能性があります。 ご質問は、カスタマーサポートにお問い合わせください。

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

## 原因 1:Secure hash algorithm が SHA-256 に設定されています

### 解決策

1. Windows の場合、 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0 管理]**.\
   [ADFS 2.0 管理 ] ダイアログボックスが表示されます。

1. 選択 **[!UICONTROL 信頼関係]** > **[!UICONTROL 証明書利用者信託]** をクリックします。

1. 関連する証明書利用者の信頼を右クリックします。 [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL プロパティ]**.
1. をクリックします。 **[!UICONTROL 詳細]** 「 」タブで、「 **[!UICONTROL SHA-1]** から **[!UICONTROL Secure hash algorithm]** ドロップダウンメニュー。\
   ![](assets/1-350x287.png)

## 原因 2:ADFS 署名証明書の有効期限が切れようとしており、日付が重なる新しい証明書に置き換えられました

### 解決策

この [!DNL Workfront] SSO セットアップページに証明書の有効期限が表示されます。 証明書の有効期限が近づいている場合は、ADFS サーバーから新しい署名証明書を手動で取り込む必要があります。

1. Windows の場合、 **[!UICONTROL 開始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0 管理]**.\
   [ADFS 2.0 管理 ] ダイアログボックスが表示されます。

1. 選択 **[!UICONTROL 信頼関係]** > **[!UICONTROL 証明書利用者信託]** をクリックします。

1. 関連する証明書利用者の信頼を右クリックします。 [!DNL Workfront]を選択し、 **[!UICONTROL プロパティ]**.
1. をクリックします。 **[!UICONTROL 署名]** タブをクリックします。
1. 署名証明書の名前をクリックし、 **[!UICONTROL 表示]**.
1. コピー先をクリックします。 **[!UICONTROL ファイル]**...」、「 **[!UICONTROL 次へ]**.

1. 選択 **[!UICONTROL Base-64 エンコード済み x.509(CER)]**&#x200B;をクリックし、 **[!UICONTROL 次へ]**.

1. ファイル名を指定し、 **[!UICONTROL 次へ]**.
1. クリック **[!UICONTROL 完了]**.
1. In [!DNL Workfront]に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL システム]** > **[!UICONTROL シングルサインオン (SSO)]** 署名証明書を手動でアップロードします。

## 原因 3:証明書失効確認が失敗しています

これに対する解決策は、のバージョンによって異なります。 [!DNL Microsoft] 使用している ADFS。 問い合わせ [!DNL Microsoft]ご使用のバージョンに適したコマンドを取得するためのののドキュメント。
