---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: cURL を使用した HTTP モジュールの追加
description: cURL リクエストをシナリオに貼り付けると、Fusion は cURL リクエストから設定された HTTP モジュールを作成します。
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 785f39fabcb19233fd1bc79c14222225a3ea72a2
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 17%

---

# cURL を使用した HTTP モジュールの追加

cURL リクエストをシナリオに貼り付けると、Fusion は cURL リクエストから設定された HTTP モジュールを作成します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront プラン</td>  
      <td>任意</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront プラン</td>  
      <td>
        新規：標準 <br>
        または <br>
        現在：仕事以上
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion ライセンス</td>  
      <td> 
        現在：Workfront Fusion ライセンスは必要ありません。<br>
        または <br>
        レガシー：任意
      </td>  
    </tr>  
    <tr>  
      <td>製品</td>  
      <td> 
        新規：Adobe Workfront Workfront プランを選択またはPrimeを購入する必要があります。<br>
        Ultimate Workfront プラン：Workfront Fusion が含まれています。<br>
        または <br>
        現在：Adobe Workfront Fusion を購入する必要があります。
      </td>  
    </tr> 
  </tbody>  
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

+++

## cURL リクエストからの HTTP モジュールの作成


cURL を使用して HTTP モジュールを作成するには：

1. Fusion の外部（テキストエディターなど）で cURL リクエストのテキストを作成します。
1. cURL リクエストをクリップボードにコピーします。
1. 左側のパネルで「**[!UICONTROL シナリオ]**」タブをクリックします。
1. モジュールを作成するシナリオを選択します。
1. シナリオの任意の場所をクリックして、シナリオエディターに移動します。
1. シナリオエディターの任意の空白を右クリックして、「**貼り付け**」を選択します。

   または

   Ctrl + V （Windows）または Cmd + V （Mac）を押します。


   HTMLモジュールが作成されます。
1. モジュールをドラッグして、シナリオに接続します。

## トラブルシューティング

cURL がシナリオに貼り付けられていない場合は、ブラウザー設定を調べ、クリップボードからの貼り付けが有効になっていることを確認します。


