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
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 99%

---

# [!UICONTROL SOAP] モジュール

[!UICONTROL SOAP]モジュールを使用して、[!UICONTROL Adobe Workfront Fusion]で[!UICONTROL SOAP]API に接続できます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL SOAP] モジュールの使用

[!UICONTROL SOAP] モジュールは現在ベータ版であり、次の機能をサポートしていません。

* 要素の再定義
* 小数部桁数の制限
* 合計桁数の制限
* 空白の制限
* マルチパートの入出力メッセージ。シングルパートメッセージのみがサポートされています。
* [[!UICONTROL SOAP] エンコーディング](https://schemas.xmlsoap.org)スキーマおよび要素を活用して定義されたカスタム XML スキーマ要素

>[!INFO]
>
>**例：**
>  
>以下は、[!UICONTROL Workfront Fusion] では正しく認識されません。
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

これには `soapenc:Array`、`soapenc:arrayType` および `wsdl:arrayType` 参照が含まれていますが、これらは [!UICONTROL Workfront Fusion] ではまだサポートされていません。

## 回避策

[!UICONTROL SOAP] モジュールが WSDL ファイルの処理を拒否するか、モジュールの設定で様々なエラーが発生する場合は、代わりに、汎用の **[!UICONTROL HTTP]／[!UICONTROL リクエストの実行]**&#x200B;モジュールを使用してみてください。

1. [!DNL Workfront Fusion] で新しいシナリオを作成します。
1. シナリオに **[!UICONTROL HTTP]／[!UICONTROL リクエストの実行]**&#x200B;モジュールを挿入します。
1. モジュールの設定を開き、次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL Enabled]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. 新しい Web ブラウザーウィンドウまたはタブを開きます。
1. WSDL URL を Web ブラウザーのアドレスバーに貼り付け、XML ファイルを取得します。

   通常、WSDL URL の末尾は `?wsdl` になりますが、そうでない場合もあります。例：`http://voip.ms/api/v1/server.wsdl`

1. WSDL ファイルが Web ブラウザーに直接表示されない場合は、ダウンロードしたファイルをテキストエディターで開きます。
1. 次の `<service>` または `<wsdl:service>` タグを探します。

   ![](assets/service-350x65.png)

1. 見つかったら、`location` 属性から URL をコピーします。
1. [!DNL Workfront Fusion] で、URL を HTTP モジュールの「URL」フィールドに貼り付けます。
1. 新しい Web ブラウザーウィンドウまたはタブで、「[オンライン [!UICONTROL SOAP] クライアント](https://wsdlbrowser.com/)」を開きます。
1. WSDL URL を「WSDL URL」フィールドに貼り付けます。
1. 「**[!UICONTROL 参照]**」をクリックします。
1. 左側の機能のリストから選択します。例：`getLanguages`
1. 「[!UICONTROL XML をリクエスト]」テキストエリアの内容をコピーします。
1. [!UICONTROL Workfront Fusion] で、コピーした内容をモジュールの「URL」フィールドに貼り付けます。
1. 疑問符を実際の値に置き換えることで、選択したパラメーターの値を指定します。

   ![](assets/request-xml-350x172.png)

1. 「**[!UICONTROL OK]**」をクリックしてモジュールの設定を閉じます。
1. シナリオまたはモジュールを実行します。
