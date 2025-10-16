---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 個人用プルーフのデフォルトを設定する
description: 作成するすべての新規プルーフに適用される個別のプルーフデフォルト設定を指定できます。これらのデフォルトは、Workfront で初回のプルーフを生成するか新しいプルーフバージョンをアップロードするたびに適用されます。
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 96%

---

# 個人用プルーフのデフォルトを設定する

作成するすべての新規プルーフに適用される個別のプルーフデフォルト設定を指定できます。これらのデフォルトは、Workfront で初回のプルーフを生成するか新しいプルーフバージョンをアップロードするたびに適用されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
    <p>作業またはプラン</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 個人用プルーフのデフォルトを設定する

{{step1-to-proofing}}

1. 右上隅で、自分のアバターをクリックし、「**個人設定**」を選択します。
1. 「**プルーフの既定値** 」タブを選択して、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>デフォルトのメール通知設定</strong> </td> 
     </tr> 
     <tr> 
      <td>デフォルトのメールアラート</td> 
      <td>ユーザーがメールの更新を受け取る頻度を選択します。すべてのアクティビティ、自分のコメントに返信、決定、最終決定、時間別概要、日別概要、無効のいずれかを選択します。</td> 
     </tr> 
     <tr> 
      <td>新規ゲストレビュアー向けのデフォルトのメールアラート</td> 
      <td>ゲストレビュアーがメールの更新を受け取る頻度を選択します。オプションは、デフォルトのメールアラートのオプションと同じです。</td> 
     </tr> 
     <tr> 
      <td>新規プルーフ通知</td> 
      <td>プルーフに追加されたときに通知を受け取ることを選択します。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>メッセージ設定</strong> </td> 
     </tr> 
     <tr> 
      <td>プルーフ件名テンプレート</td> 
      <td>プルーフを共有する際に、メールの件名に表示する内容を入力します。</td> 
     </tr> 
     <tr> 
      <td>プルーフメッセージテンプレート</td> 
      <td>プルーフを共有する際に、メールの本文に表示する内容を入力します。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>デフォルトのプルーフ設定</strong> </td> 
     </tr> 
     <tr> 
      <td>すべての決定が完了したらプルーフをロック</td> 
      <td>すべての決定がおこなわれた後に、それ以降の変更から自動的にプルーフをロックするように選択します。</td> 
     </tr> 
     <tr> 
      <td>1 つの決定のみが必要</td> 
      <td>プルーフに対して 1 つの決定のみを必要とするように選択します。</td> 
     </tr> 
     <tr> 
      <td>ログインは必須です</td> 
      <td> <p>Workfront Proof ログイン資格情報を持つユーザーのみがプルーフを使用できるようにします。</p> <p>メモ：Workfront Proof 資格情報は、会社が SSO を使用していない限り、Workfront 資格情報とは異なる場合があります。この機能は、会社が SSO を使用している場合にのみ使用することをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td>登録が有効</td> 
      <td>組織外のレビュアーがパブリック URL または埋め込みコードを介してプルーフに新規登録できるようにします。このオプションを選択した場合、「プルーフにアクセスするには、サブスクライバーがメール内のリンクをクリックする必要があります」も利用できます。外部のレビュアーがメール内のリンクをクリックしてプルーフにアクセスするように求める場合に、このオプションを選択します。「パブリック共有」オプションが選択されてこのユーザーが作成するすべてのプルーフに適用されている場合、このオプションはデフォルトで有効になります。 </td> 
     </tr> 
     <tr> 
      <td>新規ゲストレビュアー向けのデフォルトの役割</td> 
      <td>新規ゲストレビュアー向けのデフォルトのプルーフの役割を選択します。オプションは、デフォルトのプルーフの役割のオプションと同じです。</td> 
     </tr> 
     <tr> 
      <td>元のファイルのダウンロードのブロック</td> 
      <td>元のファイルのダウンロードを許可しない場合に選択します。 </td> 
     </tr> 
     <tr> 
      <td>デフォルトのプルーフの役割</td> 
      <td>デフォルトのプルーフの役割を選択します。 </td> 
     </tr> 
     <tr> 
      <td>デフォルトのマークアップカラー</td> 
      <td>デフォルトのマークアップ色を選択します。 </td> 
     </tr> 
    </tbody> 
   </table>
