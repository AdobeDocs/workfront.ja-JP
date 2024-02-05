---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: プルーフビューアーでのインタラクティブなプルーフの解像度の変更
description: 様々なデバイスでのインタラクティブなプルーフの外観をプレビューし、様々な解像度に基づいてコンテンツが表示され、応答する様子を確認できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: d4fa663e22daf25fec77be79a452eb207857bdda
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 94%

---

# プルーフビューアーでのインタラクティブなプルーフの解像度の変更

様々なデバイスでのインタラクティブなプルーフの外観をプレビューし、様々な解像度に基づいてコンテンツが表示され、応答する様子を確認できます。

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
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## デスクトッププルーフビューアーと web プルーフビューアーのデバイスと解像度の表示

Adobe Workfront 管理者は、インタラクティブなコンテンツをデスクトッププルーフビューアーで確認するか、ZIP ファイルにバンドルされたコンテンツとして web プルーフビューアーで確認できるようにシステムを設定しています。

* デスクトッププルーフビューアーでは、様々な解像度やデバイスでのコンテンツの表示と応答を確認できます。レビュアーが特定のデバイスを指定すると、そのデバイス上でのコンテンツの表示と、そのデバイスのユーザーインターフェイス仕様の表示が切り替わります。例えば、あるブランドのスマートフォンの赤いボタンが、別のブランドでは青い場合があります。

* Web プルーフビューアーでは、様々なデバイスの解像度で表示されるインタラクティブコンテンツを表示できます。ただし、web プルーフビューアーでは、ボタンの色など、これらのデバイスのインターフェイス仕様を使用したコンテンツはエミュレートされません。

  >[!NOTE]
  >
  >Workfrontの管理者は、組織内のユーザーのカスタムデバイスを設定できます。詳しくは、 [配達確認用のカスタムデバイスの設定](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) 記事内 [組織の配達確認設定を構成します](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

## プリセットのデバイスまたは解像度設定でプルーフを表示

1. 開くプルーフが含まれているドキュメントリストに移動します。
1. ドキュメントにポインタを合わせて、「**プルーフを開く**」をクリックします。
1. プルーフビューアーの中央下部にある「**レスポンシブ**」をクリックします。

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. デスクトッププルーフビューアーで、表示されるデバイスと解像度のリストから目的のデバイスをクリックします。

   または

   Web プルーフビューアーで、表示される解像度のリストから目的の解像度をクリックします。

   これら 2 つのビューアーの違いについて詳しくは、[web プルーフビューアーとデスクトッププルーフビューアーの違いの概要](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)を参照してください。

   インタラクティブなプルーフは、選択した解像度でレンダリングされます。

## カスタム解像度設定でプルーフを表示

1. 開くプルーフが含まれているドキュメントリストに移動します。
1. ドキュメントにポインタを合わせて、「**プルーフを開く**」をクリックします。
1. プルーフビューアーの中央下部にある「**レスポンシブ**」をクリックします。
1. カスタム&#x200B;**レスポンシブ**&#x200B;解像度を入力します。

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   または

   インタラクティブコンテンツにポインタを合わせて、右下隅の青い境界線（右または下の端）を目的の解像度にドラッグします。

   ![Drag_blue_edges_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   カスタム解像度は、次の場所に表示されます。

   * ビューアーの中央下部にある&#x200B;**解像度**&#x200B;パネル。\
     ![Screenshot_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * レビュアーがプルーフに追加したすべてのコメント。各コメントには、レビュアーがコメントを作成したときに選択した画面の解像度が含まれます。
