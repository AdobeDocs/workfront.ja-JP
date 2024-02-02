---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 自動ワークフローテンプレートの作成と管理
description: 組織のコンテンツレビュープロセスが頻繁に繰り返される場合や、コンテンツが同じ担当者によって頻繁にレビューされる場合、Adobe Workfront 管理者は、指定した校正ロールと通知設定を持つレビュー担当者を含む自動ワークフローテンプレートを作成できます。自動ワークフローテンプレートは、レビュー担当者が 1 人か 2 人だけの単純なものもあれば、多くの段階と依存関係を持つ複雑なものもあります。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: ht
source-wordcount: '2096'
ht-degree: 100%

---

# 自動ワークフローテンプレートの作成と管理

組織のコンテンツレビュープロセスが頻繁に繰り返される場合や、コンテンツが同じ担当者によって頻繁にレビューされる場合、Adobe Workfront 管理者は、指定した校正ロールと通知設定を持つレビュー担当者を含む自動ワークフローテンプレートを作成できます。自動ワークフローテンプレートは、レビュー担当者が 1 人か 2 人だけの単純なものもあれば、多くの段階と依存関係を持つ複雑なものもあります。

自動ワークフローテンプレートを使用すると、自動ワークフローでプルーフを簡単に作成できます。ユーザーがプルーフを作成するときは、必要なテンプレートを選択するだけです。

自動ワークフローテンプレートは、いつでも簡単に変更でき、レビュー担当者やステージを追加または削除できます。また、テンプレートを使用するプルーフ作成者は、プルーフのレビュー担当者を追加または削除できます。

自動ワークフローテンプレートを使用する場合は、次の点を考慮してください。

1. 自動ワークフローテンプレートの設定により、プルーフの自動ワークフローで何ができるかが決まります。例えば、テンプレートで「ステージの追加」ボタンが無効になっている場合、プルーフの自動ワークフロー設定を操作するときにこのボタンは表示されません。
1. 自動ワークフローテンプレートでユーザーが sage に追加されており、プルーフのレビュー担当者としてもすでに存在している場合、テンプレートを適用するとレビュー担当者がステージから削除されます。ステージに別のレビュアーを追加しない場合は、レビュアーを追加するように求めるメッセージが表示されます。
1. 自動ワークフローテンプレートを変更できるかどうかは、「 」で説明されているように、Workfront 管理者が構成したテンプレート設定によって異なります。テンプレートを変更する機能が無効になっている場合、テンプレートの所有者のみがテンプレートを変更できます。

自動ワークフローの詳細については、[自動ワークフローの概要](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)を参照してください。

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
   <td> <p>プルーフ権限プロファイルで管理者を選択しておく必要があります。詳しくは、<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">ユーザーのプルーフアクセスを設定する</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 自動ワークフローテンプレートの作成

1. Workfront から、メインメニュー ![](assets/main-menu-icon.png)、プルーフ ![](assets/proofing-in-main-menu.png) の順にクリックして Workfront Proof にアクセスします。
1. 左側のパネルで「**ワークフロー**」をクリックします。
1. 「**ワークフロー**」タブで、**新規**／**新しいテンプレート**&#x200B;をクリックします。

