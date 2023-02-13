---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 配達確認の設定を編集
description: 配達確認の作成後は、いつでも配達確認の設定を編集できます。
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# 配達確認の設定を編集

配達確認の作成後は、いつでも配達確認の設定を編集できます。

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
   <td role="rowheader">配達確認の役割</td> 
   <td>作成者またはモデレーター</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## 配達確認の設定を編集

一部の設定は、Workfront管理者がアカウントレベルで無効にした場合、ロックされる場合があります。

1. 配達確認を行うプロジェクト、タスクまたは問題報告に移動し、 **ドキュメント** タブをクリックします。
1. 配達確認の上にマウスを移動して、「 **ドキュメントの詳細**.
1. 左側のパネルで、 **校正ビューアの設定**.
1. 以下の設定を調整します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ログインが必要です。このプルーフはゲストユーザーと共有できません</td> 
      <td> <p>レビューおよび承認プロセスに対してより高いレベルのセキュリティが必要な場合は、配達確認へのログインを使用できます。 つまり、配達確認に追加できるのはWorkfrontユーザーのみです。 アクセスする前に、電子メールとパスワードを入力する必要があります。</p> <p>注意： <em style="font-style: normal;">「ログインが必要」が有効になっている場合、「購読」を有効にすることはできません。</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">電子署名するには決定が必要です</td> 
      <td> <p>配達確認を決定するレビュー担当者の電子署名を必要とする場合があります。 レビュー担当者が決定を下すと、電子メールとパスワードの入力と確定を求めるプロンプトが表示されます。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての必要な決定がおこなわれたら配達確認をロックする</td> 
      <td> <p>最終承認者が決定を下すタイミングをロックする配達確認の状態を設定できます。 これは、レビュー担当者が配達確認に戻ってコメントを追加したり、決定を変更したりできないようにする場合に役立ちます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">オリジナル ファイルのダウンロードを許可する</td> 
      <td> <p>配達確認のレビュー担当者が、配達確認の作成元のファイルをダウンロードすることを許可できます。 これはデフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコード経由によるプルーフの共有を許可する</td> 
      <td>ユーザーが公開 URL や埋め込みコードと配達確認を共有できるようにします。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコード経由によるプルーフの登録を許可する</td> 
      <td> <p>配達確認の購読を有効にすると、配達確認に明示的に追加されていないユーザーが自分自身を配達確認に登録できます（つまり、配達確認に自分を追加します）。 その後、配信登録設定で選択した役割と電子メールのアラートが割り当てられます。</p> <p>配達確認で「購読」が有効になっている場合、以下のフィールドがアクティブになります。</p> 
       <ul> 
        <li><strong>購読者の検証が必要です</strong>  — 配達確認にアクセスするには、購読者が E メール内のリンクをクリックする必要があります<br>このオプションを選択すると、購読しているユーザーは配達確認にすぐにアクセスできなくなり、E メールで配達確認へのリンクが取得されます。 購読者の検証の目的は、アクセス権のある正しい電子メールアドレスがユーザーに入力されたことを確認することです。</li> 
        <li><strong>新規購読者のデフォルトの役割 —</strong> これは、配達確認を購読するすべてのレビュー担当者に割り当てられる、デフォルトの配達確認の役割です。</li> 
        <li><strong>新規購読者向けのデフォルトの電子メールアラート</strong>  — これは、配達確認を自分で購読するすべてのレビュー担当者に割り当てられるデフォルトの E メールアラートです。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

 
