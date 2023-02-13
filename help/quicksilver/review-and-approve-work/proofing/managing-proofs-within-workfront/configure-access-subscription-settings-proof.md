---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: 配達確認のアクセスおよび購読設定を構成する
description: ユーザーにログインを要求するかどうか、ユーザーに配達確認の購読を許可するかどうかなど、個々の配達確認に対する特定のアクセス設定や購読設定を指定できます。 配達確認の作成時に、配達確認のアクセス設定と購読設定を設定することも、Workfrontに既に存在する配達確認の設定を行うこともできます。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 3%

---

# 配達確認のアクセスおよび購読設定を構成する

ユーザーにログインを要求するかどうか、ユーザーに配達確認の購読を許可するかどうかなど、個々の配達確認に対する特定のアクセス設定や購読設定を指定できます。 配達確認の作成時に、配達確認のアクセス設定と購読設定を設定することも、Workfrontに既に存在する配達確認の設定を行うこともできます。

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

## 配達確認の作成時にアクセスと購読を設定する

配達確認の作成時に、配達確認のアクセス設定と購読設定を設定するには、次の手順を実行します。

1. 配達確認を行うプロジェクト、タスクまたは問題報告に移動し、 **ドキュメント** 」セクションに入力します。
1. クリック **新規追加** を右上の領域に追加します。
1. スクロールして **配達確認の設定** の右下隅のセクション **新しい配達確認** ページ。

1. 次の設定を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの共有を許可する</strong> </td> 
      <td>このオプションを選択した場合、配達確認はパブリック URL または埋め込みコード経由で共有できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの登録を許可する</strong> </td> 
      <td>このオプションを選択すると、配達確認に明示的に追加されていないユーザーも配達確認を購読できます。 配達確認を購読しているユーザーには、次の設定で定義した役割と E メールが付与されます。
       <ul>
        <li><p><strong>購読者の役割：</strong> 配達確認を購読するすべてのレビュー担当者に割り当てられる、デフォルトの配達確認の役割です。 </p><p>重要：If <strong>との共有を許可</strong> が次の値以外に設定されている場合は、 <strong>全員</strong> Workfrontの配達確認設定では、この購読は組織内のユーザーに対してのみ機能します。 詳しくは、 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof での配達確認の設定</a>.</p></li>
        <li><strong>購読者向けの E メールアラート設定：</strong> 配達確認を購読するすべてのレビュー担当者に割り当てられるデフォルトの E メールアラートです。</li>
       </ul><p>
        <ul>
         <li><strong>次の項目に必要な電子メールリンクを介した配達確認へのアクセス</strong> 配達確認へのリンクを含む E メールを購読者が受信するかどうかを設定します。 次を選択できます。 <strong>メールなし</strong> （配達確認にアクセスするには、E メールリンクは必要ありません）。 <strong>配達確認通知 E メールのみ</strong> （購読者が、確認なしで E メールで配達確認へのリンクを受け取る）、または <strong>検証および配達確認の通知 E メール</strong> （購読者は、E メールで配達確認へのリンクを受け取り、リンクをクリックして配達確認にアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しい E メールアドレスを入力したことを確認することです）。</li>
        </ul><p>注意： 配達確認に自動ワークフローが添付されている場合、すべての購読が配達確認の所有者に確認 E メールを生成するので、配達確認の対象となる人物を追加するステージを決定できます。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 引き続き配達確認を作成します。

## 既存の配達確認のアクセス設定と購読設定を構成する

Workfrontに既に存在する配達確認のアクセスおよび購読設定を設定するには：

1. 「ドキュメント」領域で、設定を行う配達確認を含むドキュメントを選択し、 **ドキュメントの詳細**.
1. 左側のパネルで、 **校正ビューアの設定**.
1. 次の設定を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>公開 URL または埋め込みコードを使用した配達確認の共有を許可</strong><strong>e</strong> </td> 
      <td>このオプションを選択した場合、配達確認はパブリック URL または埋め込みコード経由で共有できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの登録を許可する</strong> </td> 
      <td>このオプションを選択すると、配達確認に明示的に追加されていないユーザーも配達確認を購読できます。 配達確認を購読しているユーザーには、次の設定で定義した役割と E メールが付与されます。
       <ul>
        <li><p><strong>購読者の役割：</strong> 配達確認を購読するすべてのレビュー担当者に割り当てられる、デフォルトの配達確認の役割です。 </p><p>重要：If <strong>との共有を許可</strong> が次の値以外に設定されている場合は、 <strong>全員</strong> Workfrontの配達確認設定では、この購読は組織内のユーザーに対してのみ機能します。 詳しくは、 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof での配達確認の設定</a>.</p></li>
        <li><strong>購読者向けの E メールアラート設定：</strong> 配達確認を購読するすべてのレビュー担当者に割り当てられるデフォルトの E メールアラートです。</li>
       </ul><p>
        <ul>
         <li><strong>次の項目に必要な電子メールリンクを介した配達確認へのアクセス</strong> 配達確認へのリンクを含む E メールを購読者が受信するかどうかを設定します。 次を選択できます。 <strong>メールなし</strong> （配達確認にアクセスするには、E メールリンクは必要ありません）。 <strong>配達確認通知 E メールのみ</strong> （購読者が、確認なしで E メールで配達確認へのリンクを受け取る）、または <strong>検証および配達確認の通知 E メール</strong> （購読者は、E メールで配達確認へのリンクを受け取り、リンクをクリックして配達確認にアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しい E メールアドレスを入力したことを確認することです）。</li>
        </ul><p>注意： 配達確認に自動ワークフローが添付されている場合、すべての購読が配達確認の所有者に確認 E メールを生成するので、配達確認の対象となる人物を追加するステージを決定できます。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
