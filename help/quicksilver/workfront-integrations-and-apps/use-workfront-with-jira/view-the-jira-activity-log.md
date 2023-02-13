---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira アクティビティログの表示
description: As a [!DNL Jira] 管理者は、同期中またはチケット間の作成中に発生した例外およびエラーを表示できます [!DNL Adobe Workfront] および [!DNL Jira] 」と入力します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 次を表示： [!UICONTROL [!DNL Jira] アクティビティログ]

As a [!DNL Jira] 管理者は、同期中またはチケット間の作成中に発生した例外およびエラーを表示できます [!DNL Adobe Workfront] および [!DNL Jira] 内 [!UICONTROL アクティビティログ].

アクティビティログには、最大 500 個の項目が表示され、最新の項目から始まります。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 計画</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：で別々のシステム管理者アカウントを作成することをお勧めします。 [!DNL Jira] および [!DNL Workfront] ユーザーに付随する可能性のある既存の統合を使用するのではなく、この統合専用にする場合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

次の間で項目をリンクする前に [!DNL Workfront] および [!DNL Jira]を

* インストール [!DNL Workfront for Jira]

   インストールの手順 [!DNL Workfront for Jira]を参照してください。 [インストール [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 次にアクセス： [!UICONTROL [!DNL Jira] アクティビティログ]:

1. システム管理者として Jira にログインします。
1. クリック **[!UICONTROL 設定]** メイン [!DNL Jira] メニュー
1. クリック **[!UICONTROL アドオン]**&#x200B;を、 **[!UICONTROL アドオンの管理]**.

1. を展開します。 **[!DNL Workfront]** アドオン。
1. クリック **[!UICONTROL 設定]**.
1. にログインします。 [!DNL Workfront] をシステム管理者として設定します。
1. を選択します。 **[!UICONTROL アクティビティログ]** タブをクリックします。

   アイテムの作成中、または 2 つのアプリケーション間のフィールドの同期中に発生した例外およびエラーに関する情報を表示します。

   ログには、次のフィールドが含まれます。

   * 発生日
   * Jira のユーザーの名前
   * Jira 発行番号
   * 発生したエラーの簡単な説明。
