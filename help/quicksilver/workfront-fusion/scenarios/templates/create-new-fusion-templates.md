---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] での新規テンプレートの作成'
description: ' [!DNL Adobe] Workfront Fusion で新しいシナリオテンプレートを作成できます。'
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 92%

---

# [!DNL Adobe Workfront Fusion] での新規テンプレートの作成

[!DNL Adobe] Workfront Fusion で新しいシナリオテンプレートを作成できます。

>[!TIP]
>
>新規テンプレートを作成する前に、「[!UICONTROL パブリックテンプレート]」タブをチェックして、作成するテンプレートがまだないことを確認します。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 新規テンプレートの作成

シナリオの作成と同様のプロセスでテンプレートを作成できます。Fusion 管理者は、既存のシナリオからテンプレートを作成することもできます。

* [テンプレートの作成](#build-a-template)
* [シナリオからのテンプレートの作成](#create-a-template-from-a-scenario)

### テンプレートの作成

1. 左側のナビゲーションパネルで、**[!UICONTROL テンプレート]**&#x200B;アイコン ![](assets/fusion-template-icon.png) をクリックします。
1. 右上隅にある「**[!UICONTROL テンプレートの新規作成]**」をクリックします。
1. （オプション）左上隅にあるデフォルトの&#x200B;**[!UICONTROL 新規テンプレート名]**&#x200B;を置き換えることで、テンプレートの名前を変更します。
1. （オプション）テンプレートの言語を変更するには、**[!UICONTROL テンプレートを設定]** ![](assets/fusion-scenario-settings-icon.png) をクリックし、言語ドロップダウンから言語を選択します。

   >[!IMPORTANT]
   >
   >言語の選択は、システム設定で使用できる言語に対応し、パブリックテンプレートの名前と説明にのみ関係します。テンプレートを保存した後は、テンプレート言語を変更することはできません。

1. （オプション）テンプレートの説明を入力するには、**[!UICONTROL テンプレートの設定]**&#x200B;アイコン ![](assets/fusion-scenario-settings-icon.png) をクリックし、説明を入力します。
1. 標準シナリオを作成する場合と同じ方法で、アプリ、モジュールおよびツールを追加します。

   モジュールにコンテキストヘルプを追加するには、この記事にある[設定[!UICONTROL ウィザード]の機能](#set-up-wizard-functionality)を参照してください。

   シナリオの作成について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md)でのシナリオの作成を参照してください

   >[!NOTE]
   >
   >接続、資格情報またはプライバシーの影響を受けるその他の情報を追加する必要があるモジュールがテンプレートに含まれている場合、この情報はテンプレートユーザーと共有されません。

1. （オプション）「**[!UICONTROL 1 回実行]**」をクリックして、テンプレートをテストします。
1. **[!UICONTROL 保存]**&#x200B;アイコン ![](assets/save-icon.png) をクリックします。

>[!NOTE]
>
>テンプレートを保存すると、すべてのチームメンバーに対して表示されるようになります。テンプレートをチーム外でアクセスできるようにするには、リクエストを送信して承認および公開する必要があります。 リクエストはAdobe Workfrontに対して承認が求められ、承認されると、チーム外の他のユーザーがテンプレートにアクセスできるようになります。
>
>テンプレートの公開について詳しくは、 [公開して共有 [!DNL Adobe Workfront Fusion] テンプレート](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### シナリオからのテンプレートの作成

>[!NOTE]
>
>シナリオからテンプレートを作成するには、Fusion 管理者である必要があります。

1. シナリオの作成元となるシナリオのシナリオ詳細ページを開きます。
1. ページの右上隅付近にある&#x200B;**管理**&#x200B;ドロップダウンをクリックします。
1. 「**テンプレートとして複製**」を選択します。

   シナリオが新規テンプレートページにコピーされます。
1. （オプション）左上隅にあるデフォルトの&#x200B;**[!UICONTROL 新規テンプレート名]**&#x200B;を置き換えることで、テンプレートの名前を変更します。
1. （オプション）テンプレートの言語を変更するには、**[!UICONTROL テンプレートを設定]** ![](assets/fusion-scenario-settings-icon.png) をクリックし、言語ドロップダウンから言語を選択します。

   >[!IMPORTANT]
   >
   >言語の選択は、システム設定で使用できる言語に対応し、パブリックテンプレートの名前と説明にのみ関係します。テンプレートを保存した後は、テンプレート言語を変更することはできません。

1. （オプション）テンプレートの説明を入力するには、**[!UICONTROL テンプレートを設定]** ![](assets/fusion-scenario-settings-icon.png) をクリックし、説明を入力します。
1. 標準シナリオの編集時と同じ方法で、アプリ、モジュールおよびツールを編集します。

   モジュールにコンテキストヘルプを追加するには、この記事の[設定[!UICONTROL ウィザード]機能](#set-up-wizard-functionality)を参照してください。

   >[!NOTE]
   >
   >接続、資格情報またはプライバシーの影響を受けるその他の情報を追加する必要があるモジュールがテンプレートに含まれている場合、この情報はテンプレートユーザーと共有されません。

1. （オプション）「**[!UICONTROL 1 回実行]**」をクリックして、テンプレートをテストします。
1. **[!UICONTROL 保存]**&#x200B;アイコン ![](assets/save-icon.png) をクリックします。

## [!UICONTROL  ウィザード]機能の設定 {#set-up-wizard-functionality}

[!DNL Workfront Fusion template] [!UICONTROL ウィザード]では、今後テンプレートを使用するユーザーに対して、モジュールで使用される特定のフィールドに関する手順や情報を提供します。

1. テンプレートに追加されたモジュールをクリックして、モジュールのフィールドを表示します。
1. [!UICONTROL ウィザード]情報を追加するフィールドを見つけ、そのフィールドの「**[!UICONTROL ウィザードで使用]**」を有効にします。
1. ユーザーに対して表示する情報を、「[!UICONTROL ヘルプ]」フィールドに入力します。
1. （オプション）テンプレートの使用時にユーザーに対してこのテキストを表示するには、「**[!UICONTROL デフォルト値として使用]**」を有効にします。
1. 情報を入力する各フィールドに対して、手順 2～4 を繰り返します。
1. 「**[!UICONTROL OK]**」をクリックして、変更を保存してモジュールを閉じます。
