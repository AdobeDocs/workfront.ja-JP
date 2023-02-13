---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 外部ユーザーライセンスの種類がアクセスレベルにありません
description: '[ セットアップ ] の [ アクセスレベル ] に [ 外部ユーザライセンスの種類 ] が表示されなくなりました。'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 外部ユーザーライセンスの種類がアクセスレベルにありません

## 問題

[ セットアップ ] の [ アクセスレベル ] に [ 外部ユーザライセンスの種類 ] が表示されなくなりました。

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

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL システム]** > **[!UICONTROL 環境設定]**.

1. 内 **[!UICONTROL セキュリティ]** セクションで、オプションを確認します。 **[!UICONTROL E メールアドレスを使用して、Workfrontアカウントを持たないユーザーと共同作業する]** が有効になっている。

   このオプションが有効になっていない場合、外部ユーザーはアクセスレベル設定に表示されません。
