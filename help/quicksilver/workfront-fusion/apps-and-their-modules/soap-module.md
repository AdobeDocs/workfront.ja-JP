---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: SOAP モジュール
description: SOAP モジュールを使用して、Adobe Workfront Fusion で SOAP API に接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# [!UICONTROL SOAP モジュール]

以下を使用して、 [!UICONTROL SOAP] 接続するモジュール [!UICONTROL SOAP] の API [!UICONTROL Adobe Workfront Fusion].

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
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

## の使用 [!UICONTROL SOAP] モジュール

この [!UICONTROL SOAP] モジュールは現在ベータ版で、次の機能をサポートしていません。

* 要素の再定義
* 分数の桁数制限
* 合計桁数制限
* 空白の制限
* 入出力メッセージの複数の部分。 単一パーツのメッセージのみがサポートされます
* の助けを借りて定義されたカスタム XML スキーマ要素 [[!UICONTROL SOAP] エンコード](http://schemas.xmlsoap.org) スキーマと要素。

>[!INFO]
>
>**例:**
>  
>以下は、 [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```

これには、 `soapenc:Array`, `soapenc:arrayType` および `wsdl:arrayType` 参照 ( まだ [!UICONTROL Workfront Fusion].

## 回避策

この [!UICONTROL SOAP] モジュールは WSDL ファイルの処理を拒否するか、モジュールの設定で様々なエラーをスローします。ユニバーサル **[!UICONTROL HTTP] > [!UICONTROL リクエストを実行]** 代わりにモジュールを使用します。

1. In [!DNL Workfront Fusion]、新しいシナリオを作成します。
1. を **[!UICONTROL HTTP] > [!UICONTROL リクエストを実行]** モジュールを設定します。
1. モジュールの設定を開き、次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL メソッド ]</td> 
      <td> <p>[!UICONTROLPOST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 本文の種類 ]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL コンテンツタイプ ]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 応答を解析 ]</td> 
      <td>[!UICONTROL 有効 ]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. 新しい Web ブラウザーウィンドウまたはタブを開きます。
1. WSDL URL を Web ブラウザーのアドレスバーに貼り付け、XML ファイルを取得します。

   WSDL URL は通常、で終わります `?wsdl`必ずしもそうではありません。 `http://voip.ms/api/v1/server.wsdl`.

1. WSDL ファイルが Web ブラウザーに直接表示されない場合は、ダウンロードしたファイルをテキストエディターで開きます。
1. を検索します。 `<service>` または `<wsdl:service>` タグ：

   ![](assets/service-350x65.png)

1. 見つかったら、 `location` 属性。
1. In [!DNL Workfront Fusion]「 」で、URL を HTTP モジュールの「 URL 」フィールドに貼り付けます。
1. を開きます。 [オンライン [!UICONTROL SOAP] クライアント](https://wsdlbrowser.com/) をクリックします。
1. WSDL URL を「WSDL URL」フィールドに貼り付けます。
1. クリック **[!UICONTROL 参照]**.
1. 左側の関数のリストから選択します。例： `getLanguages`.
1. 次の内容をコピー： [!UICONTROL XML をリクエスト] テキスト領域
1. In [!UICONTROL Workfront Fusion]」で、コピーした内容をモジュールの「 URL 」フィールドに貼り付けます。
1. 疑問符を実際の値に置き換えて、選択したパラメーターの値を指定します。

   ![](assets/request-xml-350x172.png)

1. クリックしてモジュールの設定を閉じる **[!UICONTROL OK]**.
1. シナリオまたはモジュールを実行します。
