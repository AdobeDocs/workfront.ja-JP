---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 配達確認の自動ワークフローへのステージおよびユーザーの追加
description: 配達確認の所有者の場合は、既存の自動ワークフローにステージを追加できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 45839f8a-31b2-43a3-a9ea-5437df8cc6b4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 4%

---

# 配達確認の自動ワークフローへのステージおよびユーザーの追加

配達確認の所有者の場合は、既存の自動ワークフローにステージを追加できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：プレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
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

## 自動ワークフローへのステージおよびユーザーの追加

1. ドキュメントの一覧で、ドキュメントの上にマウスポインターを置いて、 **校正ワークフロー** 表示されたとき。
1. Adobe Workfrontの右上隅にある **新しいステージ**.
1. 以下を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名前</strong> </td> 
      <td>ステージ名を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期限</strong> </td> 
      <td>期限の日付を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p><strong>ステージを有効化</strong> </p> </td> 
      <td>ステージをアクティブにするタイミングを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期限オプション</strong> </td> 
      <td>デッドラインのトリガー方法を選択</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ステージをロック</strong> </td> 
      <td>ステージをロックするかどうかを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プライマリ決定者</strong> </td> 
      <td>主な意思決定者を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>決定</strong> </td> 
      <td>1 つの決定のみが必要な場合に選択します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プライバシー</strong> </td> 
      <td>ステージがプライベートかどうかを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ユーザーを追加</strong> </td> 
      <td>連絡先名または E メールアドレスを入力し、配達確認の役割を選択して、E メールアラートを設定します。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **ステージを追加**.
1. （オプション）ワークフローに満足するまで、手順 3 と 4 を繰り返します。
1. クリック **完了**.
