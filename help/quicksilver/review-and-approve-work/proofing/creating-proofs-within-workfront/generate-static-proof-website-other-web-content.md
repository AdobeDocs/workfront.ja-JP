---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Web サイトまたはその他の Web コンテンツ用の静的配達確認の作成
description: 新しい静的配達確認を生成するか、Web コンテンツ用の既存の静的配達確認の新しいバージョンを生成できます。 Web コンテンツには、ストリーミングビデオ、HTMLアニメーション、インタラクティブバナーを含む広告などを含めることができますが、静的な校正を行うために、複数のスクリーンショットに切り取られます。
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Web サイトまたはその他の Web コンテンツ用の静的配達確認の作成

新しい静的配達確認を生成するか、Web コンテンツ用の既存の静的配達確認の新しいバージョンを生成できます。 Web コンテンツには、ストリーミングビデオ、HTMLアニメーション、インタラクティブバナーを含む広告などを含めることができますが、静的な校正を行うために、複数のスクリーンショットに切り取られます。

Web サイトまたは他の Web コンテンツ用の静的配達確認を作成する際は、次の点を考慮します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：選択またはプレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャ以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## Web サイトまたはその他の Web コンテンツ用の静的配達確認の作成

静的配達確認を作成するには、Web サイトが（ファイアウォールの内側ではなく）公にアクセス可能である必要があります。または、組織のにWorkfrontドメインが含まれている必要がありま許可リストす。 Workfrontは、パスワードで保護された Web サイトを静的配達確認として取り込むことはできません。

>[!TIP]
>
>認証およびパスワードで保護されたページが必要な内部ページに対しては、静的校正ではなく、インタラクティブ校正をお勧めします。 詳しくは、 [インタラクティブコンテンツの配達確認の概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 新しい Web サイトの配達確認または既存の Web サイトの新しいバージョンを作成するプロジェクト、タスクまたは問題を開きます。
1. クリック **ドキュメント** をクリックします。
1. （条件付き）新しい配達確認を作成する場合は、 **新規追加**&#x200B;を選択し、「 **配達確認** をクリックします。
1. （条件付き）既存の配達確認の新しいバージョンを作成する場合：

   1. 新しいバージョンを作成する URL 配達確認の上にマウスを移動し、そのバージョンを囲む明るい青色の背景をクリックして選択します。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. クリック **新規追加** > **バージョン** > **配達確認**.

1. 配達確認する Web サイトの URL を **ファイルを追加** 領域を選択し、 **入力**.

   URL は、入力したボックスの下に表示されます。

   ![](assets/url-name-appears-below-350x142.png)

1. 追加した URL をクリックします。

   Web サイトの配達確認を設定するためのオプションが表示されます。

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. （オプション）Web サイトの URL から別の URL に配達確認の名前を変更する場合は、 **配達確認の名前。**
1. 確認 **スクリーンショットをキャプチャ** が選択され、次のいずれかのオプションを使用します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>スクリーンショットの解像度</strong> </td> 
      <td> <p>レビュー担当者が配達確認を表示する際にコンテンツの解像度を調整して、電話、タブレット、モニターなど、様々なサイズのデバイスでどのように表示されるかを確認できます。</p> <p>複数の解像度を選択した場合は、選択した解像度ごとに個別の配達確認が作成されます。</p> <p>注意：レビュー担当者が配達確認にコメントすると、コメントに対していつコメントが付けられたかを示す解像度がコメントに含まれ、他のレビュー担当者がコメントに関連付けられた解像度を把握できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>サブページを検索</strong> </td> 
      <td> <p>Web サイトのサブページおよびそのメインページを取り込みます。 「すべて選択」をクリックしてすべてのページを含めるか、含める特定のページのみをクリックします。 プラスボタンとマイナスボタンを使用すると、Web サイトのサブページ領域を拡大または閉じることができます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >作成する配達確認の後続のバージョンに対しては、キャプチャのスクリーンショット設定を変更できません。

1. クリック **完了**.

   手順 8 で複数のスクリーンショット解像度を選択した場合、リストには各解像度のスクリーンショットのセットが含まれます。 これらのスクリーンショットを個別の配達確認として生成したり、1 つの配達確認に組み合わせたりできます（のを参照）。 これらを組み合わせることをお勧めします。特に、静的な Web サイトの配達確認を作成する場合にはお勧めします。

   >[!NOTE]
   >
   >既存の URL 配達確認に新しいバージョンを追加する場合、元の配達確認または以前のバージョンに設定されたオプションは、そのバージョンで維持されます。

1. クリック **配達確認を作成** をクリックして、確認プロセスを行わずに簡単な配達確認を作成します。\
   または\
   詳細な配達確認を設定して続行します。

   * [基本ワークフローを使用した詳細な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
