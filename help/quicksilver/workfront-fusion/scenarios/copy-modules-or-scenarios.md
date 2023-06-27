---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: でのモジュールまたはシナリオのコピー [!DNL Adobe Workfront Fusion]
description: でのモジュールまたはシナリオのコピー [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# でのモジュールまたはシナリオのコピー [!DNL Adobe Workfront Fusion]

では、モジュール、モジュールのグループ、またはシナリオ全体をコピーできます [!DNL Adobe Workfront Fusion]. この機能を使用すると、シナリオやシナリオの一部を再び構築しなくても再利用できます

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

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

モジュールをコピーする前に、シナリオにモジュールを追加する必要があります。

## モジュールまたはモジュールのグループのコピー

モジュールをコピーすると、コピー元のモジュールのすべてのフィールド値と設定が保持されます。

1 つ以上のモジュールを、同じシナリオの別の領域、または別のシナリオに貼り付けることができます。

モジュールを別のシナリオに貼り付ける場合は、次の点を考慮してください。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* コピーしなかった別のモジュールから情報を取り込むフィールド値は、その情報にアクセスできなくなりました。 新しいシナリオから情報を取り込むには、これらのフィールドを設定する必要があります。
* 別のチームまたは組織が所有するシナリオにモジュールを貼り付ける場合は、すべての接続を、新しいシナリオを所有するグループまたは組織が所有する接続に更新する必要があります。

### モジュールのコピー

モジュールのグループをコピーする方法は、単一のモジュールをコピーする場合と似ています。

1. コピーするモジュールを右クリックします。

   >[!NOTE]
   >
   >次のボタンを押すと、複数のモジュールを選択できます [!UICONTROL shift] をクリックし、コピーするモジュールをクリックします。 モジュールのグループをコピーすると、接続線、フィルタ、またはルーティングロジックもコピーされます。

1. 選択 **[!UICONTROL モジュールをコピー]**.
1. シナリオのコピー先となる領域にカーソルを移動します。
1. 右クリックし、「 」を選択します。 **[!UICONTROL 貼り付け]**.
1. 貼り付けたモジュールをシナリオ内の適切な場所にドラッグして、シナリオに接続します。

   キーボードショートカットを使用してコピー&amp;ペーストすることもできます。

## 複製によるシナリオのコピー

シナリオを複製すると、シナリオのコピーが作成され、編集できます。

1. シナリオの詳細ページを開きます。

   1. 次をクリック： **[!UICONTROL シナリオ]** 」タブをクリックし、詳細を表示するシナリオをクリックします。

      または

      を使用して、 [のシナリオエディター [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)、左向き矢印をクリックします。 ![](assets/exit-editing-arrow.png) ウィンドウの左上隅付近にある

1. 右クリック **[!UICONTROL オプション]** をクリックします。
1. 選択 **[!UICONTROL 複製]**.
1. （オプション）新しいシナリオの名前を入力します。
1. （オプション）有効にする **[!UICONTROL 新しいモジュールの状態を、複製されるモジュールと同じ状態に保ちます。]** コピーしたシナリオに、元のシナリオで処理された最新のレコードに関する情報も含まれるようにするため。
1. クリック **[!UICONTROL 保存]** をクリックして、シナリオを作成します。

## ブループリントを使用してシナリオをコピーする

シナリオのブループリントは、特定の時点での特定のシナリオの配置、マッピング、フィールド値を表します。 シナリオのブループリントをコンピューター上の JSON ファイルに書き出し、新しいシナリオの作成時に読み込むことができます。 シナリオのブループリントからインポートしたシナリオは編集できます。

シナリオのブループリントは、シナリオ全体を表します。 シナリオから特定のモジュールのみをコピーする場合は、 [モジュールまたはモジュールのグループのコピー](#copy-a-module-or-a-group-of-modules) 」を参照してください。

>[!NOTE]
>
>のコンテキストのブループリントに関する情報 [!DNL Adobe Workfront]を参照してください。 [ブループリントの概要](../../administration-and-setup/blueprints/blueprints-overview.md).

### シナリオのブループリントを書き出し

1. シナリオで、 **[!UICONTROL 詳細]** メニューを使用します。
1. クリック **[!UICONTROL ブループリントを書き出し]**.

   JSON ファイルが作成され、コンピューターにダウンロードされます。 このファイルは、 [!DNL Downloads] フォルダー。

### ブループリントを読み込む

>[!IMPORTANT]
>
>ブループリントを既存のシナリオに読み込むと、既存のシナリオがシナリオのブループリントに置き換えられます。 既存のシナリオにブループリントを追加することはできません。

1. 新しいシナリオの作成を開始します。
1. シナリオで、 **[!UICONTROL 詳細]** メニューを使用します。
1. クリック **[!UICONTROL ブループリントを読み込み]**.
1. 表示されるダイアログで、 **[!UICONTROL 参照]**
1. 読み込むブループリントに移動し、 **[!UICONTROL 開く]**.
1. 「**[!UICONTROL 保存]**」をクリックします。

   JSON ファイルが作成され、コンピューターにダウンロードされます。 このファイルは、 [!UICONTROL ダウンロード] フォルダー。

## テンプレートを使用してシナリオをコピーおよび再利用

テンプレートを作成して、 [!DNL Workfront Fusion] シナリオ。 テンプレートからシナリオを作成する場合、テンプレートを変更せずにシナリオを変更できます。 フィールドの値は、テンプレートに保存されません。

テンプレートの作成と使用について詳しくは、 [シナリオテンプレート](../../workfront-fusion/scenarios/templates/fusion-templates.md).
