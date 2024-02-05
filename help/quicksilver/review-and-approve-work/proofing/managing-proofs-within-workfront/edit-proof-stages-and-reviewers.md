---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: プルーフのステージとレビュアーを編集
description: 配達確認のステージとレビュー担当者の編集方法を説明します。
author: Courtney
feature: Digital Content and Documents
exl-id: 91549c2d-d7b1-461c-a3c4-ad0032acfb23
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 98%

---

# プルーフのステージとレビュアーを編集

プルーフの所有者または作成者である場合や、正しいプルーフの役割が割り当てられている場合は、プルーフのステージとレビュアーの詳細を編集できます。

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
   <td role="rowheader">プルーフの役割</td> 
   <td>作成者またはモデレーター </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## ステージを編集

1. ドキュメントを含むドキュメントリストで、ドキュメントを含む行の上にポインタを合わせて、「**プルーフワークフロー**」をクリックします。

   または

   スタンドアロンの Workfront プルーフで、プルーフの右の&#x200B;**その他**（3 つの点）メニューをクリックし、**プルーフの詳細を表示**&#x200B;をクリックします。

1. 「**ワークフロー**」セクションの次のいずれかを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期日を編集</td> 
      <td> <p>日付を選択し、表示されるカレンダーで新しい日付を選択します。期日を完全に削除するには、表示されるカレンダーの下の<strong>クリア</strong>を選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">個々のレビュアーを削除</td> 
      <td> <p>レビュアーの名前の右側にある<strong>その他</strong>メニューを選択し、ドロップダウンメニューで<strong>削除</strong>をクリックします。表示されるボックスで<strong>確認</strong>をクリックし、プルーフからレビュアーを削除します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複数のレビュアーを削除</td> 
      <td>名前の横にあるチェックボックスをオンにし、「ステージ」セクションの右上隅の<strong>削除</strong>アイコンをクリックします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべてのレビュアーにメッセージを送信</td> 
      <td>「ステージ」セクションの右上隅にある<strong>その他</strong>メニュー、「<strong>全員にメッセージを送信</strong>」の順に選択します。メッセージを設定し、「<strong>送信</strong>」を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージにレビュアーを追加</td> 
      <td>「ステージ」セクションの右上隅にある<strong>その他</strong>メニューで、「<strong>共有</strong>」を選択します。ユーザーを追加し、そのユーザーの役割とメールアラートを設定し、必要に応じて繰り返します。終了したら、「<strong>共有</strong>」をクリックします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージの削除</td> 
      <td> <p>「ステージ」セクションの右上隅にある<strong>その他</strong>メニューを選択してから、ステージの<strong>削除</strong>を選択します。</p> <p>メモ：ステージが 1 つだけの場合、ステージは削除できません。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## レビュアーの詳細を編集

1. Workfront で、プルーフにポインタを合わせて、**プルーフの詳細**&#x200B;をクリックし、プルーフの詳細ページを開きます。
1. 「**ワークフロー**」セクションで、レビュアーの名前の右側にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-button-small.png) をクリックし、表示されるドロップダウンメニューの「**編集**」をクリックします。

1. 表示される&#x200B;**レビュアーを編集**&#x200B;ボックスで、次の詳細を編集します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">表示名*</td> 
      <td> <p>プルーフのレビュアーの表示名を変更するには、テキストフィールドをクリックし、インラインで名前を編集します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">役割</td> 
      <td>プルーフに対するレビュアーの役割を変更するには、ドロップダウンメニューを開き、目的の役割を選択します。詳細情報を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">メールアラート</td> 
      <td>プルーフに対するレビュアーのメールアラートを変更するには、ドロップダウンメニューを開き、目的のメールアラートを選択します。詳しくは、記事内の<a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">プルーフのコメントおよび決定の通知の概要</a>を参照してください。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">決定*</td> 
      <td> <p>プルーフに対するレビュアーの決定を変更するには、ドロップダウンメニューを開き、目的の決定を選択します。別のユーザーに代わって行った決定は、プルーフの「アクティビティ」セクションに記載されます。このオプションは、レビューが決定した場合にのみ表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージ</td> 
      <td>レビュアーをステージ間で移動することはできません。ただし、期限が異なるレビュアーを削除して、再度追加することはできます。</td> 
     </tr> 
    </tbody> 
   </table>

   &#42;このフィールドを編集するには、プルーフの作成者または所有者である必要があります。

1. 「**保存**」をクリックします。
