---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: でのモジュールの設定 [!DNL Adobe Workfront Fusion]
description: 作成するモジュールごとに設定を指定する必要があります。
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# でのモジュールの設定 [!DNL Adobe Workfront Fusion]

作成するモジュールごとに設定を指定する必要があります。

例えば、 [[!DNL Dropbox] モジュール](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md) モジュールでは、ファイルをアップロードするターゲットフォルダーを指定する必要があります。 の [[!UICONTROL 電子メール] モジュール](../../workfront-fusion/apps-and-their-modules/email-modules.md) モジュールを使用する場合は、電子メールの送信先の電子メールアドレスを入力する必要があります。

>[!NOTE]
>
>モジュール設定の他に、シナリオの設定を調整することもできます。 シナリオの名前を変更したり、スケジュールを変更したり、他のアクションの中で追加の設定を指定したりできます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr>  
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## モジュールの設定

1. シナリオに新しいモジュールを追加します。

   または

   シナリオエディターでモジュールのアイコンをクリックします。詳しくは、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. モジュールで必要な場合は、 **[!UICONTROL 接続]** を、指定したサービスの登録ユーザーアカウントに追加します。詳しくは、 [接続について [!DNL Adobe Workfront Fusion] アプリまたはサービスに](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
1. 各フィールドに、適切なテキストを入力します。

   または

   クリック **[!UICONTROL マップ]** 「 」フィールドの右側に表示される場合は、シナリオの別のモジュールの項目をマッピングします。

   太字のパラメーターは必須です。

   様々な項目データタイプの情報 [!DNL Workfront Fusion] を認識できる（日付、数値、テキストなど）ので、 [の項目データタイプ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

1. （条件付き）モジュールに、表示および使用する高度なオプションがある場合、 **[!UICONTROL 詳細設定を表示]**.
