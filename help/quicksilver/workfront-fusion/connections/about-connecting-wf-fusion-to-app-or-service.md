---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: ' [!DNL Adobe Workfront Fusion]  のアプリまたはサービスへの接続について'
description: ほとんどのアプリでは、接続を作成する必要があります。それによって、 [!DNL Adobe Workfront Fusion]  は特定のシナリオの設定に従って、特定のサードパーティサービスと通信できます。
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '402'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] のアプリまたはサービスへの接続について

ほとんどのアプリでは、接続を作成する必要があります。それによって、[!DNL Adobe Workfront Fusion] は特定のシナリオの設定に従って、特定のサードパーティサービスと通信できます。

例えば、[!DNL Workfront] からの情報を取得するシナリオを作成する場合は、[!DNL Workfront] アカウントにアクセスするために [!DNL Workfront Fusion] に対するアクセス権を付与する必要があります。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプやアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## アクセス権

すべての接続に対して、[!DNL Workfront Fusion] では、特定のシナリオを正常に完了するために必要なアクセス権のみが必要です。例えば、[!DNL Google Docs] からドキュメントを一覧表示するシナリオを作成する場合、[!DNL Workfront Fusion] ではドキュメントの内容を取得する権限は要求されません。

残念ながら、一部のサービスでは特定のタスクへのアクセスを制限できません。したがって [!DNL Workfront Fusion] には完全なアクセス権が必要です。これらのサービスに登録されたアカウントへの、[!DNL Workfront Fusion] のアクセスを制限する方法について詳しくは、アプリケーション固有のドキュメントを参照してください。

## 接続の管理について

すべての接続は、[!UICONTROL 接続]エリアから管理することができます。ここでは、次の操作を実行できます。

* 各接続について [!DNL Workfront Fusion] に付与された権限を確認
* 接続名を変更
* 既存の接続を再認証
* 既存の接続を削除
* サービスへの接続が正常に確立されたことを確認

[!UICONTROL 接続]エリアを開くには、左ナビゲーションの「<b>[!UICONTROL 接続]</b>」をクリックします。

## 接続を更新する

[!DNL Workfront Fusion] は通常、任意のサービスに対するアクセス権を無制限で取得します。ただし、必ずしもそうではない場合もあります。一部のサービスでは、一定期間後にアクセス権限を更新する必要があります。この場合、アクセス権が失効する直前に [!DNL Workfront Fusion] からメールで通知が届きます。

接続を更新するには：

1. **[!UICONTROL 接続]**&#x200B;エリアの「**[!UICONTROL 再認証]**」ボタンをクリックします。
