---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Web サイトまたはその他の web コンテンツ用のインタラクティブなプルーフを作成する
description: 新しいインタラクティブなプルーフを生成するか、web コンテンツ用の既存のインタラクティブのプルーフの新しいバージョンを生成できます。これには、web サイト、ストリーミングビデオやオーディオを含む広告、HTML アニメーション、インタラクティブバナーなどの他の種類のインタラクティブコンテンツが含まれます。
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 35d76d3cb06c9e9b449844f304f1443e24a221d4
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 95%

---

# Web サイトまたはその他の web コンテンツ用のインタラクティブなプルーフを作成する

新しいインタラクティブなプルーフを生成するか、web コンテンツ用の既存のインタラクティブのプルーフの新しいバージョンを生成できます。これには、web サイト、ストリーミングビデオやオーディオを含む広告、HTML アニメーション、インタラクティブバナーなどの他の種類のインタラクティブコンテンツが含まれます。

インタラクティブなプルーフでは、レビュー担当者は、web サイトや他の web コンテンツを、通常通りにナビゲートおよび操作できます。

>[!IMPORTANT]
>
>レビュー担当者は、web サイトまたはインタラクティブコンテンツにアクセスできることを確認してください。インターネット上でもアクセスできる場合に限り、プルーフプロセスでアクセスできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## Web サイトまたはその他の web コンテンツ用のインタラクティブなプルーフを作成する

1. 新しい web サイトのプルーフまたは既存の web サイトの新しいバージョンを作成するプロジェクト、タスクまたはイシューに移動します。
1. 左側のパネルで「**ドキュメント**」をクリックします。
1. （条件付き）新しいプルーフを作成する場合は、「**新規追加**」をクリックし、表示されるメニューで「**プルーフ**」をクリックします。

1. （条件付き）既存プルーフの新しいバージョンを作成する場合、**新規プルーフ**&#x200B;ページが表示されます。

   1. 新しいバージョンを作成する URL プルーフの上にポインタを合わせて、そのバージョンを囲む薄い青色の背景をクリックして選択します。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. **新規追加**&#x200B;ドロップダウンで、**バージョン**／**プルーフ**&#x200B;をクリックします。

1. Adobe Analytics の **ファイルを追加** 「 」セクションで、配達確認する Web サイトの URL を入力し、 **入力**.  このプロセスを繰り返して、プルーフする複数の web サイトを追加できます。

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > URL は 1,000 文字未満にする必要があります。

1. 追加した URL をクリックします。

   ![](assets/click-url-350x137.png)

1. （オプション）Web サイトの URL から別の名前にプルーフの名前を変更する場合は、「**プルーフ名**」を入力します。
1. 「**インタラクティブ**」を選択し、「**完了**」をクリックします。

   >[!NOTE]
   >
   >既存の URL プルーフに新しいバージョンを追加する場合、元のプルーフまたは以前のバージョンに設定されたオプションは、このバージョンでも維持されます。

1. 「**プルーフを作成**」をクリックして、レビュープロセスを行わずにシンプルなプルーフを作成します。\
   または\
   高度なプルーフの設定を続行します。

   * [基本ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
