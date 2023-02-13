---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 組織の配達確認設定を構成します
description: Adobe Workfront管理者またはWorkfront配達確認管理者は、組織のデフォルトの配達確認設定をカスタマイズできます。 これらの設定には、デフォルトの共有オプションやブランディングなどが含まれます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 0%

---

# 組織の配達確認設定を構成します

Adobe Workfront管理者またはWorkfront配達確認管理者は、組織のデフォルトの配達確認設定をカスタマイズできます。 これらの設定には、デフォルトの共有オプションやブランディングなどが含まれます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：Premium または Select</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>配達確認権限プロファイルで管理者が選択されている必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">ユーザーの校正アクセスを設定する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## アクションの設定

校正ビューアでのアクションの使用について詳しくは、 [配達確認コメントに対するアクションの使用](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

組織のアクションは、次の方法で設定できます。

* [アクションの追加または名前変更](#add-or-rename-an-action)
* [アクションの非アクティブ化または再アクティブ化](#deactivate-or-reactivate-an-action)
* [アクションの並べ替え](#reorder-actions)

### アクションの追加または名前変更 {#add-or-rename-an-action}

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定** 「 Workfront Proof 」インターフェイスの右上隅にある、 **設定** タブをクリックします。

1. 次のいずれかの操作を行います。

   * 新しいアクションを作成するには、 **アクション** セクションで、 **新しいアクション**.

      アカウントで設定できるアクションの数に制限はありません。

   * 既存のアクションの名前を変更するには、 **設定** をクリックします。

1. アクションの名前を入力し、「 **保存**.
1. クリック **保存します。**

### アクションの非アクティブ化または再アクティブ化 {#deactivate-or-reactivate-an-action}

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定** 「 Workfront Proof 」インターフェイスの右上隅にある、 **設定** タブをクリックします。

1. クリック **設定** をクリックします。
1. 選択 **有効化** または **無効化**&#x200B;を選択し、「 **保存**.

### アクションの並べ替え {#reorder-actions}

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定** 「 Workfront Proof 」インターフェイスの右上隅にある、 **設定** タブをクリックします。

1. の横にある青い上向き矢印と下向き矢印をクリックします。 **設定** 」をクリックしてアクションを並べ替えます。

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## 配達確認用のカスタムデバイスの設定

システムに任意のカスタムデバイスを追加して、ユーザーがインタラクティブなコンテンツを確認し、特定のデバイスでのコンテンツの表示をシミュレートできます。

インタラクティブコンテンツをレビューする際にユーザーがデバイスを選択する方法について詳しくは、 [校正ビューアでインタラクティブな配達確認の解像度を変更](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

カスタムデバイスを追加するには：

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. クリック **設定** > **アカウント設定** 「 Workfront Proof 」インターフェイスの右上隅にある、 **設定** タブをクリックします。

1. 内 **配達確認用のカスタムデバイス** セクションで、 **新しいデバイスを追加**.

1. 内 **新しいデバイスを追加** 表示されるボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>ユーザーがデスクトップ校正ビューアでデバイスを選択するときに表示される名前です。詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">校正ビューアでインタラクティブな配達確認の解像度を変更</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimension</td> 
      <td>このデバイスで使用するサイズを指定します。 デバイス名の下にディメンションが表示されます。</td> 
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
      <td>デバイスのユーザーエージェントを入力して、ソフトウェアを実行し、デバイス用に設計された情報を表示します。<p>ユーザーエージェントは、 <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> デバイスから。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">無効</td> 
      <td>このオプションを選択した場合、ユーザーがインタラクティブな配達確認を確認する際に、このデバイスを選択することはできません。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**作成**」をクリックします。

## 配達確認用のポップアップメッセージの設定

配達確認のポップアップメッセージを設定して、組織内のすべてのレビュー担当者に一般情報を伝えることができます。

次の状況で表示されるメッセージを設定できます。

* **メッセージの読み込み時**:配達確認が最初に開かれたときに表示されます。 配達確認の確認方法や免責事項やその他の法的テキストの提供方法をユーザーに説明するのに役立ちます。
* **決定メッセージ時**:ユーザーが配達確認に関する決定を選択すると表示されます。 ブランドや規制への準拠などのチェックリストをユーザーに提供するのに役立ちます。 決定について詳しくは、 [校正ビューアで配達確認を決定する](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **確認ボタンのテキスト**:前述の「読み込み時」ポップアップメッセージ内のボタンに表示されるラベル。

配達確認用のポップアップメッセージを作成するには：

1. クリック **編集** をクリックします。
1. メッセージを指定し、適切な書式を含めて、「 **保存**.
1. （オプション）読み込み時メッセージをカスタマイズし、確認ボタンのラベルもカスタマイズする場合は、 **編集** 右に **確認ボタンのテキスト**&#x200B;ラベルを指定して、「 **保存**.

## 配達確認のデフォルトを設定

組織の配達確認のデフォルト設定について詳しくは、 [デフォルトの配達確認設定を構成](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## 共有のデフォルトを設定

組織の配達確認を共有できるユーザー、レビュー担当者が使用できるバージョン、特定のステージに関連付けられたユーザーに自動ワークフローを含む配達確認を表示できるタイミングを指定できます。

Workfront Proof 内での設定の共有について詳しくは、 [ユーザーの共有設定を構成します](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

## Workfront Proof サイトのブランディング

Workfrontの配達確認を使用している場合は、サイトの次の領域のブランディングを設定できます。

* 配達確認が読み込まれたときに表示されるスプラッシュページ
* ログイン画面とログアウト画面
* メール通知

Workfront Proof サイトのブランディング方法について詳しくは、  [Workfront Proof サイトのブランディング](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## パスワードの詳細設定

>[!IMPORTANT]
>
>このオプションは、レガシーWorkfrontプランでのみ使用できます。 Pro、Business、Enterprise Workfrontのいずれかのプランを利用している場合、詳細なパスワード設定を構成できなくなりました。

の下 **パスワードの詳細設定**&#x200B;を使用すると、ユーザーのパスワードセキュリティを強化できます。

1. クリック **設定** をクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">パスワードの最小長</td> 
      <td>Workfront Proof のデフォルトのパスワードの長さは 6 文字です。 組織のポリシーに応じて、数を増やすことができます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>キャラクタミックス</strong> </td> 
      <td>パスワードに小文字、大文字、数字、記号を混在させて使用するようにユーザーに強制できます。 パスワードに含める文字数を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>最大文字の繰り返し</strong> </td> 
      <td>各ユーザーのパスワードで繰り返す文字数を指定できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動パスワード有効期限</td> 
      <td>ユーザーが定期的にパスワードを変更するよう強制します。 どのくらいの頻度でそれを行うかを決めます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>パスワードの繰り返し回数は許可されていません</strong> </td> 
      <td>アカウントでのパスワードの繰り返し回数を設定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プロファイルのロックアウト</strong> </td> 
      <td>指定したログイン試行が何回も失敗した後に、ユーザーをアカウントからロックアウトします。 また、アカウントに再びアクセスできるようになるまでの待ち時間も指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">30 日後にパスワードがリセットされなかった場合にユーザーをロックする</td> 
      <td>ユーザーがプロファイルのアクティベーションから 30 日以内に最初のパスワードを変更しない場合、ユーザーはアカウントからロックアウトされます。<br><p>アカウント管理者は、システムによって自動的にロックされたユーザーのロックを解除（再アクティブ化）できます。 これにより、パスワードを変更するために 7 日間の猶予期間が与えられます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">120 日間非アクティブの場合にユーザーアカウントをロックする</td> 
      <td>ユーザーがWorkfront Proof またはログインが必要な配達確認に 120 日間ログインしなかった場合、ユーザーはアカウントからロックアウトされます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>初回ログイン後にパスワードを変更</strong> </td> 
      <td>初回ログイン後に、ユーザーに一時パスワードを変更するよう求める。<p>アカウント管理者は、システムによって自動的にロックアウトされたユーザーのロックを解除（再アクティブ化）できます。</p><p>パスワード情報の詳細については、 <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Workfront Proof のログインとパスワードおよび電子メールの変更</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
