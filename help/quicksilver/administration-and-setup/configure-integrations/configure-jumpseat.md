---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat 統合の設定
description: ' [!DNL JumpSeat] を [!DNL Workfront] と統合して、カスタムの製品内ガイダンスを作成できます。'
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 01b7eb79028eb3fe47f988a31cb62ace31bba3f1
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 79%

---

# JumpSeat 統合の設定

[!DNL JumpSeat] を [!DNL Workfront] と統合して、カスタムの製品内ガイダンスをを作成できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>アクティブな [!DNL JumpSeat] プランが必要です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p> [!DNL Workfront] の管理者である必要があります。[!DNL Workfront] 管理者については、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

+++

## 前提条件

開始する前に、

* [!DNL JumpSeat] に [!DNL Workfront] をアプリケーションとして追加し、アクティブ化します。詳しくは、[アプリケーションを追加または削除する方法](https://support.jumpseat.io/article/how-to-add-an-application/)を参照してください。

>[!IMPORTANT]
>
>Adobe統合エクスペリエンスを使用している場合は、次のアプリケーション URL を使用する必要があります。`.workfront.adobe.com`



## [!DNL JumpSeat] 統合の設定

プレビュー環境と実稼動環境の両方で、[!DNL JumpSeat] 統合を設定することをお勧めします。

>[!TIP]
>
>[!DNL JumpSeat] に 2 つの別個の [!DNL Workfront] アプリケーション（プレビュー用に 1 つ、実稼動用に 1 つ）を追加してアクティブ化する必要があります。詳しくは、[アプリケーションを追加または削除する方法](https://support.jumpseat.io/article/how-to-add-an-application/)を参照してください。

[!DNL JumpSeat] 統合を設定するには、次の手順に従います。

{{step-1-to-setup}}

1. 左パネルで、**[!UICONTROL システム]**／**[!UICONTROL [!DNL JumpSeat]統合]**&#x200B;をクリックします。
1. **[!UICONTROL [!DNL JumpSeat]URL]** を入力します。この URL は、[!DNL JumpSeat] の拡張機能アイコンにあります。

>[!BEGINSHADEBOX]

**例：**

https://{mycompanyname}.jumpseat.io

&#x200B;>>

>[!ENDSHADEBOX]

1. **[!UICONTROL [!DNL JumpSeat]統合トークン]**&#x200B;を入力します。これは、[!DNL JumpSeat] の&#x200B;**[!UICONTROL 設定]**&#x200B;ページで確認できます。

   **例：**$2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 「**[!UICONTROL 構成をテスト]**」をクリックします。
1. 統合を&#x200B;**[!UICONTROL アクティブ]**&#x200B;にするか、**[!UICONTROL 非アクティブ]**&#x200B;にするかを選択します。

   >[!IMPORTANT]
   >
   >統合をアクティブにするには、手順 5 で実行した設定テストに合格する必要があります。

   ![JumpSeat 統合ページ](assets/jumpseat-integration-page.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

>[!TIP]
>
>[!DNL JumpSeat] 統合の設定について詳しくは、[JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/) の [!DNL JumpSeat] ドキュメントを参照してください。
