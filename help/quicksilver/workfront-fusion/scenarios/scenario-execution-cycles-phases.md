---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] でのシナリオの実行、サイクル、フェーズ'
description: この記事では、 [!DNL Adobe Workfront Fusion]  シナリオ実行時に発生するイベント（初期化、操作、コミット、ロールバックなど）について説明します。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '550'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのシナリオの実行、サイクル、フェーズ

[!DNL Adobe Workfront Fusion] は、リレーショナルデータベースと同様のトランザクションシステムです。各シナリオの実行は、初期化フェーズから開始され、操作フェーズとコミット／ロールバックフェーズで構成される 1 つ以上のサイクルが続き、最終化フェーズで終了します。

>[!INFO]
>
>**例**
>
>初期化
>
>サイクル 1
>
>操作（読み取りまたは書き込み）
>
>コミットまたはロールバック
>
>サイクル 2
>
>操作（読み取りまたは書き込み）
>
>コミットまたはロールバック
>
>...
>
>サイクル N
>
>操作（読み取りまたは書き込み）
>
>コミットまたはロールバック
>
>最終化

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 初期化

初期化フェーズ中に、必要な接続（データベース、メールサービスなどへの接続）がすべて作成されます。また、各モジュールが意図した操作を実行できるかどうかも確認されます。

## サイクル

各サイクルは、一連の操作で構成される、分割できない作業単位を表します。サイクルの最大数は、[!UICONTROL シナリオ設定]パネルで設定することができます。デフォルト値は 1 です。

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md) のシナリオ設定パネルを参照してください。

## 操作

操作フェーズの読み取り／書き込み操作中に、次の操作が実行されます。

* 読み取り操作は、事前に定義されたシナリオに従って他のモジュールで処理されるサービスからデータを取得することで構成されます。例えば、[!UICONTROL Dropbox]／[!UICONTROL ファイルを監視]モジュールは、前回のシナリオ実行以降に作成された新しいバンドル（ファイル）を返します。
* 書き込み操作は、さらに処理するために、特定のサービスにデータを送信することで構成されます。例えば、[!DNL Dropbox]／[!UICONTROL ファイルをアップロード]モジュールは、ファイルを [!DNL Dropbox] フォルダーにアップロードします。

## コミット

すべてのモジュールに対して操作フェーズが成功した場合、コミットフェーズが開始され、その間に、モジュールで実行されたすべての操作がコミットされます。つまり、[!DNL Workfront Fusion] では、操作フェーズに関与するすべてのサービスに、その成功に関する情報を送信します。

## ロールバック

任意のモジュールで操作中またはコミットフェーズ中にエラーが発生した場合は、フェーズが中止され、ロールバックフェーズが開始されて、指定されたサイクル中のすべての操作が無効になります。一部のモジュールでは、ロールバックをサポートしておらず、これらのモジュールで実行された操作を取り消すことができません。詳しくは、[ACID モジュール](#acid-modules)の節を参照してください。

## 最終化

最終化フェーズでは、開いている接続（FTP 接続やデータベース接続など）が閉じられ、シナリオが完了します。

## ACID モジュール

ロールバック（トランザクション性とも呼ばれます）をサポートしているすべての [!DNL Workfront Fusion] モジュールは、ACID タグでマークされます。

![](assets/acid-modules-350x189.png)

このタグでマークされていないモジュールは、他のモジュールでエラーが発生した場合でも、初期状態に戻すことはできません。非 ACID モジュールの典型的な例は、[!UICONTROL メール]／[!UICONTROL メールの送信]アクションです。メールの送信後は、送信を取り消すことはできません。
