---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: で新しいテンプレートを作成 [!DNL Adobe Workfront Fusion]
description: で新しいシナリオテンプレートを作成できます。 [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# で新しいテンプレートを作成 [!DNL Adobe Workfront Fusion]

で新しいシナリオテンプレートを作成できます。 [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>新しいテンプレートを作成する前に、 [!UICONTROL 公開テンプレート] 」タブを使用して、作成するテンプレートがまだ使用できないことを確認します。

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
  <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 新しいテンプレートを作成

シナリオの作成と同様のプロセスでテンプレートを作成できます。 また、Fusion 管理者は、既存のシナリオからテンプレートを作成することもできます。

* [テンプレートの作成](#build-a-template)
* [シナリオからのテンプレートの作成](#create-a-template-from-a-scenario)

### テンプレートの作成

1. クリック **[!UICONTROL テンプレート]** ![](assets/fusion-template-icon.png) をクリックします。
1. クリック **[!UICONTROL 新しいテンプレートを作成]** をクリックします。
1. （オプション）デフォルトの **[!UICONTROL 新しいテンプレート名]** をクリックします。
1. （オプション）テンプレートの言語を変更するには、 **[!UICONTROL テンプレートの設定]** ![](assets/fusion-scenario-settings-icon.png) 言語ドロップダウンから言語を選択します。

   >[!IMPORTANT]
   >
   >「言語」選択は、システム設定で使用できる言語に対応し、パブリックテンプレートの名前と説明のみに関係します。 テンプレートを保存すると、テンプレート言語は変更できなくなります。

1. （オプション）テンプレートの説明を入力するには、 **[!UICONTROL テンプレートの設定]** ![](assets/fusion-scenario-settings-icon.png) をクリックし、説明を入力します。
1. 標準シナリオを作成する場合と同じ方法で、アプリ、モジュールおよびツールを追加します。

   モジュールにコンテキストヘルプを追加するには、 [設定 [!UICONTROL ウィザード] 機能](#set-up-wizard-functionality) 」を参照してください。

   シナリオの作成について詳しくは、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >接続、資格情報、またはその他のプライバシーに関する機密情報を追加する必要があるモジュールがテンプレートに含まれている場合、この情報はテンプレートユーザーと共有されません。

1. （オプション）「 **[!UICONTROL 1 回実行]** をクリックして、テンプレートをテストします。
1. 次をクリック： **[!UICONTROL 保存]** アイコン ![](assets/save-icon.png).

>[!NOTE]
>
>テンプレートを保存すると、すべてのチームメンバーに対して表示されます。 チーム外でテンプレートにアクセスできるようにするには、テンプレートを公開してから共有リンクを使用するか、管理者にテンプレートの承認と公開を依頼する必要があります。

### シナリオからのテンプレートの作成

>[!NOTE]
>
>シナリオからテンプレートを作成するには、Fusion 管理者である必要があります。

1. シナリオを作成するシナリオのシナリオの詳細ページを開きます。
1. 次をクリック： **管理者** ドロップダウンを使用して、ページの右上隅に表示されます。
1. 選択 **テンプレートとして複製**.

   シナリオが新しいテンプレートページにコピーされます。
1. （オプション）デフォルトの **[!UICONTROL 新しいテンプレート名]** をクリックします。
1. （オプション）テンプレートの言語を変更するには、 **[!UICONTROL テンプレートの設定]** ![](assets/fusion-scenario-settings-icon.png) 言語ドロップダウンから言語を選択します。

   >[!IMPORTANT]
   >
   >「言語」選択は、システム設定で使用できる言語に対応し、パブリックテンプレートの名前と説明のみに関係します。 テンプレートを保存すると、テンプレート言語は変更できなくなります。

1. （オプション）テンプレートの説明を入力するには、 **[!UICONTROL テンプレートの設定]** ![](assets/fusion-scenario-settings-icon.png) をクリックし、説明を入力します。
1. 標準シナリオの編集時と同じ方法で、アプリ、モジュールおよびツールを編集します。

   モジュールにコンテキストヘルプを追加するには、 [設定 [!UICONTROL ウィザード] 機能](#set-up-wizard-functionality) 」を参照してください。

   >[!NOTE]
   >
   >接続、資格情報、またはその他のプライバシーに関する機密情報を追加する必要があるモジュールがテンプレートに含まれている場合、この情報はテンプレートユーザーと共有されません。

1. （オプション）「 **[!UICONTROL 1 回実行]** をクリックして、テンプレートをテストします。
1. 次をクリック： **[!UICONTROL 保存]** アイコン ![](assets/save-icon.png).

## 設定 [!UICONTROL ウィザード] 機能 {#set-up-wizard-functionality}

この [!DNL Workfront Fusion template] [!UICONTROL ウィザード] では、今後、テンプレートのユーザーに対し、モジュールで使用される特定のフィールドに関する手順や情報を提供できます。

1. テンプレートに追加されたモジュールをクリックして、モジュールのフィールドを確認します。
1. 追加するフィールドを見つけます。 [!UICONTROL ウィザード] 情報、および有効化 **[!UICONTROL ウィザードで使用]** そのフィールドの
1. ユーザーに表示させる情報を [!UICONTROL ヘルプ] フィールドに入力します。
1. （オプション）テンプレートの使用時にユーザーにこのテキストを表示させるには、 **[!UICONTROL デフォルト値として使用]**.
1. 情報を入力する各フィールドに対して、手順 2 ～ 4 を繰り返します。
1. クリック **[!UICONTROL OK]** 変更を保存してモジュールを閉じます。
