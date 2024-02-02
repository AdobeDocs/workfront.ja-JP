---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] でのモジュールまたはシナリオのコピー'
description: ' [!DNL Adobe Workfront Fusion] でのモジュールまたはシナリオのコピー'
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '806'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのモジュールまたはシナリオのコピー 

[!DNL Adobe Workfront Fusion] では、モジュール、モジュールのグループ、またはシナリオ全体をコピーできます。この機能を使用すると、シナリオやシナリオの一部を再び構築しなくても再利用できます

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select]または[!UICONTROL Prime]の [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

モジュールをコピーする前に、シナリオにモジュールを追加する必要があります。

## モジュールまたはモジュールのグループのコピー

モジュールをコピーすると、コピー元のモジュールのすべてのフィールド値と設定が保持されます。

モジュールを同じシナリオの別の領域に貼り付けたり、別のシナリオにペーストしたりできます。

モジュールを別のシナリオにペーストする場合は、次の点を考慮してください。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* コピーしなかった別のモジュールから情報を取り込むフィールド値は、その情報にアクセスできなくなります。新しいシナリオから情報を取り込むには、これらのフィールドを設定する必要があります。
* 別のチームまたは組織が所有するシナリオにモジュールをペーストする場合は、すべての接続を、新しいシナリオを所有するグループまたは組織が所有する接続に更新する必要があります。

### モジュールのコピー

モジュールのグループをコピーする方法は、単一のモジュールをコピーする場合と似ています。

1. コピーするモジュールを右クリックします。

   >[!NOTE]
   >
   >[!UICONTROL shift] を押しながらコピーするモジュールをクリックすると、複数のモジュールを選択できます。モジュールのグループをコピーすると、接続線、フィルター、ルーティングロジックもコピーされます。

1. 「**[!UICONTROL モジュールをコピー]**」を選択します。
1. シナリオのコピー先となる領域にカーソルを移動します。
1. 右クリックし、「**[!UICONTROL ペースト]**」を選択します。
1. ペーストしたモジュールをシナリオ内の適切な場所にドラッグして、シナリオに接続します。

   キーボードショートカットを使用してコピー＆ペーストすることもできます。

## クローンによるシナリオのコピー

シナリオをクローンすると、シナリオのコピーが作成され、編集できます。

1. シナリオの詳細ページを開きます。

   1. 左パネルの「**[!UICONTROL シナリオ]**」タブをクリックし、詳細が必要なシナリオをクリックします。

      または

      [ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) のシナリオエディターでシナリオを使用している場合は、ウィンドウの左上隅付近にある左向き矢印 ![](assets/exit-editing-arrow.png) をクリックします。

1. ページの右上隅にある「**[!UICONTROL オプション]**」を右クリックします。
1. 「**[!UICONTROL クローン]**」を選択します。
1. （オプション）新しいシナリオの名前を入力します。
1. （オプション）「**[!UICONTROL 新しいモジュールの状態を複製されるモジュールと同じ状態に保つ]**」を有効にして、コピーされたシナリオに元のシナリオで処理された最新のレコードに関する情報も確実に含まれるようにします。
1. 「**[!UICONTROL 保存]**」をクリックしてシナリオを作成します。

## ブループリントを使用したシナリオのコピー

シナリオのブループリントは、特定の時点での特定のシナリオの配置、マッピング、フィールド値を表します。シナリオのブループリントをコンピューター上の JSON ファイルに書き出し、シナリオの新規作成時に読み込むことができます。シナリオのブループリントから読み込んだシナリオは編集できます。

シナリオのブループリントは、シナリオ全体を表します。シナリオから特定のモジュールのみをコピーする場合は、「[モジュールまたはモジュールのグループのコピー](#copy-a-module-or-a-group-of-modules)」を参照してください。

>[!NOTE]
>
>[!DNL Adobe Workfront] のコンテキストにおけるブループリントの詳細については、[ブループリントの概要](../../administration-and-setup/blueprints/blueprints-overview.md)を参照してください。

### シナリオのブループリントの書き出し

1. シナリオのシナリオ設定エリアで、**[!UICONTROL その他]**&#x200B;メニューをクリックします。
1. 「**[!UICONTROL ブループリントを書き出し]**」をクリックします。

   JSON ファイルが作成され、コンピューターにダウンロードされます。このファイルは、[!DNL Downloads] フォルダーにあります。

### ブループリントの読み込み

>[!IMPORTANT]
>
>ブループリントを既存のシナリオに読み込むと、既存のシナリオがシナリオのブループリントに置き換えられます。既存のシナリオにブループリントを追加することはできません。

1. シナリオの新規作成を開始します。
1. シナリオのシナリオ設定エリアで、**[!UICONTROL その他]**&#x200B;メニューをクリックします。
1. 「**[!UICONTROL ブループリントを読み込み]**」をクリックします。
1. 表示されるダイアログで、「**[!UICONTROL 参照]**」をクリックします。
1. 読み込むブループリントに移動し、「**[!UICONTROL 開く]**」をクリックします。
1. 「**[!UICONTROL 保存]**」をクリックします。

   JSON ファイルが作成され、コンピューターにダウンロードされます。このファイルは、[!UICONTROL ダウンロード]フォルダーにあります。

## テンプレートを使用したシナリオのコピーおよび再利用

[!DNL Workfront Fusion] シナリオの開始点としてテンプレートを作成できます。テンプレートからシナリオを作成する場合、テンプレートを変更せずにシナリオを変更できます。テンプレートには、フィールドの値は保存されません。

テンプレートの作成と使用について詳しくは、[シナリオテンプレート](../../workfront-fusion/scenarios/templates/fusion-templates.md)を参照してください。
