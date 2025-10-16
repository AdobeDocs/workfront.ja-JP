---
title: 拡張コネクターを使用したアセットおよびフォルダーのリンク
description: ドキュメントをサポートする任意の Workfront オブジェクトに Experience Manager Assets からアセットまたはフォルダーをリンクできます。
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 90%

---


# 拡張コネクターを使用したアセットおよびフォルダーのリンク

ドキュメントをサポートする任意の Workfront オブジェクトに Experience Manager Assets からアセットまたはフォルダーをリンクできます。Experience Manager Assets から送信されたアセットは、Workfront のドキュメントストレージ全体にはカウントされません。Workfront から Experience Manager Assets にアップロードおよび送信されたドキュメントは、全体的なストレージにカウントされます。


>[!NOTE]
>
>拡張コネクタを介してリンクされた Excel ファイルは、Workfrontでプレビューできません。 ファイルにアクセスするには、ファイルをダウンロードする必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>投稿者以上</p>
   <p>リクエスト以上</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">その他の製品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントへの表示アクセス権以上</p> </td> 
  </tr> 
 </tbody> 
</table>


詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

開始する前に、

* Workfront for Experience Manager 拡張コネクタをインストール

## Experience Manager Assets からのアセットのリンク

Experience Manager Assets から Workfront にアセットをリンクできます。アセットをリンクすると、次の操作が可能になります。

* [Experience Manager Assets のリンクされたアセットのプルーフ](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [ドキュメントの新しいバージョンをアップロードする](../../../documents/managing-documents/upload-new-document-version.md)

アセットを Experience Manager Assets にリンクするには：

1. ドキュメントを追加する Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動します。
1. 「**新規追加**」をクリックして、管理者が設定した Experience Manager Assets 統合を選択します。

   >[!NOTE]
   >
   >この統合には任意の名前を選択できるため、Experience Manager Assets について特に言及されていない場合があります。

1. 目的のアセットを選択します。

   ![&#x200B; アセットを選択 &#x200B;](assets/select-an-asset.png)

1. 「**リンク**」をクリックします。

## Experience Manager Assets からのフォルダーのリンク

フォルダー内の個々のアセットを表示する権限は、Experience Manager Assets 権限に依存します。

フォルダーを Experience Manager Assets にリンクするには：

1. ドキュメントを追加する Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動します。
1. 「**新規追加**」をクリックして、管理者が設定した Experience Manager Assets 統合を選択します。

   >[!NOTE]
   >
   >この統合には任意の名前を選択できるため、Experience Manager Assets について特に言及されていない場合があります。

1. 目的のフォルダーを選択します。

   ![&#x200B; フォルダーを選択 &#x200B;](assets/select-a-folder.png)

1. 「**リンク**」をクリックします。

## Experience Manager Assets からの新しいバージョンのリンク

Experience Manager Assets から新しいアセットを取り込み、Workfront で新しいバージョンとして既存のアセットに追加できます。ドキュメントが既にリンクされていて、Experience Manager Assets で新しいバージョンが追加されている場合、新しいバージョンは Workfront に自動的に表示されます。

>[!TIP]
>
>**ドキュメントの詳細**／**バージョン**&#x200B;に移動すると、アセットのすべてのバージョンを表示できます。

Experience Manager Assets から新しいバージョンをリンクするには：

1. ドキュメントを追加する Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動します。
1. 新しいバージョンに置き換えるアセットを選択します。リンクされたフォルダー内に新しいバージョンのアセットを作成することはできません。
1. 「**新規追加**」をクリックして、管理者が設定した Experience Manager Assets 統合を選択します。

   >[!NOTE]
   >
   >この統合には任意の名前を選択できるため、Experience Manager Assets について特に言及されていない場合があります。

1. 目的のアセットを選択します。

   ![&#x200B; アセットを選択 &#x200B;](assets/select-an-asset.png)

1. 「**リンク**」をクリックします。
