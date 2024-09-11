---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Microsoft Exchange での POP 設定
description: ' [!DNL Microsoft Exchange]  の POP メールアカウントが無効になっています。'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 97%

---

# [!DNL Microsoft Exchange] での POP 設定

## 問題

[!DNL Microsoft Exchange] の POP メールアカウントが無効になっています。

## ソリューション

問題のトラブルシューティングに時間を費やす前に、ユーザーの POP アカウントが正しく設定されていることを確認してください。POP アカウントが正しく設定されていることを確認した後も問題が解決しない場合は、[!DNL Microsoft] サポートまたはそのパートナーにお問い合わせください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## [!DNL Microsoft Exchange] での POP 設定

>[!NOTE]
>
>次の手順を、実稼動 [!DNL Workfront] システム向けに [!DNL Microsoft Exchange] での POP 設定に関する一般的なガイドとして使用できます。この手順は、Exchange のバージョンや Microsoft によるコード変更によって大きく異なる場合があります。

1. Exchange 2010 サーバーで POP3 サービスを起動し、有効にします。

   >[!NOTE]
   >
   >デフォルトでは、POP3 サービスは開始されていません。

   1. [!DNL Microsoft] のサーバーマネージャーを起動します。
   1. **[!UICONTROL サーバーマネージャー]**／**[!UICONTROL 設定]**／**[!UICONTROL 高度なセキュリティを備えた Windows ファイアウォール]**／**[!UICONTROL サービス]**&#x200B;の順に移動します。

   1. **[!DNL Microsoft Exchange]POP3**&#x200B;を右クリックし、「**[!UICONTROL プロパティ]**」をクリックします。

   1. （条件付き）POP サービスが自動的に開始されるようにするには、「**[!UICONTROL 一般]**」タブで、「**[!UICONTROL 起動]**」タイプを「[!UICONTROL 自動]」に設定します。

1. サーバーに POP3 を設定します。

   1. [!DNL Microsoft Exchange] 管理コンソールを起動します。
   1. [!DNL Microsoft] **[!UICONTROL Exchange オンプレミス]**／**[!UICONTROL サーバー設定]**／**[!UICONTROL クライアントアクセス]**&#x200B;の順に移動します。

   1. 「**[!UICONTROL POP3]**」を選択します。

      POP3 は「[!UICONTROL POP3]」タブと「[!UICONTROL IMAP4]」タブの下のリストにあります。

   1. 右側の&#x200B;**[!UICONTROL アクション]**&#x200B;で、「**[!UICONTROL POP3]**」を選択し、「**[!UICONTROL プロパティ]**」を選択します。

   1. 「**[!UICONTROL POP3 プロパティ]**」をクリックし、「**[!UICONTROL 連結]**」タブを開きます。

      POP3 サーバー用に設定された、すべての使用可能な IP アドレスとポート番号が表示されます。上部のボックスには暗号化されていないことが表示され、下部のボックスには SSL/TLS 接続用の IP とポートが表示されます。

   1. 「**[!UICONTROL POP3 プロパティ]**」をクリックし、「**[!UICONTROL 認証]**」タブを開きます。

   1. **[!UICONTROL 安全な]**&#x200B;ログインを選択します。

      クライアントがサーバーに対して認証を行うには、TLS 接続が必要です。

1. ユーザーが POP に接続できるようにするか、許可します。

   1. [!DNL Microsoft Exchange] 管理コンソールを起動します。
   1. [!DNL Microsoft] **[!UICONTROL Exchange オンプレミス]**／**[!UICONTROL 受信者設定]**／**[!UICONTROL メールボックス]**&#x200B;の順に移動します。

      メールボックスまたはユーザーのリストが表示されます。

   1. [!DNL Workfront] 内で使用されているメールをハイライト表示します。
   1. 右側の&#x200B;**[!UICONTROL アクション]**&#x200B;で、「**[!UICONTROL プロパティ]**」を選択し、「**[!UICONTROL メールボックスの機能]**」タブを開きます。

   1. （条件付き）POP3 が無効な場合、「**[!UICONTROL POP3]**」、「**[!UICONTROL 有効にする]**」の順にクリックします。

      メールボックスまたはユーザーのリストが表示されます。

1. 受信コネクタを設定します。

   1. [!DNL Microsoft Exchange] 管理コンソールを起動します。
   1. [!DNL Microsoft] **[!UICONTROL Exchange オンプレミス]**／**[!UICONTROL サーバー設定]**／**[!UICONTROL ハブトランスポート]**&#x200B;の順に移動します。

      受信コネクタのリストが表示されます。

   1. 受信コネクタ&#x200B;*クライアント* *EX01* が有効になっていることを確認します。

      *クライアント* *EX01* は、Exchange サーバーの名前です。

   1. *クライアント EX01* を選択し、右側の&#x200B;**[!UICONTROL アクション]**&#x200B;で、「**[!UICONTROL プロパティ]**」を選択します。

   1. 「**[!UICONTROL 認証]**」タブを開き、**[!UICONTROL トランスポート層セキュリティ（TLS）]**&#x200B;がオンになっていることを確認します。

      >[!NOTE]
      >
      >基本認証を行うには、TLS と統合 Windows 認証を開始する必要がある場合があります。
