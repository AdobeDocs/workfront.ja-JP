---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 自動ワークフローテンプレートの作成と管理
description: Adobe Workfront管理者は、組織のコンテンツレビュープロセスが頻繁に繰り返される場合や、同じユーザーによってコンテンツが頻繁にレビューされる場合に、指定した配達確認の役割と通知設定を持つレビュー担当者を含む自動ワークフローテンプレートを作成できます。 自動ワークフローテンプレートは、1 人または 2 人のレビュー担当者で簡単に作成することも、多くのステージや依存関係を持つ複雑なレビュー担当者でも作成することもできます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# 自動ワークフローテンプレートの作成と管理

Adobe Workfront管理者は、組織のコンテンツレビュープロセスが頻繁に繰り返される場合や、同じユーザーによってコンテンツが頻繁にレビューされる場合に、指定した配達確認の役割と通知設定を持つレビュー担当者を含む自動ワークフローテンプレートを作成できます。 自動ワークフローテンプレートは、1 人または 2 人のレビュー担当者で簡単に作成することも、多くのステージや依存関係を持つ複雑なレビュー担当者でも作成することもできます。

自動ワークフローテンプレートを使用すると、自動ワークフローで配達確認を簡単に作成できます。 配達確認を作成する際には、必要なテンプレートを選択するだけです。

自動ワークフローテンプレートの変更、レビュー担当者やステージの追加や削除をいつでも簡単におこなえます。 また、このテンプレートを使用する配達確認作成者は、配達確認のレビュー担当者を追加または削除できます。

自動ワークフローテンプレートを使用する際は、次の点に注意してください。

1. 自動ワークフローテンプレートの設定によって、配達確認の自動ワークフローで何ができるかが決まります。 例えば、テンプレートで「ステージを追加」ボタンが無効になっている場合、配達確認の自動ワークフロー設定で作業している間は表示されません。
1. 自動ワークフローテンプレート内のステージにユーザーが追加され、配達確認のレビュー担当者としても既に存在する場合に、テンプレートを適用すると、レビュー担当者がステージから削除されます。 別のレビュー担当者をステージに追加しない場合は、レビュー担当者を追加するように促すメッセージが表示されます。
1. 自動ワークフローテンプレートを変更できるかどうかは、 Workfront管理者が設定したテンプレート設定によって異なります（を参照）。 テンプレートを変更する機能が無効になっている場合、変更できるのはテンプレートの所有者だけです。

