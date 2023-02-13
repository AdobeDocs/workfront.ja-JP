---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Microsoft Exchange での POP の設定
description: の POP 電子メールアカウント [!DNL Microsoft Exchange] は無効です。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# POP in の設定 [!DNL Microsoft Exchange]

## 問題

の POP 電子メールアカウント [!DNL Microsoft Exchange] は無効です。

## 解決策

時間をかけて問題のトラブルシューティングを行う前に、ユーザーの POP アカウントが正しく設定されていることを確認してください。 POP アカウントが正しく設定されていることを確認した後も引き続き問題が発生する場合は、 [!DNL Microsoft] サポートまたはパートナーの 1 人が追加のサポートを受けられます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## POP in の設定 [!DNL Microsoft Exchange]

>[!NOTE]
>
>次の手順を、POP in の設定に関する一般的なガイドとして使用できます [!DNL Microsoft Exchange] 実稼動用 [!DNL Workfront] システム。 手順は、Exchange のバージョンやMicrosoftがおこなったコード変更によって大きく異なる場合があります。

1. Exchange 2010 サーバーで POP3 サービスを起動し、有効にします。

   >[!NOTE]
   >
   >デフォルトでは、POP3 サービスは開始されません。

   1. 開始 [!DNL Microsoft]のサーバーマネージャー。
   1. 移動： **[!UICONTROL サーバーマネージャ]** > **[!UICONTROL 設定]** >**[!UICONTROL 高度なセキュリティを備えた Windows ファイアウォール]** > **[!UICONTROL サービス]**.

   1. 右クリック **[!DNL Microsoft Exchange]POP3**&#x200B;を選択し、「 **[!UICONTROL プロパティ]**.

   1. （条件付き）POP サービスが自動的に開始するように、 **[!UICONTROL 一般]** タブ、 **[!UICONTROL 起動]** 入力 [!UICONTROL 自動].

1. サーバーに POP3 を設定します。

   1. を開始します。 [!DNL Microsoft Exchange] 管理コンソール。
   1. 移動： [!DNL Microsoft] **[!UICONTROL Exchange オンプレミス]** > **[!UICONTROL サーバー設定]** > **[!UICONTROL クライアントアクセス]**.

   1. 選択 **[!UICONTROL POP3]**.

      POP3 はリストの [!UICONTROL POP3] および [!UICONTROL IMAP4] タブ

   1. 右側の下 **[!UICONTROL アクション]**&#x200B;を選択します。 **[!UICONTROL POP3]**&#x200B;を選択して、 **[!UICONTROL プロパティ]**.

   1. クリック **[!UICONTROL POP3 プロパティ]**&#x200B;をクリックし、 **[!UICONTROL 連結]** タブをクリックします。

      POP3 サーバー用に設定された、使用可能な IP アドレスとポート番号がすべて表示されます。 上部のボックスには「暗号化されていません」と表示され、下部のボックスには SSL/TLS 接続用の IP とポートが表示されます。

   1. クリック **[!UICONTROL POP3 プロパティ]**&#x200B;をクリックし、 **[!UICONTROL 認証]** タブをクリックします。

   1. **[!UICONTROL セキュアを選択]** ログインします。

      クライアントがサーバーに対して認証をおこなうには、TLS 接続が必要です。

1. ユーザーの POP への接続を有効にするか、許可します。

   1. を開始します。 [!DNL Microsoft Exchange] 管理コンソール。
   1. 移動： [!DNL Microsoft] **[!UICONTROL Exchange オンプレミス]** > **[!UICONTROL 受信者の設定]** > **[!UICONTROL Mailbox]**.

      メールボックスまたはユーザーのリストが表示されます。

   1. 内で使用されている E メールをハイライトします [!DNL Workfront].
   1. 右側の下 **[!UICONTROL アクション]**&#x200B;を選択します。 **[!UICONTROL プロパティ]**&#x200B;をクリックし、 **[!UICONTROL メールボックスの機能]** タブをクリックします。

   1. （条件付き）POP3 が無効な場合、 **[!UICONTROL POP3]**&#x200B;を選択し、「 **[!UICONTROL 有効にする]**.

      メールボックスまたはユーザーのリストが表示されます。

1. 受信コネクタを設定します。

   1. 開始 [!DNL Microsoft Exchange] 管理コンソール。
   1. 移動： [!DNL Microsoft] **[!UICONTROL Exchange オンプレミス]** > **[!UICONTROL サーバー設定]** > **[!UICONTROL ハブトランスポート]**.

      受信コネクタのリストが表示されます。

   1. 受信コネクタを確認します。 *クライアント* *EX01* が有効になっている。

      ここで、 *クライアント* *EX01* は、Exchange サーバーの名前です。

   1. 選択 *クライアント EX01*&#x200B;右の下に **[!UICONTROL アクション]**&#x200B;を選択します。 **[!UICONTROL プロパティ]**.

   1. を開きます。 **[!UICONTROL 認証]** 「 」タブで、 **[!UICONTROL トランスポート層セキュリティ (TLS)]** がオンになっている。

      >[!NOTE]
      >
      >基本認証を使用するには、TLS と統合 Windows 認証を開始する必要がある場合があります。
