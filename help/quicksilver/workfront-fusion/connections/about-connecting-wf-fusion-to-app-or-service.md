---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 接続の概要
description: ほとんどのアプリでは、接続を作成する必要があります。それによって、 [!DNL Adobe Workfront Fusion]  は特定のシナリオの設定に従って、特定のサードパーティサービスと通信できます。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 27%

---

# 接続の概要

<!-- Audited: 3/2024-->

ほとんどのアプリでは、 [!DNL Workfront Fusion] 特定のシナリオの設定に従って、特定のサードパーティサービスと通信できる接続が必要です。

例えば、[!DNL Workfront] からの情報を取得するシナリオを作成する場合は、[!DNL Workfront] アカウントにアクセスするために [!DNL Workfront Fusion] に対するアクセス権を付与する必要があります。

接続は、Fusion がアプリケーションへのアクセスに使用する認証と権限を表します。 各アプリケーションに 1 つ以上の接続を作成し、複数のモジュールやシナリオで同じ接続を使用できます。

ほとんどの接続は、1 つのアプリケーションに対してのみ使用されます。 例： [!DNL Workfront] で接続を使用することはできません [!UICONTROL Salesforce] モジュール。 一部 [!DNL Adobe] アプリケーションは接続を共有できます。 詳細については、にリストされているアプリケーションの記事を参照してください [アプリとそのモジュール](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

接続はチームレベルで管理されます。 チームのすべてのメンバーはチームの接続にアクセスでき、チーム外のユーザーはチームの接続にアクセスできません。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL 作業 ] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在：いいえ [!DNL Workfront Fusion] ライセンス要件</p>
   <p>または</p>
   <p>レガシー：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>新規：</p> <ul><li>[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Workfront] プラン：組織による購入が必要です [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] プラン： [!DNL Workfront Fusion] が含まれます。</li></ul>
   <p>または</p>
   <p>現在：組織による購入が必要です。 [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## アクセス権

すべての接続に対して、[!DNL Workfront Fusion] では、特定のシナリオを正常に完了するために必要なアクセス権のみが必要です。例えば、ドキュメントをリストするシナリオを作成する場合、 [!DNL Google Docs], [!DNL Workfront Fusion] は、ドキュメントの内容を取得するために権限を要求しません。 後でドキュメントのコンテンツにアクセスする必要があることがわかった場合は、接続を更新するか、そのコンテンツにアクセスできる新しい接続を作成します。

すべてのサービスで、特定のタスクへのアクセスを制限できるわけではありません。 この場合、 [!DNL Workfront Fusion] フルアクセス権が必要です。 制限方法の詳細 [!DNL Workfront Fusion] これらのサービスに登録されたアカウントへのアクセスについては、に一覧表示されているアプリケーション固有のドキュメントを参照してください。 [アプリとそのモジュール](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## 接続の管理

すべての接続は、から管理できます。 [!UICONTROL 接続] 領域。

>[!NOTE]
>
>接続はチームが所有します。 探している接続が見つからない場合は、正しいチームを表示していることを確認してください。
>
>新しいチームを選択するには：
>
>* 左側のナビゲーションでチーム名をクリックし、新しいチームを選択します。
>
>    または
>
>* 左側のナビゲーションで「チームの概要」をクリックし、ページ上部付近のチーム名の横にあるドロップダウン矢印をクリックします。 新しいチームを選択します。

1. [!UICONTROL 接続]エリアを開くには、左ナビゲーションの「<b>[!UICONTROL 接続]</b>」をクリックします。
1. （オプション）環境とタイプのドロップダウンをクリックし、オプションを選択して、環境と接続のタイプを示します。
1. （オプション）付与された権限を表示するには [!DNL Workfront Fusion] 接続の場合、表示アイコンをクリックします ![接続権限の表示](assets/view-connection-permissions.png) その接続の。
1. （オプション）接続の名前を変更するには、接続名をハイライト表示し、新しい名前を入力します。
1. （オプション）接続を再認証するには、 **再認証** その接続の。
1. （オプション）接続を削除するには、 **削除** その接続の。
1. （オプション）サービスへの接続が正常に確立されたことを確認するには、 **検証** 接続の場合。



## 接続を更新する

[!DNL Workfront Fusion] は通常、任意のサービスに対するアクセス権を無制限で取得します。一部のアプリケーションでは、一定期間後にアクセス権限を更新する必要があります。 この場合、アクセス権が失効する直前に [!DNL Workfront Fusion] からメールで通知が届きます。

接続を更新するには：

1. **[!UICONTROL 接続]**&#x200B;エリアの「**[!UICONTROL 再認証]**」ボタンをクリックします。
