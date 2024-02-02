---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：SAML 2.0 エラー：プライマリ StatusCode」
description: ADFS への接続が正常に確立できません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '370'
ht-degree: 100%

---

# エラーメッセージ：SAML 2.0 エラー：プライマリ StatusCode

## 問題

ADFS への接続が正常に確立できません。

![SAML_2.0_Error_Error_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>正常なテスト接続を確立しても問題が発生する場合は、属性マッピングが正しくないか、連合 ID に問題が発生する可能性があります。ご質問は、カスタマーサポートにお問い合わせください。

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
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 原因 1：セキュアハッシュアルゴリズムが SHA-256 に設定されている

### ソリューション

1. Windows の場合、**[!UICONTROL 開始]**／**[!UICONTROL 管理]**／**[!UICONTROL ADFS 2.0 管理]**&#x200B;をクリックします。\
   ADFS 2.0 管理ダイアログボックスが表示されます。

1. 左側のペインで&#x200B;**[!UICONTROL 信頼関係]**／**[!UICONTROL 証明書利用者の信頼]**&#x200B;を選択します。

1. [!DNL Adobe Workfront] に関連する証明書利用者の信頼を右クリックし、「**[!UICONTROL プロパティ]**」を選択します。
1. 「**[!UICONTROL 詳細]**」タブをクリックし、**[!UICONTROL セキュアハッシュアルゴリズム]**&#x200B;ドロップダウンメニューから「**[!UICONTROL SHA-1]**」を選択します。\
   ![](assets/1-350x287.png)

## 原因 2：ADFS 署名証明書の有効期限が近づいており、日付が重複する新しい証明書に置き換えられた

### ソリューション

[!DNL Workfront] SSO 設定ページに証明書の有効期限が表示されます。証明書の有効期限が近づいている場合は、ADFS サーバーから新しい署名証明書を手動で取り込む必要があります。

1. Windows の場合、**[!UICONTROL 開始]**／**[!UICONTROL 管理]**／**[!UICONTROL ADFS 2.0 管理]**&#x200B;をクリックします。\
   ADFS 2.0 管理ダイアログボックスが表示されます。

1. 左側のペインで&#x200B;**[!UICONTROL 信頼関係]**／**[!UICONTROL 証明書利用者の信頼]**&#x200B;を選択します。

1. [!DNL Workfront] に関連する証明書利用者の信頼を右クリックし、「**[!UICONTROL プロパティ]**」を選択します。
1. 「**[!UICONTROL 署名]**」タブをクリックします。
1. 署名証明書の名前をクリックし、「**[!UICONTROL 表示]**」をクリックします。
1. 「**[!UICONTROL ファイル]**&#x200B;にコピー」をクリックし、「**[!UICONTROL 次へ]**」を選択します。

1. 「**[!UICONTROL Base-64 エンコード x.509 (CER)]**」をクリックし、「**[!UICONTROL 次へ]**」をクリックします。

1. ファイル名を指定し、「**[!UICONTROL 次へ]**」をクリックします。
1. 「**[!UICONTROL 完了]**」をクリックします。
1. [!DNL Workfront] で、**[!UICONTROL 設定]**／**[!UICONTROL システム]**／**[!UICONTROL シングルサインオン (SSO)]** をクリックし、署名証明書を手動でアップロードします。

## 原因 3：証明書失効確認が失敗している

これに対する解決策は、使用している [!DNL Microsoft] ADFS のバージョンによって異なります。[!DNL Microsoft] のドキュメントを参照して、使用しているバージョンに適したコマンドを取得してください。
