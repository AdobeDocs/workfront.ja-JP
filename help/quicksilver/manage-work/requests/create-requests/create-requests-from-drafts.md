---
product-area: requests
navigation-topic: create-requests
title: ドラフトからのリクエストの作成
description: 新しいリクエストを入力する際に Workfront が提案する利用可能なドラフトを使用する以外に、「ドラフト」セクションからドラフトリクエストにアクセスし、そこから送信を完了することもできます。
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 2c2ccbadd6470773808bbd5a205310fbb1e1944e
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 84%

---

# ドラフトからリクエストを作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

新しいリクエストを入力する際に Workfront が提案する利用可能なドラフトを使用する以外に、「ドラフト」セクションからドラフトリクエストにアクセスし、そこから送信を完了することもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：Contributor 以上</p>
   または
   <p>現在：Request 以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 製品</td> 
   <td> <ul><li>Adobe Workfront</li><li>計画リクエストまたはリクエストフォームを表示するには、Adobe Workfront Planning が必要です。</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ドラフトからリクエストを作成するための前提条件

ドラフトからリクエストを作成する前に、以下の操作を行う必要があります。

* リクエストの作成を開始します。これにより、リクエストがドラフトとして「ドラフト」セクションに自動的に保存されます。

  リクエストの作成について詳しくは、[Adobe Workfront リクエストの作成および送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

## ドラフトからリクエストを作成

{{step1-to-requests}}

1. 左側のパネルで「**ドラフト**」を選択します。

   それぞれのリクエストキューのそれぞれのキュートピックのドラフトがこのリストに表示されます。

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. （オプション）列の見出しをクリックして、その列でリストを並べ替えます。

1. ドラフトリストの以下の列で、それぞれのドラフトに関する情報を確認します。

   | 件名 | これは、リクエストの作成を開始したときにリクエストに付けた名前です。 |
   |---|---|
   | パス | 最初にリクエストを送信する予定だったリクエストキュー、トピックグループおよびキュートピックの名前。 |
   | エントリ日 | リクエストの作成を開始した日付。 |
   | 最終更新日 | 前回の更新。最初にリクエストを開始してから更新していない場合、エントリ日と最終更新日日は同じです。 |

   {style="table-layout:auto"}

1. （任意）ドラフトリストの右上隅にあるクイックフィルターを使用して、リクエストのドラフト、リクエストキュー、キュートピック、またはトピックグループの名前を入力し、続いてドラフトの名前をクリックして開きます。

   >[!TIP]
   >
   >リクエストエリアの「ドラフト」セクションでは、永続的なフィルターを適用できません。さらに、ドラフトリストの表示を修正したり変更したりするオプションもありません。

1. [Adobe Workfront リクエストの作成および送信](../../../manage-work/requests/create-requests/create-submit-requests.md)の説明に従って、リクエストの情報を更新します。
1. （オプションおよび条件付き）リクエストの入力中の任意の時点でドラフトを削除したい場合は、「**ドラフトを破棄**」をクリックします。これにより、復元できない下書きが削除されます。ドラフトの削除について詳しくは、[リクエストドラフトの削除](../../../manage-work/requests/create-requests/delete-request-draft.md)を参照してください。

1. （オプション）アクションを元に戻してドラフトを保持したい場合は、ページの左下隅にある「**キャンセル**」をクリックします。

1. リクエストの情報を入力したら、以下のいずれかの操作を行います。

   * リクエストを送信する準備ができたら、「**送信**」をクリックします。リクエストが「送信済み」セクションに保存されます。リクエストキューのルーティングルールに応じて、このリクエストはリクエストキューとして指定されたリクエストとは異なるプロジェクトにルーティングされる場合があります。ルーティングルールについて詳しくは、[ルーティングルールの作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)を参照してください。

     または

     送信する準備がまだ整っておらず、後で戻って完了する場合は、「**閉じる**」をクリックします。リクエストは「ドラフト」セクションに保存され、次回このリクエストキューのリクエストを送信する際に利用できます。

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     リクエストを送信すると、ドラフトは削除され、復元できません。

   >[!NOTE]
   >
   >* <span class="preview"> 新しいリクエスト用エクスペリエンスでは、ドラフトは送信されたリクエストと同じリストにあります。</span>
   ><span class="preview"> 新しいエクスペリエンスでのリクエストの作成について詳しくは、[&#x200B; リクエストの作成と送信 &#x200B;](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md#create-requests-and-generate-drafts-in-the-workfront-web-app) の記事「Workfront Web アプリでのリクエストの作成とドラフトの生成」を参照してください。</span>

