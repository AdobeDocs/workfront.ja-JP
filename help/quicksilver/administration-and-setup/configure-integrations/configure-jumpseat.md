---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat 統合の設定
description: 統合可能な [!DNL JumpSeat] と [!DNL Workfront] を使用して、製品内のカスタムガイダンスを作成します。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# JumpSeat 統合の設定

統合可能な [!DNL JumpSeat] と [!DNL Workfront] を使用して、製品内のカスタムガイダンスを作成します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>製品</strong></td> 
   <td>アクティブな [!DNL JumpSeat] プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p> 次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

始める前に、

* 追加とアクティブ化 [!DNL Workfront] の申し込みとして [!DNL JumpSeat]. 詳しくは、 [アプリケーションを追加または削除する方法](https://support.jumpseat.io/article/how-to-add-an-application/).

## の設定 [!DNL JumpSeat] 統合

アドビでは、 [!DNL JumpSeat] の統合機能を利用できます。

>[!TIP]
>
>2 つのを別々に追加してアクティブ化する必要があります [!DNL Workfront] のアプリケーション [!DNL JumpSeat] — プレビュー用に 1 つ、実稼働用に 1 つ。 詳しくは、 [アプリケーションを追加または削除する方法](https://support.jumpseat.io/article/how-to-add-an-application/) を参照してください。

次の手順で [!DNL JumpSeat] 統合：

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]**.
1. 左側のパネルで、 **[!UICONTROL システム]** > **[!UICONTROL [!DNL JumpSeat]統合]**.
1. を入力します。 **[!UICONTROL [!DNL JumpSeat]URL]**.

   **例：** [!DNL https]://{mycompanyname}.jumpseat.io

1. 次を入力します。 **[!UICONTROL [!DNL JumpSeat]統合トークン]**. これは、 **[!UICONTROL 設定]** ページ内 [!DNL JumpSeat].

   **例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. クリック **[!UICONTROL 設定をテスト]**.
1. 統合をにする場合に選択します **[!UICONTROL アクティブ]** または **[!UICONTROL 非アクティブ]**.

   >[!IMPORTANT]
   >
   >統合をアクティブ化するには、手順 5 で実行した設定テストが合格する必要があります。

   ![JumpSeat 統合ページ](assets/jumpseat-integration-page.png)

1. 「**[!UICONTROL 保存]**」をクリックします。
