---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 接続の概要
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 22%

---

# 接続の概要

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ 接続の概要 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/connection-overview.html)
>* [ 接続の管理 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/manage-connections.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

<!-- Audited: 3/2024-->

ほとんどのアプリでは、[!DNL Workfront Fusion] は接続を必要とし、特定のシナリオの設定に従って指定されたサードパーティサービスと通信できます。

例えば、[!DNL Workfront] からの情報を取得するシナリオを作成する場合は、[!DNL Workfront] アカウントにアクセスするために [!DNL Workfront Fusion] に対するアクセス権を付与する必要があります。

接続は、Fusion がアプリケーションへのアクセスに使用する認証と権限を表します。 各アプリケーションに 1 つ以上の接続を作成し、複数のモジュールやシナリオで同じ接続を使用できます。

ほとんどの接続は、1 つのアプリケーションに対してのみ使用されます。 例えば、[!DNL Workfront] 接続は [!UICONTROL Salesforce] モジュールでは使用できません。 一部の [!DNL Adobe] アプリケーションは接続を共有できます。 詳しくは、[ アプリとそのモジュール ](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md) に一覧表示されている、これらのアプリケーションの記事を参照してください。

接続はチームレベルで管理されます。 チームのすべてのメンバーはチームの接続にアクセスでき、チーム外のユーザーはチームの接続にアクセスできません。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>レガシー：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>新規：</p> <ul><li>[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Workfront] プラン：[!DNL Adobe Workfront Fusion] を購入する必要があります。</li><li>[!UICONTROL Ultimate] [!DNL Workfront] プラン：[!DNL Workfront Fusion] が含まれています。</li></ul>
   <p>または</p>
   <p>現在：[!DNL Adobe Workfront Fusion] を購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## アクセス権

すべての接続に対して、[!DNL Workfront Fusion] では、特定のシナリオを正常に完了するために必要なアクセス権のみが必要です。例えば、[!DNL Google Docs] からドキュメントをリストするシナリオを作成し [!DNL Workfront Fusion] 場合、ドキュメントの内容を取得する権限は要求されません。 後でドキュメントのコンテンツにアクセスする必要があることがわかった場合は、接続を更新するか、そのコンテンツにアクセスできる新しい接続を作成します。

すべてのサービスで、特定のタスクへのアクセスを制限できるわけではありません。 このような場 [!DNL Workfront Fusion]、フルアクセス権が必要です。 これらのサービスに登録されたアカウントへの [!DNL Workfront Fusion] ーザーアクセスを制限する方法について詳しくは、[ アプリとそのモジュール ](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md) に記載されているアプリケーション固有のドキュメントを参照してください。

## 接続の管理

「[!UICONTROL  接続 ] エリアからすべての接続を管理できます。

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
1. （オプション）接続に対する [!DNL Workfront Fusion] ーザーに付与された権限を表示するには、その接続の表示アイコン ![ 接続権限を表示 ](assets/view-connection-permissions.png) をクリックします。
1. （オプション）接続の名前を変更するには、接続名をハイライト表示し、新しい名前を入力します。
1. （任意）接続を再認証するには、その接続の **再認証** をクリックします。
1. （任意）接続を削除するには、その接続の **削除** をクリックします。
1. （オプション）サービスへの接続が正常に確立されたことを確認するには、接続の **確認** をクリックします。



## 接続を更新する

[!DNL Workfront Fusion] は通常、任意のサービスに対するアクセス権を無制限で取得します。一部のアプリケーションでは、一定期間後にアクセス権限を更新する必要があります。 この場合、アクセス権が失効する直前に [!DNL Workfront Fusion] からメールで通知が届きます。

接続を更新するには：

1. **[!UICONTROL 接続]**&#x200B;エリアの「**[!UICONTROL 再認証]**」ボタンをクリックします。
