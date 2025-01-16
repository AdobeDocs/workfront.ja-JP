---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion] でモジュール設定を行う'
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 75%

---

# [!DNL Adobe Workfront Fusion] でモジュール設定を行う

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ モジュールの設定 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/configure-a-modules-settings.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

作成するモジュールごとに設定を指定する必要があります。

例えば、[[!DNL Dropbox] モジュール](../../workfront-fusion/apps-and-their-modules/dropbox-modules.md)では、ファイルをアップロードするターゲットフォルダーを指定する必要があります。[[!UICONTROL メール]モジュール](../../workfront-fusion/apps-and-their-modules/email-modules.md)では、メールの送信先のメールアドレスを入力する必要があります。

>[!NOTE]
>
>モジュール設定の他に、シナリオの設定を調整することもできます。シナリオの名前を変更したり、スケジュールを変更したり、他のアクションの中で追加の設定を指定したりできます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr>  
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## モジュール設定を指定

1. シナリオに新しいモジュールを追加。

   または

   シナリオエディターでモジュールのアイコンをクリックします。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)でシナリオを作成を参照してください。

1. モジュールで必要な場合は、**[!UICONTROL 接続の概要]** に記載されているように、指定したサービスに登録済みのユーザーアカウントに [ 接続 ](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md) を作成します。
1. 各フィールドに、適切なテキストを入力します。

   または

   フィールドの右側に&#x200B;**[!UICONTROL マップ]**&#x200B;が表示されている場合はクリックし、シナリオ内の別のモジュールから項目をマッピングします。

   太字のパラメーターは必須です。

   [!DNL Workfront Fusion] が認識できる様々な項目データタイプ（日付、数値、テキストなど）について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md) の項目データタイプを参照してください。

1. （条件付き）モジュールに、表示および使用する詳細オプションがある場合、「**[!UICONTROL 詳細設定を表示]**」を選択します。