1. 「**詳細**」セクションで、次の情報を指定します。

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
      <td>テンプレートを管理する Workfront 管理者または Workfront Proof 管理者を選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートグループ</td> 
      <td> <p> 組織の自動ワークフローがグループに編成されている場合は、グループの名前を選択できます。詳しくは、この記事で後述する<a href="#create-automated-workflow-template-groups" class="MCXref xref">自動ワークフローテンプレートグループの作成</a>を参照してください。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">テンプレートのタイムゾーン </td> 
      <td> <p>テンプレートのデフォルトのタイムゾーンは、作業しているタイムゾーンです。テンプレートを使用するプルーフ作成者とレビュアーのタイムゾーンが異なる場合は、ここでタイムゾーンを変更して、ステージの期限をそれらのユーザーにとって適切な時間に設定できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">許可</td> 
      <td> <p>テンプレートを使用してプルーフを作成する人が利用できるステージアクティビティを選択できます。</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. **ステージ**&#x200B;セクションで、自動ワークフロテンプレートの各ステージを構成します。

   複数のステージを追加したり、ステージ間に作成したりできます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>ステージ名は、「ワークフロー」セクションの上部、プルーフの詳細ページ上、レビュー担当者に送信されるメール通知内にある、「自動化ワークフロー」ダイアグラム上に表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージをアクティブ化</td> 
      <td> <p>ステージを自動または手動のどちらでアクティブ化するかを指定します。最初のステージで、「<strong>プルーフ作成日時</strong>」「<strong>指定日時</strong>」「<strong>手動</strong>」を選択できます。</p> <p>それ以外のオプションは、親ステージを選択する必要があるため、2 つ目のステージを追加すると使用できるようになります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期限の計算元</td> 
      <td> <p>期限の計算方法を、以下のように指定します。</p> 
       <ul> 
        <li> <p><strong>プルーフ作成日時</strong>：「<strong>期限（+ 営業日）</strong>」の下にあるドロップダウンリストで、プルーフの作成日に加算する営業日数を選択して、プルーフの期限を自動的に設定します。</p> </li> 
        <li><strong>ステージの開始時</strong>：「<strong>期限（+ 営業日）</strong>」の下にあるドロップダウンリストで、ステージのアクティベーション日に加算する営業日数を選択して、プルーフの期限を自動的に設定します。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージのロック</td> 
      <td>コメント用にステージのロックを許可するかどうかを指定します。オプションとして、次のステージの開始時または親ステージですべての決定が行われた時にステージを手動でロックするか自動的にロックするかを選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要な校正判断者</td> 
      <td> <p>対応可能な校正判断者は、レビュー担当者をステージに追加した後にのみ、リストに表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つの決定のみが必要です</td> 
      <td>ステージのレビュープロセスは、校正判断者の誰かが決定を送信するとすぐに完了します。詳しくは、<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof でのプルーフの設定</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">プライベートステージ</td> 
      <td>ステージに追加されていない人や Workfront 管理者ではない人からのコメントと決定を非表示にします&lt;!--
        FLARE でドラフトを作成：
         スーパーバイザー以上

       -->. 詳しくは、&lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>自動化ワークフローの概要&lt;/a>を参照してください。&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">このステージの削除を許可しない</td> 
      <td> <p>ステージを必須にします。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. このテンプレートを使用するプルーフが常にステージ内の同一人物に送信される場合は、プルーフを作成するたびに追加する必要がないように、ここに追加します。

   このテンプレートを使用するプルーフの各担当者の&#x200B;**役割**&#x200B;と、このテンプレートを使用するプルーフでユーザーが作業する際に受け取ってもらいたい&#x200B;**メールアラート**&#x200B;を選択します。

   プルーフの役割について詳しくは、[デフォルトのプルーフの役割を設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)を参照してください。プルーフのメールアラートについて詳しくは、[Workfront Proof でのメール通知の設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)の記事にある[ユーザーのプルーフのデフォルト設定を指定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur)の節を参照してください。

   各ユーザーは 1 つのステージにのみ追加できます。ステージに追加できるユーザーの数に制限はありません。

   >[!TIP]
   >
   >ステージダイアグラムで、ステージの間にレビュー担当者の名前をドラッグ＆ドロップできます。使用可能なステージは青色でハイライト表示されます。

1. テンプレートに追加する他のすべてのステージに対して、上記の 2 つの手順を繰り返します。

   「**ワークフロー**」セクションの上部で、設定中の自動化ワークフローのダイアグラムを確認できます。ステージの追加を続けると、ステージ間の依存関係を示す線と共にダイアグラムに表示されます。ダイアグラム内のステージをクリックすると、そのステージの設定を確認できます。

   ダイアグラムを表示する必要がない場合は、「**ダイアグラムを隠す**」をクリックします。

1. 「**テンプレートを次と共有する**」セクションで、オプション（テンプレートがまだ組織全体で共有されていない場合）をクリックして、テンプレートを使用できるユーザーを指定します。

   デフォルトでは、自動化ワークフローの新しいテンプレートは組織の全員と共有されます。

1. 「**作成**」をクリックします。

## 自動化ワークフローのテンプレートの変更

