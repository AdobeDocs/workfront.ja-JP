---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：XML デジタル署名を検証できませんでした」
description: ADFS への接続が正常に確立できません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 94%

---

# エラーメッセージ：XML デジタル署名を検証できませんでした

## 問題

ADFS への接続が正常に確立できません。

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>正常なテスト接続を確立しても問題が発生する場合は、属性マッピングが正しくないか、連合 ID に問題が発生する可能性があります。ご質問は、カスタマーサポートにお問い合わせください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td>[!DNL Workfront] 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

この表にある情報についての詳細は、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 原因 1：証明書が正しくない

### ソリューション

ADFS サーバーから手動で署名証明書を取得します。

1. [!DNL Windows] で、**[!UICONTROL 開始]**／**[!UICONTROL 管理]**／**[!UICONTROL ADFS 2.0 管理]**&#x200B;をクリックします。\
   ADFS 2.0 管理ダイアログボックスが表示されます。

1. 左側のパネルで&#x200B;**[!UICONTROL 信頼関係]**／**[!UICONTROL 証明書利用者の信頼]**&#x200B;を選択します。

1. **[!UICONTROL 証明書利用者の信頼]**&#x200B;を右クリックし、続いて&#x200B;**[!UICONTROL プロパティ]**&#x200B;を選択します。

1. 「**[!UICONTROL 署名]**」タブをクリックします。
1. 署名証明書の名前をクリックし、「**[!UICONTROL 表示]**」をクリックします。
1. 「**[!UICONTROL ファイル]**&#x200B;にコピー」をクリックし、「**[!UICONTROL 次へ]**」を選択します。

1. 「**[!UICONTROL Base-64 エンコード x.509 (CER)]**」をクリックし、「**[!UICONTROL 次へ]**」をクリックします。

1. ファイル名を指定し、「**[!UICONTROL 次へ]**」をクリックします。
1. 「**[!UICONTROL 完了]**」をクリックします。
1. [!DNL Adobe Workfront] で、**[!UICONTROL 設定]**／**[!UICONTROL システム]**／**[!UICONTROL シングルサインオン(SSO)]** をクリックし、署名証明書を手動でアップロードします。

## 原因 2：[!DNL Workfront] が RSA 署名を期待している場合に、証明書が DSA を使用して署名されている

### ソリューション

証明書を再作成し、RSA 署名を DSA の代わりに使用します。

## 原因 3：XML データが正しくない

### ソリューション

ADFS 管理システムから XML メタデータを再書き出しおよび再読み込みします。

## 原因 4：SAML 側でのエラーが原因で、リクエストを実行できなかった

### ソリューション

SAML プロバイダーに問い合わせてください。
