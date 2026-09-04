---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Canvas ダッシュボードのコピー
description: カンバスダッシュボードをコピーして、オーディエンス固有のコピーなど、そのバリエーションを作成できます。その際、最初から再構築する必要はありません。
author: Courtney
feature: Reports and Dashboards
source-git-commit: b66f6931ee2fe83688fb8910861af6e958d1f74f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 16%

---

# Canvas ダッシュボードのコピー

{{highlighted-preview-article-level}}

>[!IMPORTANT]
>
>Canvas ダッシュボード機能は現在、ベータ版ステージに参加しているユーザーのみが利用できます。 機能の一部が完了していないか、この段階で意図したとおりに動作しない可能性があります。 ご利用のエクスペリエンスに関するフィードバックは、Canvas ダッシュボードのベータ版の概要記事の「[ フィードバックを提供](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)」セクションの手順に従って送信してください。<br>
>バグや技術的な問題についてフィードバックがある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[カスタマーサポートに連絡](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。<br>
>このベータ版は、次のクラウドプロバイダーでは利用できないことに注意してください。
>
>* Amazon Web Services用に独自のキーを持ち込む
>* Azure
>* Google Cloud Platform

Canvas ダッシュボードをコピーして、エグゼクティブダッシュボードのディレクターレベルのコピーなど、別のオーディエンス向けにバリエーションを作成できます。最初から再構築する必要はありません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>標準 </p> 
<p>プラン</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>ダッシュボードの編集またはアクセス権の作成</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>ダッシュボードへのアクセスを表示</p>
  </td> 
  </tr>
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## 前提条件

ダッシュボードを複製する前に、ダッシュボードを作成する必要があります。

詳しくは、[ キャンバスダッシュボードの作成](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)を参照してください。

## ダッシュボードのコピー

>[!NOTE]
>
>共有の環境設定は、新しいダッシュボードにコピーされません。 ウィジェットに&#x200B;**ユーザーとして実行**&#x200B;設定がある場合、その設定は、指定ユーザーまたはシステム管理者の場合にのみコピーに保存されます。

ダッシュボードをコピーするには：

{{step1-to-dashboards}}

1. 左側のパネルで、「**キャンバスダッシュボード**」をクリックします。

1. **Canvas ダッシュボード** ページで、コピーするダッシュボードを開きます。

1. 右上隅の&#x200B;**詳細** ![詳細アイコン ](assets/more-icon.png) アイコンを選択し、**コピー**を選択します。
   ![ ダッシュボードのメニューオプションをコピー](assets/duplicate-dashboard.png)

1. **ダッシュボードをコピー** ダイアログボックスで、新しいダッシュボードの&#x200B;**名前**&#x200B;を入力します。デフォルトでは、ソースダッシュボードの名前の後に「（コピー）」が続きます。

1. （オプション）「**ダッシュボードの詳細**」タブで、新しいダッシュボードの&#x200B;**説明**&#x200B;または&#x200B;**通貨**を更新します。
   ![ ダッシュボードをコピー – ダッシュボードの詳細タブ ](assets/duplicate-details.png)

1. （オプション）「**ウィジェット**」タブをクリックし、重複するダッシュボードに含めたくないウィジェットの選択を解除します。
   ![ ダッシュボードをコピー – 「ウィジェット」タブ ](assets/copy-widgets.png)

1. （オプション）「**フィルターとプロンプト**」タブをクリックし、**ダッシュボードフィルターのコピー**&#x200B;または&#x200B;**ダッシュボードプロンプトのコピー**をオフにして、重複したダッシュボードから除外します。
   ![ ダッシュボードをコピー – 「フィルターとプロンプト」タブ ](assets/copy-filters.png)

1. 「**ダッシュボードをコピー**」をクリックします。

確認メッセージが表示され、新しいダッシュボードへのリンクが表示されます。