Workfront のプルーフ管理者は、自動化ワークフローのテンプレートを変更できます。変更内容は、変更時に自動的に保存されます。

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、「プルーフ」![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。
1. 左側のパネルで「**ワークフロー**」をクリックします。
1. 表示される「**ワークフローテンプレート**」リストで、変更するテンプレートをクリックします。
1. 「**詳細**」セクションで、次の情報を指定します。

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
      <td>テンプレートを管理する Workfront 管理者または Workfront Proof 管理者を選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートグループ</td> 
      <td> <p> 組織の自動ワークフローがグループに編成されている場合は、グループの名前を選択できます。詳しくは、この記事で後述の<a href="#create-automated-workflow-template-groups" class="MCXref xref">自動化ワークフローテンプレートグループの作成</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートのタイムゾーン </td> 
      <td> <p>テンプレートのデフォルトのタイムゾーンは、作業しているタイムゾーンです。テンプレートを使用するプルーフ作成者とレビュアーのタイムゾーンが異なる場合は、ここでタイムゾーンを変更して、ステージの期限をそれらのユーザーにとって適切な時間に設定できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">許可</td> 
      <td> <p>テンプレートを使用するプルーフ作成者から使用できるステージアクティビティを選択します。 </p> <p><b>警告</b>：「ステージを追加」および「ステージにユーザーを追加」オプションを選択しない場合、テンプレート所有者も、このテンプレートを使用するプルーフの所有者も、ステージを追加したり、プルーフを共有したりできません。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **ワークフロー**&#x200B;セクションで、ステージの名前を変更し、そのステージの設定 ![](assets/arrow-button.png) を展開して、必要な変更を加えます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期限の計算元</td> 
      <td> <p>期限の計算方法を、以下のように指定します。</p> 
       <ul> 
        <li> <p><strong>期限をプルーフ作成から計算</strong>：<strong>ステージ期限を設定</strong>ドロップダウンリストで、プルーフの作成日に追加する営業日の数を選択して、プルーフの期限を自動的に設定します。</p> </li> 
        <li><strong>期限をステージのアクティブ化から計算</strong>：<strong>ステージの期限を設定</strong>ドロップダウンリストで、ステージがアクティブになる日に追加する営業日の数を選択して、プルーフの期限を自動的に設定します。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージをアクティブ化</td> 
      <td> <p>ステージを自動または手動のどちらでアクティブ化するかを指定します。最初のステージの場合は、「<strong>プルーフ作成日時</strong>」、「<strong>指定日時</strong>」または「<strong>手動</strong>」を選択できます。</p> <p>それ以外のオプションは、親ステージを選択する必要があるため、2 つ目のステージを追加すると使用できるようになります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージのロック</td> 
      <td>コメント用にステージのロックを許可するかどうかを指定します。オプションとして、次のステージの開始時または親ステージですべての決定が行われた時にステージを手動でロックするか自動的にロックするかを選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>意思決定者の 1 人が初めて決定を送信したときに、ステージが終了します。詳しくは、<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof でのプルーフの設定</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">プライバシー</td> 
      <td>ステージに追加されていない人や、スーパーバイザー以上でない人からのコメントや決定を、アカウントで非表示にします。詳しくは、<a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化ワークフローの概要</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージの削除</td> 
      <td>ステージを必須にします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">その他 <img src="assets/more-icon.png"></td> 
      <td>ステージにレビュー担当者を追加するか、ステージを削除します。<p>特定のステージで各プルーフが同一人物に送信される場合は、プルーフを作成するたびに名前を追加する必要がないように、ここに名前を指定することができます。ステージに追加するユーザーの名前を入力および選択して、プルーフでの<strong>役割</strong>と、ユーザーに必要な<strong>メールアラート</strong>設定を追加します。プルーフの役割については、<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">デフォルトのプルーフ役割の設定</a>を参照してください。プルーフのメールアラートについては、<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Workfront Proof でのメール通知の設定</a>の記事にある<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">ユーザーのプルーフのデフォルト設定</a>の節を参照してください。</p><p>ステージに追加できるユーザーの数に制限はありません</p><p>ヒント：ステージダイアグラムで、レビュー担当者の名前をステージ間にドラッグ＆ドロップできます。使用可能なステージは青色でハイライト表示されます。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. テンプレートに追加する他のステージについて、この手順を繰り返します。

   「**ワークフロー**」セクションの上部に、設定中の自動化ワークフローのダイアグラムが表示されます。ステージの追加を続けると、ステージ間の依存関係を示す線と共にダイアグラムに表示されます。ダイアグラム内のステージをクリックすると、そのステージの設定を確認できます。

   図を表示する必要がない場合は、「**ダイアグラムを隠す**」をクリックします。

1. 「**共有：**」セクションでユーザーを削除する場合は、その他ボタン ![](assets/more-icon.png) をクリックし、続いて「**削除**」をクリックします。

## 自動化ワークフローテンプレートグループの作成 {#create-automated-workflow-template-groups}

Workfront 管理者は、組織のアカウントにあるすべての自動化ワークフローテンプレートを表示および管理することができます。テンプレートをグループに整理すると便利なことがあります。

自動化ワークフローテンプレートグループを作成するには、次の手順に従います。

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、続いてプルーフアイコン ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。
1. 左パネルの「**ワークフロー**」をクリックします。
1. 「**ワークフロー**」タブで、**新規**／**新規テンプレートグループ**&#x200B;をクリックします。
1. 新規テンプレートグループのわかりやすい名前を入力し、**Enter** キーを押します。

グループ間でテンプレートを移動するには、ドラッグ＆ドロップします。

## 自動化ワークフローテンプレートの管理

1. Workfront でメインメニュー ![](assets/main-menu-icon.png) をクリックし、続いてプルーフアイコン ![](assets/proofing-in-main-menu.png) をクリックして Workfront Proof にアクセスします。

1. Workfront Proof の左パネルで、「**ワークフロー**」をクリックします。
1. 表示される&#x200B;**ワークフロー**&#x200B;ページで、次のいずれかの操作を行います。

   * 新規テンプレートを追加
   * 新規テンプレートグループを追加
   * 1 つ以上のテンプレートグループを削除
   * テンプレートの詳細にアクセス
   * 別のテンプレートグループにテンプレートをドラッグ
