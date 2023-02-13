---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: のデータストア [!DNL Adobe Workfront Fusion]
description: データストアは、データベースやシンプルなテーブルと同様に、シナリオのデータを格納し、個々のシナリオやシナリオの実行間でデータを転送できます。 データストアを使用すると、同期中に様々なシステムから新しいデータを保存できます。
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# のデータストア [!DNL Adobe Workfront Fusion]

データストアは、データベースやシンプルなテーブルと同様に、シナリオのデータを格納し、個々のシナリオやシナリオの実行間でデータを転送できます。 データストアを使用すると、同期中に様々なシステムから新しいデータを保存できます。

データストアモジュールを使用すると、 [!DNL Adobe Workfront Fusion] データストア：

* 追加
* 置き換え
* 更新
* 取得
* 削除
* 検索
* カウント

データストアモジュールの使用について詳しくは、 [[!UICONTROL データストア] モジュール](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

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

## にデータストアを作成する [!DNL Workfront Fusion]

* [データストアのセットアップ](#set-up-the-data-store)
* [データ構造の設定](#set-up-the-data-structure)

### データストアのセットアップ

モジュールでデータストアを使用する前に、次の場所にデータストアを作成する必要があります。 [!DNL Workfront Fusion].

>[!NOTE]
>
>組織に使用可能なデータストアの数が制限されています。 使用可能な数を超えるデータストアを作成しようとする場合、 [!DNL Workfront] は [!UICONTROL 最大店舗数に達しました] エラー。
>
>詳しくは、 [最大ストア数到達エラー](#maximum-stores-reached-error) 」を参照してください。

1. にログインします。 [!DNL Workfront Fusion] アカウント
1. クリック **[!UICONTROL データストア]** をクリックします。
1. クリック **[!UICONTROL データストアを追加]** をクリックします。
1. 新しいデータストアの設定を入力します。

   フィールドの太字のタイトル [!DNL Workfront Fusion] モジュールは、必要な設定を示します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL データストア名 ] </td> 
      <td> <p>データストアの名前を入力します。 </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL データ構造 ]</p> </td> 
      <td> <p>データ構造は、テーブルの列のリストです。 このリストは、列名とデータタイプを示します。</p> <p>次のいずれかの操作を行います。</p> 
       <ul> 
        <li style="font-weight: bold;">作成済みのデータ構造を選択</li> 
        <li> <p style="font-weight: bold;">新しいデータ構造を追加</p> <p>クリック <strong>[!UICONTROL 追加 ]</strong> をクリックして、新しいデータ構造を作成します。</p> <p>詳しくは、 <a href="#set-up-the-data-structure" class="MCXref xref">データ構造の設定</a> 」の節を参照してください。</p> </li> 
        <li style="font-weight: bold;"> <p>このフィールドは空のままにします</p> <p style="font-weight: normal;">データ構造を選択または追加しない場合、データベースにはプライマリキーのみが含まれます。 このようなデータベースタイプは、キーのみを保存する場合に便利で、特定のキーがデータベースに存在するかどうかのみを知る必要があります。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL データストレージサイズ（MB 単位）]</p> </td> 
      <td> <p>データストアのサイズを、総内部データストレージから割り当てます。</p> <p>注意：予約金額はいつでも変更できます。</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### データ構造の設定

1. データストアを作成または編集する際に、 **[!UICONTROL 追加]**.
1. 内 **[!UICONTROL データ構造を追加]** 表示されるボックスで、次のフィールドを設定します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL データ構造名 ]</td> 
      <td> <p> 新しいデータ構造の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL の仕様 ]</p> </td> 
      <td> <p>データストアの列を設定するには、次のいずれかの操作を行います。</p> 
       <ul> 
        <li> <p>クリック <strong>[!UICONTROL 項目を追加 ]</strong> をクリックして、1 つの列のプロパティを手動で指定します。</p> <p>次を入力します。 <strong>[!UICONTROL 名前 ]</strong> および <strong>[!UICONTROL の種類 ]</strong> データストア列のを参照し、対応するプロパティを定義します。</p> </li> 
        <li> <p>クリック <strong>[!UICONTROL Generator]</strong> を使用して、指定したサンプルデータから列を特定します。</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>例: </b></span></span> 
          <p>例えば、次の JSON サンプルデータは 3 つの列を作成します。名前、年齢および電話番号。 電話番号は、携帯電話および固定電話の電話番号を集めたものです。</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>データストア表示の空の列：</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>その後、手動で値をデータストアに追加するか、 [!DNL Workfront Fusion] データストアモジュール。</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>ペイロードがデータ構造と一致するようにするには、このオプションを有効にします。 データ構造で指定されていない追加の項目を含むペイロードは拒否されます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 既存のデータストアの編集