自動ワークフローについて詳しくは、 [自動ワークフローの概要](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

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

## 自動ワークフローテンプレートの作成

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする
1. クリック **ワークフロー** をクリックします。
1. の **ワークフロー** タブ、クリック **新規** > **新規テンプレート**.

1. 内 **詳細** セクションで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">テンプレート名</td> 
      <td>（必須）テンプレートの名前を入力します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレート所有者</td> 
      <td>テンプレートを管理するWorkfront管理者またはWorkfront Proof 管理者を選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートグループ</td> 
      <td> <p> 組織の自動ワークフローがグループに整理されている場合は、グループの名前を選択できます。 詳しくは、 <a href="#create-automated-workflow-template-groups" class="MCXref xref">自動ワークフローテンプレートグループの作成</a> 詳しくは、この記事の後半で説明します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">テンプレートのタイムゾーン </td> 
      <td> <p>テンプレートのデフォルトタイムゾーンは、作業中のタイムゾーンです。 テンプレートを使用する配達確認作成者とレビュー担当者のタイムゾーンが異なる場合は、ここでタイムゾーンを変更して、ユーザーに適したタイミングでステージ期限が設定されるようにできます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">許可</td> 
      <td> <p>テンプレートを使用して配達確認を作成する際に、その人物に対して使用可能なステージアクティビティを選択できます。</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 内 **ステージ** 「 」セクションで、自動ワークフローテンプレートの各ステージを設定します。

   複数のステージを追加して、その間に作成できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>ステージ名は、「ワークフロー」セクションの上部にある自動ワークフローダイアグラム、配達確認の詳細ページ、レビュー担当者に送信される電子メール通知に表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージを有効化</td> 
      <td> <p>ステージを自動的にアクティブにするか、手動でアクティブにするかを指定します。 最初のステージで、 <strong>配達確認の作成時</strong>, <strong>特定の日時に</strong>または <strong>手動</strong>.</p> <p>その他のオプションは、親ステージを選択する必要があるので、第 2 ステージを追加する際に使用できるようになります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期限の計算元</td> 
      <td> <p>期限の計算方法を指定します。</p> 
       <ul> 
        <li> <p><strong>配達確認の作成</strong>:ドロップダウンリストで、 <strong>期限（+営業日）</strong>「 」で、配達確認の作成日に追加する稼働日数を選択して、配達確認の期限を自動的に設定します。</p> </li> 
        <li><strong>ステージの開始時</strong>:ドロップダウンリストで、 <strong>期限（+営業日）</strong>「 」で、ステージのアクティベーション日に追加する営業日数を選択して、配達確認の期限を自動的に設定します。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージをロック</td> 
      <td>コメントに対するステージのロックを許可するかどうかを指定します。 オプションは、次のステージの開始時または親ステージですべての決定がおこなわれた時に、手動または自動でステージをロックすることです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">プライマリ決定者</td> 
      <td> <p>使用可能な意思決定者は、レビュー担当者をステージに追加した後でのみ、リストに表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 名による決定のみが必要です。</td> 
      <td>ステージのレビュープロセスは、1 人の意思決定者が決定を送信するとすぐに完了します。 詳しくは、 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof での配達確認の設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">プライベートステージ</td> 
      <td>ステージに追加されていない人やWorkfront管理者以外の人に対するコメントや決定を非表示にします&lt;!&gt;— FLARE で下書き：スーパーバイザー以上

       -->. 詳しくは、「自動ワークフローの概&lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>要&lt;/a>」&lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>を参照してください&lt;/a>。&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">このステージの削除を許可しない</td> 
      <td> <p>ステージを必須にします。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. このテンプレートを使用する配達確認が常にステージ内の同じ人物に送信される場合は、配達確認を作成するたびに追加する必要がないように、ここに追加します。

   各担当者の **役割** このテンプレートおよび **E メールアラート** このテンプレートを使用する配達確認を処理する際に、ユーザーに受け取ってもらいたい。

   配達確認の役割について詳しくは、 [既定の校正の役割を設定する](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). 配達確認 E メールアラートについて詳しくは、 [ユーザーの配達確認のデフォルトを設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) 記事内  [Workfront Proof での電子メール通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   各ユーザーは 1 つのステージにのみ追加できます。 ステージに追加できるユーザーの数に制限はありません。

   >[!TIP]
   >
   >ステージダイアグラムで、ステージ間にレビュー担当者名をドラッグ&amp;ドロップできます。 使用可能なステージは青色でハイライト表示されます。

1. テンプレートに追加する他のステージに対して、上記の 2 つの手順を繰り返します。

   の上部 **ワークフロー** 「 」セクションには、設定している自動ワークフローの図が表示されます。 ステージを追加し続けると、ステージ間の依存関係を示す線でダイアグラムに表示されます。 ダイアグラム内のステージをクリックすると、そのステージの設定を表示できます。

   図を表示する必要がない場合は、 **図を非表示にする**.

1. 内 **テンプレートの共有先** 「 」セクションで、「 」オプション（テンプレートが組織全体でまだ共有されていない場合）をクリックして、使用できるユーザーを指定します。

   デフォルトでは、新しい自動ワークフローテンプレートは、組織の全員と共有されます。

1. 「**作成**」をクリックします。

## 自動ワークフローテンプレートの変更

Workfrontの配達確認管理者は、自動ワークフローテンプレートを変更できます。 変更内容は、作成時に自動的に保存されます。

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする
1. クリック **ワークフロー** をクリックします。
1. 内 **ワークフローテンプレート** 表示されるリストで、変更するテンプレートをクリックします。
1. 内 **詳細** セクションで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">テンプレート名</td> 
      <td>（必須）テンプレートの名前を入力します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレート所有者</td> 
      <td>テンプレートを管理するWorkfront管理者またはWorkfront Proof 管理者を選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートグループ</td> 
      <td> <p> 組織の自動ワークフローがグループに整理されている場合は、グループの名前を選択できます。 詳しくは、 <a href="#create-automated-workflow-template-groups" class="MCXref xref">自動ワークフローテンプレートグループの作成</a> 詳しくは、この記事の後半で説明します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートのタイムゾーン </td> 
      <td> <p>テンプレートのデフォルトタイムゾーンは、作業中のタイムゾーンです。 テンプレートを使用する配達確認作成者とレビュー担当者のタイムゾーンが異なる場合は、ここでタイムゾーンを変更して、ユーザーに適したタイミングでステージ期限が設定されるようにできます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">許可</td> 
      <td> <p>テンプレートを使用して配達確認を作成するユーザーに対して使用可能にするステージアクティビティを選択します。 </p> <p><b>警告</b>:「ステージを追加」および「ステージに人を追加」オプションを選択しない場合、テンプレートの所有者も、このテンプレートを使用する配達確認の所有者も、ステージを追加したり、配達確認を共有したりできません。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 内 **ワークフロー** セクションで、任意のステージの名前を変更し、設定を展開します。 ![](assets/arrow-button.png) 必要に応じて変更を加えます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期限の計算元</td> 
      <td> <p>期限の計算方法を指定します。</p> 
       <ul> 
        <li> <p><strong>配達確認の作成から計算された期限</strong>:内 <strong>ステージの期限を設定</strong> 「 」ドロップダウンリストで、配達確認の作成日に追加する稼動日数を選択して、配達確認の期限を自動的に設定します。</p> </li> 
        <li><strong>ステージの有効化から計算された期限</strong>:内 <strong>ステージの期限を設定</strong> 「 」ドロップダウンリストで、ステージのアクティベーション日に追加する営業日数を選択して、配達確認の期限を自動的に設定します。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージを有効化</td> 
      <td> <p>ステージを自動的にアクティブにするか、手動でアクティブにするかを指定します。 最初のステージで、 <strong>配達確認の作成時</strong>, <strong>特定の日時に</strong>または <strong>手動</strong>.</p> <p>その他のオプションは、親ステージを選択する必要があるので、第 2 ステージを追加する際に使用できるようになります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージをロック</td> 
      <td>コメントに対するステージのロックを許可するかどうかを指定します。 オプションは、次のステージの開始時または親ステージですべての決定がおこなわれた時に、手動または自動でステージをロックすることです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>1 人の意思決定者が決定を初めて送信したときにステージを終了します。 詳しくは、 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof での配達確認の設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">プライバシー</td> 
      <td>ステージに追加されていない人や、スーパーバイザー以上でない人に対するコメントおよび決定をアカウントに非表示にします。 詳しくは、 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動ワークフローの概要</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージの削除</td> 
      <td>ステージを必須にします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">件が非表示 <img src="assets/more-icon.png"></td> 
      <td>ステージにレビュー担当者を追加するか、ステージを削除します。<p>特定のステージで各配達確認が同じ人に送信される場合は、配達確認を作成するたびに追加する必要がないように、ここに名前を指定できます。 ステージに追加するユーザーの名前を入力して選択し、そのユーザーの名前を追加します <strong>役割</strong> 証明に <strong>E メールアラート</strong> ユーザーに必要な設定。 役割の校正について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">既定の校正の役割を設定する</a>. 配達確認 E メールアラートについて詳しくは、 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">ユーザーの配達確認のデフォルトを設定</a> 記事内 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Workfront Proof での電子メール通知設定</a>.</p><p>ステージに追加できるユーザー数に制限はありません</p><p>ヒント：ステージダイアグラムで、ステージ間にレビュー担当者名をドラッグ&amp;ドロップできます。 使用可能なステージは青色でハイライト表示されます。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. テンプレートに追加する他のステージに対して、手順を繰り返します。

   の上部 **ワークフロー** 「 」セクションには、設定している自動ワークフローの図が表示されます。 ステージを追加し続けると、ステージ間の依存関係を示す線でダイアグラムに表示されます。 ダイアグラム内のステージをクリックすると、そのステージの設定を表示できます。

   図を表示する必要がない場合は、 **図を非表示にする**.

1. 内 **共有先** 」セクションで、ユーザーを削除する場合は、「その他」 ![](assets/more-icon.png) ボタンをクリックし、 **削除**.

## 自動ワークフローテンプレートグループの作成 {#create-automated-workflow-template-groups}

Workfront管理者は、組織のアカウントですべての自動ワークフローテンプレートを表示および管理できます。 テンプレートをグループに整理すると便利です。

自動ワークフローテンプレートグループを作成するには：

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする
1. クリック **ワークフロー** をクリックします。
1. の **ワークフロー** タブ、クリック **新規** > **新しいテンプレートグループ**.
1. 新しいテンプレートグループのわかりやすい名前を入力し、 **入力**.

グループ間でテンプレートを移動するには、ドラッグ&amp;ドロップします。

## 自動ワークフローテンプレートを管理

1. Workfrontでメインメニューをクリックします。 ![](assets/main-menu-icon.png)、「校正」をクリックします。 ![](assets/proofing-in-main-menu.png) Workfront Proof にアクセスする

1. Workfront Proof の左側のパネルで、 **ワークフロー**.
1. の **ワークフロー** 表示されたページで、次のいずれかの操作を行います。

   * 新しいテンプレートを追加
   * 新しいテンプレートグループを追加
   * 1 つ以上のテンプレートグループを削除します
   * テンプレートの詳細へのアクセス
   * 別のテンプレートグループにテンプレートをドラッグします
