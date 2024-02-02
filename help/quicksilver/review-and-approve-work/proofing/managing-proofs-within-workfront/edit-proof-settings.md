---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: プルーフの設定を編集
description: プルーフの作成後は、いつでもプルーフの設定を編集できます。
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '622'
ht-degree: 100%

---

# プルーフの設定を編集

プルーフの作成後は、いつでもプルーフの設定を編集できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
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
   <td>作成者またはモデレーター</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## プルーフの設定を編集

一部の設定は、Workfront 管理者がアカウントレベルで無効にした場合、ロックされる場合があります。

1. プルーフが必要なプロジェクト、タスク、またはイシューに移動し、「**ドキュメント**」タブをクリックします。
1. プルーフの上にマウスを移動して、「**ドキュメントの詳細**」をクリックします。
1. 左側のパネルで、「**プルーフビューアーの設定**」をクリックします。
1. 以下の設定を調整します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ログインが必要です。このプルーフはゲストユーザーと共有できません</td> 
      <td> <p>レビューおよび承認プロセスに対してより高いレベルのセキュリティが必要な場合は、プルーフへのログインを必須にすることができます。つまり、プルーフに追加できるのは Workfront ユーザーのみです。アクセスする前に、メールアドレスとパスワードを入力する必要があります。</p> <p>メモ：<em style="font-style: normal;">「ログインが必要」が有効になっている場合、登録を有効にすることはできません。</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">電子サインするには決定が必要です</td> 
      <td> <p>プルーフを決定するレビュアーの電子サインを要求できます。レビュアーが決定すると、メールアドレスとパスワードの入力および決定の確認を求めるプロンプトが表示されます。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての必要な決定が行われた時点でプルーフをロックする</td> 
      <td> <p>最終承認者が決定したときに、プルーフの状態をロックするように設定できます。これは、レビュアーがプルーフに戻ってコメントを追加したり、決定を変更したりできないようにしたい場合に役立ちます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">オリジナル ファイルのダウンロードを許可する</td> 
      <td> <p>プルーフのレビュアーが、プルーフが作成された元のファイルをダウンロードできるように許可できます。これはデフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコード経由によるプルーフの共有を許可する</td> 
      <td>ユーザーが公開 URL や埋め込みコードとプルーフを共有できるようにします。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パブリック URL または埋め込みコード経由によるプルーフの登録を許可する</td> 
      <td> <p>プルーフの登録を有効にすると、プルーフに明示的に追加されていないユーザーが、自分自身をプルーフに登録できるようになります（つまり、プルーフに自分自身を追加できるようになります）。その後、登録の設定で選択した役割とメールアドレスのアラートが割り当てられます。</p> <p>プルーフで「登録」が有効になっている場合、次のフィールドがアクティブになります。</p> 
       <ul> 
        <li><strong>サブスクライバーの検証が必要です</strong> - プルーフにアクセスするには、サブスクライバーがメール内のリンクをクリックする必要があります<br>このオプションを選択すると、登録しているユーザーはプルーフにすぐにはアクセスできませんが、メールでプルーフへのリンクを取得することになります。サブスクライバー認証の目的は、ユーザーが正しい、アクセス権を持つメールアドレスを入力したと確認することです。</li> 
        <li><strong>新規サブスクライバーのデフォルトの役割 -</strong> これは、プルーフを登録するすべてのレビュアーに割り当てられるデフォルトのプルーフの役割です。</li> 
        <li><strong>新規サブスクライバー向けのデフォルトのメールアラート</strong> - これは、プルーフを自分で登録するすべてのレビュアーに割り当てられるデフォルトのメールアラートです。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

 
