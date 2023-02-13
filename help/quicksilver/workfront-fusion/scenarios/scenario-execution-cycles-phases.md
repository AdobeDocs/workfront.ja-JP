---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]
description: この記事では、 [!DNL Adobe Workfront Fusion] シナリオが実行されている状態（初期化、操作、コミット、ロールバックなど）。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] は、リレーショナルデータベースと同様のトランザクションシステムです。 各シナリオの実行は、初期化フェーズから開始され、操作フェーズとコミット/ロールバックフェーズで構成される 1 つ以上のサイクルが続き、最終化フェーズで終了します。

>[!INFO]
>
>**例**
>
>初期化
>
>サイクル#1
>
>操作（読み取りまたは書き込み）
>
>コミットまたはロールバック
>
>サイクル#2
>
>操作（読み取りまたは書き込み）
>
>コミットまたはロールバック
>
>...
>
>サイクル#N
>
>操作（読み取りまたは書き込み）
>
>コミットまたはロールバック
>
>確定

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA) </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 初期化

初期化フェーズ中に、必要な接続（データベースへの接続、E メールサービスなど）がすべて作成されます。 また、各モジュールが意図した操作を実行できるかどうかも確認されます。

## サイクル

各サイクルは、一連の操作で構成される、分割できない作業単位を表します。 サイクルの最大数を [!UICONTROL シナリオ設定] パネル。 デフォルト値は 1 です。

詳しくは、 [のシナリオ設定パネル [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 操作

操作フェーズの読み取り/書き込み操作の実行中：

* 読み取り操作は、事前に定義されたシナリオに従って他のモジュールで処理されるサービスからデータを取得することで構成されます。 例えば、 [!UICONTROL Dropbox] >[!UICONTROL 監視ファイル] モジュールは、前回のシナリオ実行以降に作成された新しいバンドル（ファイル）を返します。
* 書き込み操作は、さらに処理するために、特定のサービスにデータを送信することで構成されます。 例えば、 [!DNL Dropbox] >[!UICONTROL ファイルのアップロード] モジュールは、ファイルを [!DNL Dropbox] フォルダー。

## コミット

すべてのモジュールに対して操作フェーズが成功した場合、コミットフェーズが開始され、その間に、モジュールによって実行されたすべての操作がコミットされます。 つまり、 [!DNL Workfront Fusion] は、操作フェーズに関係するすべてのサービスに、その成功に関する情報を送信します。

## ロールバック

任意のモジュールの操作中またはコミットフェーズ中にエラーが発生した場合は、フェーズが中止され、ロールバックフェーズが開始され、指定されたサイクルの無効化中にすべての操作が行われます。 一部のモジュールはロールバックをサポートしておらず、これらのモジュールで実行された操作を取り戻すことができません。 詳しくは、 [ACID モジュール](#acid-modules) 」セクションに入力します。

## 確定

終了段階で、開いている接続（FTP 接続、データベース接続など）が閉じられ、シナリオが完了します。

## ACID モジュール

すべて [!DNL Workfront Fusion] ロールバック（トランザクションとも呼ばれます）をサポートするモジュールには、ACID タグが付けられます。

![](assets/acid-modules-350x189.png)

他のモジュールでエラーが発生した場合、このタグでマークされていないモジュールを元の状態に戻すことはできません。 非 ACID モジュールの典型的な例は、 [!UICONTROL 電子メール] >[!UICONTROL メールの送信] アクション。 E メールの送信後は、送信を取り消すことはできません。
