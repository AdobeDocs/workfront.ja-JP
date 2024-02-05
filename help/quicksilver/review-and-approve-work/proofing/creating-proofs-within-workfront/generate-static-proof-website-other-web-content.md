---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Web サイトまたはその他の web コンテンツ用の静的プルーフの作成
description: 新しい静的プルーフを生成するか、web コンテンツ用の既存の静的プルーフの新しいバージョンを生成できます。Web コンテンツには、ストリーミングビデオ、HTML アニメーション、インタラクティブバナーを含む広告などを含めることができますが、静的なプルーフを行うために、複数のスクリーンショットに切り取られます。
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 35d76d3cb06c9e9b449844f304f1443e24a221d4
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 98%

---

# Web サイトまたはその他の web コンテンツ用の静的プルーフの作成

新しい静的プルーフを生成するか、web コンテンツ用の既存の静的プルーフの新しいバージョンを生成できます。Web コンテンツには、ストリーミングビデオ、HTML アニメーション、インタラクティブバナーを含む広告などを含めることができますが、静的なプルーフを行うために、複数のスクリーンショットに切り取られます。

Web サイトまたは他の web コンテンツ用の静的プルーフを作成する際は、次の点を考慮します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Select または Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
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

## Web サイトまたはその他の web コンテンツ用の静的プルーフの作成

静的プルーフを作成するには、web サイトがパブリックにアクセスできる（ファイアウォールの内側ではない）か、組織の許可リストに Workfront ドメインが含まれている必要があります。Workfront は、パスワードで保護された web サイトを静的プルーフとして取り込むことはできません。

>[!TIP]
>
>認証およびパスワードで保護されたページが必要な内部ページに対しては、静的プルーフではなく、インタラクティブプルーフをお勧めします。詳しくは、[インタラクティブコンテンツのプルーフの概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)を参照してください。

1. 新しい web サイトのプルーフまたは既存の web サイトの新しいバージョンを作成するプロジェクト、タスクまたはイシューに移動します。
1. 左側のパネルで「**ドキュメント**」をクリックします。
1. （条件付き）新しいプルーフを作成する場合は、「**新規追加**」をクリックし、表示されるメニューで「**プルーフ**」をクリックします。
1. （条件付き）既存プルーフの新しいバージョンを作成する場合：

   1. 新しいバージョンを作成する URL プルーフにポインタを合わせて、そのバージョンを囲む水色の背景をクリックして選択します。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. **新規追加**／**バージョン**／**プルーフ**&#x200B;をクリックします。

1. **ファイルを追加**&#x200B;領域にプルーフする web サイトのURLを入力し、**Enter** を押します。

   >[!NOTE]
   >
   > URL は 1,000 文字未満にする必要があります。

1. 追加した URL をクリックします。

   Web サイトのプルーフ設定用オプションが表示されます。

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. （オプション）Web サイトの URL から別の名前にプルーフの名前を変更する場合は、「**プルーフ名**」を入力します。
1. 「**スクリーンショットをキャプチャ**」を選択し、次のいずれかのオプションを使用するようにしてください。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>スクリーンショットの解像度</strong> </td> 
      <td> <p>レビュアーがプルーフを表示する際にコンテンツの解像度を調整して、電話、タブレット、モニターなど、様々なサイズのデバイスでどのように表示されるかを確認できます。</p> <p>複数の解像度を選択した場合は、選択した解像度ごとに別々のプルーフが作成されます。</p> <p>メモ：レビュアーがプルーフにコメントする場合、コメントにはコメントが作成された日時を示す解像度が含まれ、他のレビュアーがコメントに関連付けられた解像度を把握できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>サブページを検索</strong> </td> 
      <td> <p>Web サイトのサブページおよびそのメインページを取り込みます。「すべて選択」をクリックしてすべてのページを含めるか、含める特定のページのみをクリックします。プラスボタンとマイナスボタンを使用すると、Web サイトのサブページ領域を拡大または閉じることができます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >作成するプルーフの後続のバージョンに対しては、キャプチャのスクリーンショット設定を変更できません。

1. 「**完了**」をクリックします。

   手順 8 で複数のスクリーンショット解像度を選択した場合、リストには各解像度のスクリーンショットのセットが含まれます。これらのスクリーンショットを個別のプルーフとして生成したり、1 つのプルーフに組み合わせたりすることができます（参照）。特に、静的な web サイトプルーフを作成しているときには、これらを組み合わせることをお勧めします。

   >[!NOTE]
   >
   >既存の URL プルーフに新しいバージョンを追加する場合、元のプルーフまたは以前のバージョンに設定されたオプションは、このバージョンでも維持されます。

1. 「**プルーフを作成**」をクリックして、レビュープロセスを行わずにシンプルなプルーフを作成します。\
   または\
   高度なプルーフの設定を続行します。

   * [基本ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [自動ワークフローを使用した高度なプルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
