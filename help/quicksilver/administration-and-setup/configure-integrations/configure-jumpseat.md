---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat 統合の設定
description: ' [!DNL JumpSeat] を [!DNL Workfront] と統合して、カスタムの製品内ガイダンスを作成できます。'
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Courtney, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/e2uZM6ICiPOrupfHh0rQHmh--rDWxjwpend11THYdh4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 272
ht-degree: 82%

---

# JumpSeat 統合の設定

[!DNL JumpSeat] を [!DNL Workfront] と統合して、カスタムの製品内ガイダンスをを作成できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table>
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
    <p>ワークフロー Ultimate</p>
   <td> <p>PrimeまたはUltimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront ライセンス
   </td>
   <td>標準
   <p>計画</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>製品
   </td>
   <td>アクティブな [!DNL JumpSeat] プランが必要です。
   </td>
  </tr>
   <tr>
   <td>アクセスレベル設定
   </td>
   <td>[!DNL Workfront] 管理者である必要があります。
   </td>
  </tr>
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

開始する前に、

* [!DNL JumpSeat] に [!DNL Workfront] をアプリケーションとして追加し、アクティブ化します。 詳しくは、[アプリケーションを追加または削除する方法](https://support.jumpseat.io/article/how-to-add-an-application/)を参照してください。

>[!IMPORTANT]
>
>次のアプリケーション URLを使用する必要があります：`.workfront.adobe.com`



## [!DNL JumpSeat] 統合の設定

プレビュー環境と本番環境の両方で、[!DNL JumpSeat] 統合を設定することをお勧めします。

>[!TIP]
>
>[!DNL JumpSeat] に 2 つの別個の [!DNL Workfront] アプリケーション（プレビュー用に 1 つ、実稼動用に 1 つ）を追加してアクティブ化する必要があります。 詳しくは、[アプリケーションを追加または削除する方法](https://support.jumpseat.io/article/how-to-add-an-application/)を参照してください。

[!DNL JumpSeat] 統合を設定するには、次の手順に従います。

{{step-1-to-setup}}

1. 左パネルで、**[!UICONTROL システム]**／**[!UICONTROL [!DNL JumpSeat]統合]**&#x200B;をクリックします。
1. **[!UICONTROL [!DNL JumpSeat]URL]**&#x200B;を入力します。これは、[!DNL JumpSeat]の拡張機能アイコンにあります。

>[!BEGINSHADEBOX]

**例：**

https://{mycompanyname}.jumpseat.io

>>

>[!ENDSHADEBOX]

1. **[!UICONTROL [!DNL JumpSeat]統合トークン]**&#x200B;を入力します。 これは、[!DNL JumpSeat] の&#x200B;**[!UICONTROL 設定]**&#x200B;ページで確認できます。

   **例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 「**[!UICONTROL 構成をテスト]**」をクリックします。
1. 統合を&#x200B;**[!UICONTROL アクティブ]**&#x200B;にするか、**[!UICONTROL 非アクティブ]**&#x200B;にするかを選択します。

   >[!IMPORTANT]
   >
   >統合をアクティブにするには、手順 5 で実行した設定テストに合格する必要があります。

   ![JumpSeat 統合ページ](assets/jumpseat-integration-page.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

>[!TIP]
>
>[!DNL JumpSeat]統合の設定について詳しくは、[JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/)の[!DNL JumpSeat] ドキュメントを参照してください。
