---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion] でモジュール設定を行う'
description: 作成するモジュールごとに設定を指定する必要があります。
author: Becky
feature: Workfront Fusion
exl-id: 7e66728d-8c6f-4597-98c4-bc6d36f96911
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '334'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でモジュール設定を行う

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
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr>  
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプやアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## モジュール設定を指定

1. シナリオに新しいモジュールを追加。

   または

   シナリオエディターでモジュールのアイコンをクリックします。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)でシナリオを作成を参照してください。

1. モジュールで必要な場合は、その特定のサービスの登録済みユーザーアカウントに&#x200B;**[!UICONTROL 接続]**&#x200B;を作成します。詳しくは、[アプリまたはサービスへの  [!DNL Adobe Workfront Fusion]  の接続について](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)を参照してください。
1. 各フィールドに、適切なテキストを入力します。

   または

   フィールドの右側に&#x200B;**[!UICONTROL マップ]**&#x200B;が表示されている場合はクリックし、シナリオ内の別のモジュールから項目をマッピングします。

   太字のパラメーターは必須です。

   [!DNL Workfront Fusion] が認識できる様々な項目データタイプ（日付、数値、テキストなど）について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md) の項目データタイプを参照してください。

1. （条件付き）モジュールに、表示および使用する詳細オプションがある場合、「**[!UICONTROL 詳細設定を表示]**」を選択します。
