---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 個人用校正のデフォルトを設定
description: 作成する配達確認に適用される個人用配達確認のデフォルト設定を定義できます。 これらのデフォルトは、Workfrontで初回の配達確認を生成するか新しい配達確認バージョンをアップロードするたびに適用されます。
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 個人用校正のデフォルトを設定

作成する配達確認に適用される個人用配達確認のデフォルト設定を定義できます。 これらのデフォルトは、Workfrontで初回の配達確認を生成するか新しい配達確認バージョンをアップロードするたびに適用されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：選択またはそれ以上</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャ以降</td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## 個人用校正のデフォルトを設定

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **校正**.

1. 右上隅で、自分のアバターをクリックし、「 」を選択します。 **個人設定**.
1. を選択します。 **校正の既定値** 」タブで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>デフォルトの電子メール通知設定</strong> </td> 
     </tr> 
     <tr> 
      <td>デフォルトのメールアラート</td> 
      <td>ユーザーが電子メールの更新を受け取る頻度を選択します。 「すべてのアクティビティ」、「自分のコメントに返信」、「決定」、「最終決定」、「時間別の概要」、「日別の概要」または「無効」を選択します。</td> 
     </tr> 
     <tr> 
      <td>新しいゲストレビュー担当者向けのデフォルトの電子メールアラート</td> 
      <td>ゲストレビュー担当者が電子メールの更新を受け取る頻度を選択します。 オプションは、デフォルトの電子メールアラートのオプションと同じです。</td> 
     </tr> 
     <tr> 
      <td>新しい配達確認通知</td> 
      <td>配達確認に追加されたときに通知を受け取ることを選択します。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>メッセージ設定</strong> </td> 
     </tr> 
     <tr> 
      <td>配達確認の件名テンプレート</td> 
      <td>配達確認を共有する際に、電子メールの件名に表示する内容を入力します。</td> 
     </tr> 
     <tr> 
      <td>配達確認メッセージテンプレート</td> 
      <td>配達確認を共有する際に、ユーザーに電子メールの本文に表示する内容を入力します。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>デフォルトの配達確認設定</strong> </td> 
     </tr> 
     <tr> 
      <td>すべての決定がおこなわれたときに配達確認をロックする</td> 
      <td>すべての決定がおこなわれた後に、それ以降の変更から配達確認を自動的にロックするように選択します。</td> 
     </tr> 
     <tr> 
      <td>1 つの決定のみが必要</td> 
      <td>配達確認に対して 1 つの決定のみを必要とするように選択します。</td> 
     </tr> 
     <tr> 
      <td>ログインが必要です</td> 
      <td> <p>Workfront Proof ログイン資格情報を持つユーザーのみが配達確認を使用できるようにします。</p> <p>注意：Workfrontの配達確認資格情報は、会社のユーザーが SSO でない限り、Workfrontの資格情報とは異なる場合があります。 この機能は、会社のユーザーが SSO を使用する場合にのみ使用することをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td>配信登録有効</td> 
      <td>組織外のレビュー担当者が公開 URL で配達確認にサインアップしたり、コードを埋め込んだりすることを許可します。 このオプションを選択した場合、配達確認にアクセスするには、購読者が E メール内のリンクをクリックする必要があります。 外部のレビュー担当者が E メール内のリンクをクリックして配達確認にアクセスするように求める場合に選択します。 このオプションは、「公開共有」オプションが選択され、このユーザーが作成するすべての配達確認に適用される場合、デフォルトで有効になります。 </td> 
     </tr> 
     <tr> 
      <td>新しいゲストレビュー担当者のデフォルトの役割</td> 
      <td>ゲストレビュー担当者用のデフォルトの配達確認の役割を選択します。 オプションは、「デフォルトの配達確認」の役割のオプションと同じです。</td> 
     </tr> 
     <tr> 
      <td>元のファイルのダウンロードをブロック</td> 
      <td>元のファイルのダウンロードを禁止する場合に選択します。 </td> 
     </tr> 
     <tr> 
      <td>デフォルトの配達確認の役割</td> 
      <td>デフォルトの配達確認の役割を選択します。 </td> 
     </tr> 
     <tr> 
      <td>既定のマークアップカラー</td> 
      <td>既定のマークアップ色を選択します。 </td> 
     </tr> 
    </tbody> 
   </table>
