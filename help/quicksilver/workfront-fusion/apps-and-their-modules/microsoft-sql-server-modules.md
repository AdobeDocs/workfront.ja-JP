---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server モジュール
description: 以下を使用できます。 [!DNL Adobe Workfront Fusion] Microsoft SQL Server に接続するには、以下を実行します。
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# [!DNL Microsoft SQL Server] モジュール

以下を使用できます。 [!DNL Adobe Workfront Fusion] 接続する [!UICONTROL Microsoft SQL Server].

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

## 使用 [!DNL Microsoft SQL Server] モジュール

ストアドプロシージャを使用して、カスタムロジックをデータベースサーバー上で直接実行できます。 [!DNL Adobe Workfront Fusion] 入力/出力パラメータとレコードセットのインターフェイスを動的に読み込み、各パラメータまたは値を個別にマッピングできます。 シナリオの設定を開始する前に、データベースに接続するために使用するアカウントに、への読み取りアクセス権があることを確認してください `INFORMATION_SCHEMA.ROUTINES` および `INFORMATION_SCHEMA.PARAMETERS` ビュー。

条件 [!DNL Fusion] に対する接続を確立する [!DNL SQL server] 宛先、 [!DNL Fusion] ユーザーは、ホスト（サーバーがホストされているドメイン名または IP アドレス）とポートを識別します。 [!DNL Fusion] は、使用可能な任意のホストおよびポートに接続できます。

で使用される特定の IP アドレスに関する情報 [!DNL Workfront Fusion]を参照してください。 [アクセス用の IP アドレス [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

ストアドプロシージャの作成の詳細については、 [!DNL Microsoft SQL Server] ドキュメント。

>[!NOTE]
>
>[!DNL Workfront Fusion] では、複数のレコードセットをサポートしていません。 最初の処理のみが処理されます。

## エラーのトラブルシューティング [!UICONTROL ER_LOCK_WAIT_TIMEOUT:ロック待機のタイムアウトを超えました。トランザクションを再開する]

このエラーは、複数のモジュールを使用して同じデータを変更する場合に発生します。 SQL トランザクションが原因です。

SQL モジュールが実行されると、トランザクションが開始されます。 シナリオが完全に実行された後に、トランザクションが完了します。

別のモジュールが同じデータにアクセスしようとした場合は、前のトランザクションが終了するまで待つ必要があります。 シナリオの終了後に最初のトランザクションが完了するので、2 番目のトランザクションは開始できません。

### 解決策：

自動コミットをオンにします。 自動コミットは、モジュールの実行が完了した直後にすべてのトランザクションを完了（コミット）します。

1. 次をクリック： [!UICONTROL シナリオ設定] アイコン ![](assets/scenario-settings-icon.png)画面の下部に表示されます。
1. 次をクリック： **[!UICONTROL 自動コミット]** チェックボックス。
1. クリック **[!UICONTROL OK]** をクリックして、シナリオ設定を保存します。
