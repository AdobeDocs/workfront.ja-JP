---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 外部ユーザー指定ライセンスの種類がアクセスレベルにありません
description: 設定のアクセスレベルに外部ユーザー指定ライセンスの種類が表示されなくなりました。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '161'
ht-degree: 100%

---

# 外部ユーザー指定ライセンスの種類がアクセスレベルにありません

## 問題

設定のアクセスレベルに外部ユーザー指定ライセンスの種類が表示されなくなりました。

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
   <td> <p>ユーザーは [!DNL Workfront] 管理者である必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> <p><b>メモ</b>：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ソリューション

1. **[!UICONTROL 設定]**／**[!UICONTROL システム]**／**[!UICONTROL 環境設定]**&#x200B;に移動します。

1. 「**[!UICONTROL セキュリティ]**」セクションで、「**[!UICONTROL メールアドレスを使用して Workfront アカウントを持たないユーザーと共同作業]**」オプションが有効になっていることを確認します。

   このオプションが有効になっていない場合、外部ユーザーはアクセスレベル設定に表示されません。
