---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Web サイトまたはその他の Web コンテンツ用のインタラクティブな配達確認の作成
description: 新しいインタラクティブ配達確認を生成するか、Web コンテンツ用の既存のインタラクティブ配達確認の新しいバージョンを生成できます。 これは、Web サイトや、ストリーミングビデオやオーディオを含む広告、HTMLアニメーション、インタラクティブバナーなどの他の種類のインタラクティブコンテンツにすることができます。
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 35d76d3cb06c9e9b449844f304f1443e24a221d4
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Web サイトまたはその他の Web コンテンツ用のインタラクティブな配達確認の作成

新しいインタラクティブ配達確認を生成するか、Web コンテンツ用の既存のインタラクティブ配達確認の新しいバージョンを生成できます。 これは、Web サイトや、ストリーミングビデオやオーディオを含む広告、HTMLアニメーション、インタラクティブバナーなどの他の種類のインタラクティブコンテンツにすることができます。

インタラクティブな配達確認では、レビュー担当者は、Web サイトや他の Web コンテンツと通常通りに移動およびやり取りできます。

>[!IMPORTANT]
>
>レビュー担当者は、Web サイトまたはインタラクティブコンテンツにアクセスできることを確認してください。 インターネット上でもアクセスできる場合に限り、校正プロセスでアクセスできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン： Pro 以上</p> <p>または</p> <p>レガシープラン：Premium</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業またはプラン</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャ以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## Web サイトまたはその他の Web コンテンツ用のインタラクティブな配達確認の作成

1. 新しい Web サイトの配達確認または既存の Web サイトの新しいバージョンを作成するプロジェクト、タスクまたは問題を開きます。
1. クリック **ドキュメント** をクリックします。
1. （条件付き）新しい配達確認を作成する場合は、 **新規追加**&#x200B;を選択し、次に **配達確認** をクリックします。

1. （条件付き） **新しい配達確認** ページが表示されます（既存の配達確認の新しいバージョンを作成する場合）。

   1. 新しいバージョンを作成する URL 配達確認の上にマウスポインターを置き、そのバージョンを囲む明るい青色の背景をクリックして選択します。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. Adobe Analytics の **新規追加** ドロップダウンで、 **バージョン** > **配達確認**.

1. Adobe Analytics の **ファイルを追加** 「 」セクションで、配達確認する Web サイトの URL を入力し、 **入力**.  このプロセスを繰り返して、配達確認を受ける複数の Web サイトを追加できます。

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > URL は 1,000 文字未満にする必要があります。

1. 追加した URL をクリックします。

   ![](assets/click-url-350x137.png)

1. （オプション）Web サイトの URL から別の名前に配達確認の名前を変更する場合は、 **配達確認名**.
1. 選択 **インタラクティブ**&#x200B;を選択し、次に **完了**.

   >[!NOTE]
   >
   >既存の URL 配達確認に新しいバージョンを追加する場合、元の配達確認または以前のバージョンに設定されたオプションは、このバージョンでも維持されます。

1. クリック **配達確認を作成** をクリックして、確認プロセスを行わずに簡単な配達確認を作成します。\
   または\
   詳細な配達確認を設定して続行します。

   * [基本ワークフローを使用した詳細な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
