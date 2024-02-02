---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 組織のプルーフ設定の指定
description: Adobe Workfront 管理者または Workfront プルーフ管理者は、組織のデフォルトのプルーフ設定をカスタマイズできます。これらの設定には、デフォルトの共有オプションやブランディングなどが含まれます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '1265'
ht-degree: 100%

---

# 組織のプルーフ設定の指定

Adobe Workfront 管理者または Workfront プルーフ管理者は、組織のデフォルトのプルーフ設定をカスタマイズできます。これらの設定には、デフォルトの共有オプションやブランディングなどが含まれます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Premium または選択</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プルーフ権限プロファイルで管理者を選択しておく必要があります。詳細については、<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">ユーザーのプルーフアクセスの設定</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## アクションの設定

プルーフビューアーでのアクション使用について詳しくは、[プルーフコメントへのアクションの使用](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)を参照してください。

組織のアクションは、次の方法で設定できます。

* [アクションの追加または名前変更](#add-or-rename-an-action)
* [アクションの非アクティブ化または再アクティブ化](#deactivate-or-reactivate-an-action)
* [アクションの並べ替え](#reorder-actions)

### アクションの追加または名前変更 {#add-or-rename-an-action}

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、プルーフ ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. Workfront Proof の右上隅にある **設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブを選択します。

1. 次のいずれかの操作を行います。

   * 新しいアクションを作成するには、「**アクション**」セクションで「**新規アクション**」をクリックします。

     アカウントで設定できるアクションの数に制限はありません。

   * 既存のアクションの名前を変更するには、アクションの横にある「**設定**」をクリックします。

1. アクションの名前を入力し、「**保存**」をクリックします。
1. 「**保存**」をクリックします。

### アクションの非アクティブ化または再アクティブ化 {#deactivate-or-reactivate-an-action}

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、プルーフ ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. Workfront Proof の右上隅にある **設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブを選択します。

1. 非アクティブ化または再アクティブ化するアクションの横にある「**設定**」をクリックします。
1. 「**アクティブ化**」または「**非アクティブ化**」を選択し、「**保存**」をクリックします。

### アクションの並べ替え {#reorder-actions}

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、プルーフ ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. Workfront Proof の右上隅にある **設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブを選択します。

1. 「**設定**」の横にある青い上向き矢印と下向き矢印をクリックしてアクションを並べ替えます。

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## プルーフ用にカスタムデバイスを設定

カスタムデバイスをシステムに追加すると、ユーザーはインタラクティブコンテンツを確認し、特定のデバイスでコンテンツがどのように表示されるかをシミュレートできます。

インタラクティブなコンテンツをレビューする際にユーザーがデバイスを選択する方法について詳しくは、[プルーフビューアでのインタラクティブなプルーフの解像度の変更](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)を参照してください。

カスタムデバイスを追加するには：

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、「プルーフ」![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. Workfront Proof インターフェイスの右上隅で&#x200B;**設定**／**アカウント設定**&#x200B;をクリックし、「**設定**」タブをクリックします。

1. 「**プルーフ用のカスタムデバイス**」セクションで、「**新規デバイスを追加**」をクリックします。

1. 表示される&#x200B;**新規デバイスを追加**&#x200B;ボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>ユーザーがデスクトッププルーフビューアでデバイスを選択するときに表示される名前です（<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">プルーフビューアでのインタラクティブプルーフの解像度の変更</a>を参照）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">寸法</td> 
      <td>このデバイスで使用する寸法を指定します。デバイス名の下に寸法が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">比率</td> 
      <td>デバイスの比率を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイプ</td> 
      <td>デバイスがモバイル、タブレット、デスクトップのどれであるかを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーエージェント文字列</td> 
      <td>デバイスのユーザーエージェントを入力して、ソフトウェアがデバイスに対して設計どおりに動作し表示されるための情報を提供します。<p>ユーザーエージェントを取得するには、デバイスから <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> にアクセスします。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">無効</td> 
      <td>このオプションが選択されている場合、インタラクティブプルーフのレビュー時にユーザーが選択できるデバイスはありません。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**作成**」をクリックします。

## プルーフのポップアップメッセージの設定

プルーフのポップアップメッセージを設定すると、組織内のすべてのレビュー担当者に一般情報を伝えることができます。

次の状況で表示されるメッセージを設定できます。

* **読み込み時メッセージ**：プルーフが最初に開いたときに表示されます。プルーフをレビューする方法をユーザーに説明したり、免責条項やその他の法的文言を提供するのに役立ちます。
* **決定時メッセージ**：ユーザーがプルーフに関する決定を選択したときに表示されます。ブランドや規制へのコンプライアンスなどのチェックリストをユーザーに提供するのに役立ちます。決定については、[プルーフビューアでのプルーフに関する判断](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を参照してください。

* **確認ボタンのテキスト**：前述の「読み込み時」ポップアップメッセージのボタンに表示されるラベル。

プルーフのポップアップメッセージを作成するには、次の手順に従います。

1. カスタマイズするメッセージの右側にある「**編集**」をクリックします。
1. メッセージを指定し適切な書式を含めて、「**保存**」をクリックします。
1. （オプション）読み込み時メッセージをカスタマイズし、確認ボタンのラベルもカスタマイズする場合は、**確認ボタンのテキスト**&#x200B;の右側にある「**編集**」をクリックし、ラベルを指定して「**保存**」をクリックします。

## プルーフのデフォルトの設定

組織のプルーフのデフォルト設定については、[デフォルトのプルーフの設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)を参照してください。


## 共有のデフォルトの設定

組織のプルーフを共有できる相手、レビュー担当者が使用できるバージョン、特定のステージに関連付けられたユーザーに自動化ワークフローを含んだプルーフが表示されるタイミングを指定できます。

Workfront Proof 内の設定の共有について詳しくは、[ユーザーの共有設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md)を参照してください。

## Workfront Proof サイトのブランディング

Workfront Proof を使用している場合、サイトの以下のエリアにブランディングを設定することができます。

* プルーフが読み込まれたときに表示されるスプラッシュページ
* ログイン画面とログアウト画面
* メール通知

Workfront Proof サイトのブランディング方法について詳しくは、[Workfront Proof サイトのブランディング](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)を参照してください。

## パスワードの詳細設定

>[!IMPORTANT]
>
>このオプションは、従来の Workfront プランでのみ使用できます。Pro、Business、Enterprise Workfront のいずれかのプランを利用している場合は、詳細なパスワード設定を行えなくなりました。

**詳細なパスワード設定**&#x200B;で、ユーザーのパスワードのセキュリティを強化できます。

1. 対象となる設定の右側にある「**設定**」をクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">パスワードの最低文字数</td> 
      <td>Workfront Proof のパスワードの長さはデフォルトで 6 文字です。組織のポリシーに応じて、文字数を増やすことができます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文字種の混在</strong> </td> 
      <td>パスワードに大文字、小文字、数字、記号を混在させて使用するようにユーザーに強制できます。パスワードに含める文字種の数を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>最大繰り返し文字数</strong> </td> 
      <td>各ユーザーのパスワード内で繰り返すことができる文字数を指定できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動パスワード有効期限</td> 
      <td>ユーザーが定期的にパスワードを変更するよう強制します。どのくらいの頻度で変更するかを決めます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>許可されないパスワードの繰り返し回数</strong> </td> 
      <td>アカウントで許可されないパスワードの繰り返し回数を設定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プロファイルのロックアウト</strong> </td> 
      <td>指定したログイン試行回数に失敗した場合、そのユーザーをアカウントからロックアウトします。アカウントに再びアクセスできるようになるまでの待ち時間も指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">30 日経ってもパスワードがリセットされなかったユーザーをロック</td> 
      <td>ユーザーがプロファイルの有効化から 30 日以内に初期パスワードを変更しない場合、ユーザーはアカウントからロックアウトされます。<br><p>アカウント管理者は、システムによって自動的にロックされたユーザーのロックを解除（再アクティブ化）できます。パスワードの変更には、さらに 7日間の期間が必要となります。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">120 日間非アクティブの場合にユーザーアカウントをロック</td> 
      <td>ユーザーが Workfront Proof またはログインが必要なプルーフに 120 日間ログインしなかった場合、ユーザーはアカウントからロックアウトされます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>初回ログイン後にパスワードを変更</strong> </td> 
      <td>初回ログイン後、ユーザーに一時パスワードの変更を促します。<p>アカウント管理者は、システムによって自動的にロックアウトされたユーザーのロックを解除（再アクティブ化）できます。</p><p>パスワードの情報について詳しくは、<a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Workfront Proof のログインとパスワードおよびメールアドレスの変更</a>を参照してください。</p></td> 
     </tr> 
    </tbody> 
   </table>
