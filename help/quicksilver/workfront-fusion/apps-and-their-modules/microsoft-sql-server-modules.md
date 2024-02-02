---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server モジュール
description: ' [!DNL Adobe Workfront Fusion]  を使用して Microsoft SQL Server に接続することができます。'
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '391'
ht-degree: 100%

---

# [!DNL Microsoft SQL Server] モジュール

[!DNL Adobe Workfront Fusion] を使用して、[!UICONTROL Microsoft SQL Server] に接続することができます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
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

## [!DNL Microsoft SQL Server] モジュールの使用

ストアドプロシージャを使用して、カスタムロジックをデータベースサーバー上で直接実行できます。[!DNL Adobe Workfront Fusion] はレコードセットと入力／出力パラメーターのインターフェイスを動的に読み込み、各パラメーターまたは値を個別にマッピングできます。シナリオの設定を開始する前に、データベースに接続するために使用するアカウントに、`INFORMATION_SCHEMA.ROUTINES` および `INFORMATION_SCHEMA.PARAMETERS` ビューへの読み取りアクセス権があることを確認してください。

[!DNL Fusion] が [!DNL SQL server] の宛先へ接続を確立するとき、[!DNL Fusion] ユーザーはホスト（サーバーがホストされているドメイン名または IP アドレス）とポートを識別します。[!DNL Fusion] は、使用可能な任意のホストおよびポートに接続できます。

[!DNL Workfront Fusion] で使用される特定の IP アドレスに関する情報について詳しくは、[アクセス用の IP アドレス [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)を参照してください

ストアドプロシージャの作成について詳しくは、[!DNL Microsoft SQL Server] ドキュメントを参照してください。

>[!NOTE]
>
>[!DNL Workfront Fusion] では、複数のレコードセットをサポートしていません。最初の処理のみが処理されます。

## エラーのトラブルシューティング [!UICONTROL ER_LOCK_WAIT_TIMEOUT：ロック待機タイムアウトを超えました。トランザクションを再起動してください]

このエラーは、複数のモジュールを使用して同じデータを変更する場合に発生します。SQL トランザクションが原因です。

SQL モジュールが実行されると、トランザクションが開始されます。シナリオが完全に実行された後に、トランザクションが完了します。

別のモジュールが同じデータにアクセスしようとした場合は、前のトランザクションが終了するまで待つ必要があります。シナリオの終了後に最初のトランザクションが完了するので、2 番目のトランザクションは開始できません。

### 解決策：

自動コミットをオンにします。自動コミットは、モジュールの実行が完了した直後にすべてのトランザクションを完了（コミット）します。

1. 画面下部の[!UICONTROL シナリオ設定]アイコン ![](assets/scenario-settings-icon.png) をクリックします。
1. **[!UICONTROL 自動コミット]**&#x200B;チェックボックスをクリックします。
1. 「**[!UICONTROL OK]**」をクリックして、シナリオ設定を保存します。