既存のデータストアのプロパティとコンテンツは、 [!UICONTROL データストア] ～の面積 [!DNL Workfront Fusion].

* [データストアのプロパティを編集する](#edit-the-properties-of-a-data-store)
* [データストアのコンテンツの編集](#edit-the-contents-of-a-data-store)

### データストアのプロパティを編集する

データストアのプロパティには、データストアが使用するデータ構造と、データストアのサイズが含まれます。

1. クリック **[!UICONTROL データストア]** ![](assets/data-store-icon.png) 左側のナビゲーションパネルで、 [!UICONTROL データストア] 領域
1. クリック **[!UICONTROL 編集]** ![](assets/data-store-edit.png) をクリックします。
1. （オプション）このデータストアで使用するデータ構造を別の既存のデータ構造に変更する場合は、 **[!UICONTROL データ構造]** 」ドロップダウンリストから選択できます。

   または

   （オプション）このデータストアで使用するデータ構造をまったく新しいデータ構造に変更する場合は、 [データ構造の設定](#set-up-the-data-structure) 」を参照してください。

1. （オプション）新しいサイズを **[!UICONTROL データストレージサイズ (MB)]** フィールドに入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

### データストアのコンテンツの編集

1. 次をクリック： **[!UICONTROL データストア]** アイコン ![](assets/data-store-icon.png) 左側のナビゲーションパネルで、 [!UICONTROL データストア] 領域
1. クリック **[!UICONTROL 参照]** ![](assets/browse-data-store.png) をクリックします。
1. （オプション）列を目的の場所にドラッグして並べ替えます。
1. （オプション） [!UICONTROL 編集] 単一のセルを選択するには、 **[!UICONTROL 編集]** アイコン ![](assets/data-store-edit.png)を選択し、必要な値を入力します。
1. （オプション）「 **[!UICONTROL 追加]**&#x200B;をクリックし、新しい項目の情報を入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

## トラブルシューティング

* [データストアから失われたデータの復元](#restoring-lost-data-from-a-data-store)
* [スペース不足エラー](#out-of-space-error)
* [最大ストア数到達エラー](#maximum-stores-reached-error)

### データストアから失われたデータの復元

現在、失われたデータの復元を自動化できるツールはありません。

#### 回避策

1. 項目がデータストアに挿入されたシナリオのすべての実行ログを調べます。

   実行ログの調査について詳しくは、 [でのシナリオの実行履歴の表示 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. データをコピーします。
1. データをデータストアに再度挿入します。

   データストアへのデータの挿入について詳しくは、 [データストアのコンテンツの編集](#edit-the-contents-of-a-data-store) 」を参照してください。

### [!UICONTROL スペースが不足しています] エラー

An [!UICONTROL スペース不足] 以前に作成したデータストアが割り当て済みのデータストアストレージに既に割り当てられているので、エラーが発生します。

#### 回避策

1. 既存のデータストアを編集して、使用スペースを減らします。 これにより、新しいデータストアの容量が解放されます。

   詳しくは、 [データストアのプロパティを編集する](#edit-the-properties-of-a-data-store) 」を参照してください。

>[!NOTE]
>
>より多くのデータストアが必要でないことが確実でない限り、すべてのスペースを 1 つのデータストアに割り当てないことをお勧めします。

### [!UICONTROL 最大店舗数に達しました] エラー

A [!UICONTROL 最大店舗数に達しました] エラーが発生するのは、組織が使用可能なすべてのデータストアを使用しているためです。 組織には、使用可能なデータストアの数が、使用可能なシナリオの数の 2 倍に等しい数があります。 したがって、利用可能なデータストアの合計数は、購入したプランによって異なります。

例えば、組織が 15 件のシナリオでプランを購入した場合、組織は最大 30 店舗のデータストアを保有できます。

#### 回避策

既存のデータストアの数を減らすには、次のいずれかの操作を検討します。

* 既存のデータストアを結合する
* 未使用のデータストアを削除
