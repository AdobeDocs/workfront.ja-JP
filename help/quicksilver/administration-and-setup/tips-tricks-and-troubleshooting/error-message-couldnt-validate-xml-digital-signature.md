---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：XML デジタル署名を検証できませんでした」
description: ADFS への接続が正常に確立できません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '304'
ht-degree: 100%

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

1. 「**[!UICONTROL Base-64 エンコード x.509（CER）]**」、「**[!UICONTROL 次へ]**」の順にクリックします。

1. ファイル名を指定し、「**[!UICONTROL 次へ]**」をクリックします。
1. 「**[!UICONTROL 終了]**」をクリックします。
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
