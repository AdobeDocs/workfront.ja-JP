---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Adobe Workfront 内でプルーフを共有する
description: ドキュメントを共有するか、プルーフにユーザーを追加することで、Adobe Workfront 内でプルーフ済みドキュメントを共有できます。
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 5c0cd18074cffdf0a4fe15affaf61add7314a83a
workflow-type: ht
source-wordcount: '1221'
ht-degree: 100%

---

# Adobe Workfront 内でプルーフを共有する

ドキュメントを共有するか、プルーフにユーザーを追加することで、Adobe Workfront 内でプルーフ済みドキュメントを共有できます。

プルーフを共有する場合は、この記事で説明するように、受信者はドキュメントとプルーフに同じアクセス権が必要です。さらに、受信者にプルーフの承認をリクエストできます。

>[!TIP]
>
>また、プルーフビューアー内からプルーフを共有することもできます。手順については、[プルーフビューアーからプルーフを共有する](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Select または Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
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
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、役割またはプルーフ権限プロファイルを確認するには、Workfront または Workfront Proof 管理者にお問い合わせください。

## プルーフリンクの共有

プルーフリンクを共有すると、Workfront ユーザーにアクセス権が表示されます。ユーザーは、プルーフにコメントを付けることができ、Workfront のログイン資格情報でプルーフのメール通知を登録できます。プルーフ対象外のユーザーは、メールアドレスと表示名を使用してコメントや登録を行うことができます。

>[!IMPORTANT]
>
>「パブリック URL または埋め込みコード経由によるプルーフの共有を許可する」設定を有効にする必要があります。

1. ユーザーと共有するプルーフを含むドキュメントを選択します。

   選択できるのは、1 つのドキュメントのみです。複数のドキュメントのリンクを同時に共有することはできません。

1. **共有**／**プルーフリンク**&#x200B;をクリックします。
1. 表示された「**プルーフリンク**」ボックスで、次のいずれかの操作を行います。

   * リンクをクリップボードにコピーするには、「**リンクをコピー**」をクリックします。

     チャットやメールアプリケーションなど、サードパーティのツールを使ってリンクを配布できるようになりました。

   * Adobe Workfront から直接リンクをメールで送信するには、以下の操作を実行します。

      1. 「**リンクをメールする**」フィールドに入力して、受信者の名前を選択します。または、共有する外部ユーザーのメールアドレスを指定します。

         >[!NOTE]
         >
         >プルーフを共有する際にメールエイリアスが表示される場合、対応するメールエイリアスが存在するのであれば、元のメールアドレスを入力して新しいゲストユーザーを作成しないでください。

      1. 次のオプションから選択します。

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">パブリックリンクを送信</td>
            <td><p>使用しているプルーフビューア内のプルーフにユーザーを移動させるボタンをメール通知に含め、表示アクセス権を付与します。</p><p>プルーフで「<strong>公開 URL または埋め込みコードでプルーフを登録</strong>」が無効になっている場合、ユーザーは Workfront のログイン資格情報でログインし、プルーフにコメントを追加できます。このオプションを有効にすると、メールアドレスと名前（パスワードは不要）を入力したユーザーは誰でも、プルーフに署名し、コメントを追加できます。</p></td>
           </tr>
           <tr>
            <td role="rowheader">ダウンロードリンクを送信</td>
            <td>ダウンロードページにユーザーを移動させるボタンを電子メール通知に含め、そのページではファイルの詳細、ファイル名、ファイルサイズを、インラインで表示されたファイルと共に提供します。ユーザーは、ダウンロードページの「ダウンロード」リンクをクリックして、ファイルをダウンロードできます。</td>
           </tr>
           <tr>
            <td role="rowheader">カスタムメッセージを追加</td>
            <td>メール通知のカスタムの件名と本文を指定できます。</td>
           </tr>
          </tbody>
         </table>

      1. 「**送信**」をクリックします。

         受信者には、プルーフに関する情報が記載され、選択したボタンが含まれたメール通知が届きます。

         ![](assets/proof-share-email-350x87.png)

## プルーフにユーザーを追加

プルーフにに対する編集権限を持っている場合は、プルーフに任意の Workfront ユーザーを追加できます。プルーフに複数のステージがある場合は、ユーザーを個々のステージに追加します

>[!WARNING]
>
>この記事で説明する方法に加えて、既存のプルーフの「更新」タブからコメントにタグ付けして、プルーフにユーザーを追加することもできます。ただし、この方法でプルーフに追加されたユーザーは、プルーフのワークフローに追加された後で再度タグ付けされない限り、メール通知を受け取りません。
>
>そのため、ユーザーをコメントでタグ付けするのではなく、以下に示すいずれかの方法でプルーフに追加することをお勧めします。
>

>[!NOTE]
>
>従来の Workfront プランを使用し、ユーザーに対してプルーフを有効または無効にできる場合は、次の点に注意してください。
>
>* 受信者は、プルーフをレビューするために、プルーフを有効にする必要はありません
>* 自動ワークフローを有効にし、Workfront でプルーフを有効にしていないユーザーをプルーフに追加すると、自動ワークフロー内に新しいステージが作成されます。追加するユーザーが、プルーフを初めて表示する際に、自動的にこの新しいステージに追加されます。（詳しくは、[自動ワークフローの概要](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)を参照してください）。
>

### 「ドキュメント」タブからの既存のプルーフへのユーザーの追加

1. ユーザーを追加するプルーフを含むドキュメントを選択します。
1. プルーフに自動ワークフロー（ステージ）がない場合は、ステージ 1 セクションの右上隅にある&#x200B;**その他**&#x200B;アイコンをクリックし、ドロップダウンメニューの「**共有**」をクリックします。

   または

   プルーフに自動ワークフローがある場合は、レビュアーを追加するステージの右上隅にある&#x200B;**その他**&#x200B;アイコンをクリックし、ドロップダウンメニューで「**共有**」をクリックします。

1. 表示される「**このバージョンを共有**」ボックスで、**共有**&#x200B;の下に、プルーフを共有するユーザーの名前またはメールアドレスを入力し、ドロップダウンリストに表示されたら名前をクリックします。

1. （オプション）この手順を繰り返して、複数のユーザーをプルーフに追加します。
1. （オプション）レビュアーに期限を設定します。
1. （オプション）プルーフに追加したことをレビュアーに知らせたい場合は、「**メールでユーザーに通知**」が選択されていることを確認してください。
1. （オプション）メールに&#x200B;**カスタムメッセージを追加**&#x200B;します。
1. すべてのレビュアーを追加したら、「**共有**」をクリックします。

### プルーフビューアーからの既存のプルーフへのユーザーの追加

Web のプルーフビューアーと Desktop のプルーフビューアーで、プルーフをレビューしながら、プルーフにユーザーを追加できます。

詳しくは、[プルーフビューアからのプルーフの共有](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)の記事の[プルーフへのユーザーの追加とプルーフの共有](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)を参照してください。

## プルーフ承認に関するレポート

Workfront 内で共有されているプルーフの承認に関するレポートを作成できます。このレポートは、システム内で以下のプルーフの承認情報を提供します。

* 承認用に送信されたドキュメント
* 承認者の名前
* プルーフのバージョン
* プルーフ ID
* プルーフ作成日

[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)で説明されているように、オブジェクトに基づいてレポートを作成するときに、この承認にアクセスします。

プルーフの承認オブジェクトレポートについて詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の[オブジェクトに関するレポート](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects)節を参照してください。

## 共有プルーフの承認

ユーザーによってプルーフに追加され、自動ワークフローを使用して承認者の役割またはレビュアーと承認者の役割のいずれかが付与されると、承認リクエストがホームまたはマイワーク領域の「承認」タブに表示されます。その後、プルーフを確認し、プルーフに関する承認の決定を Workfront から直接行うことができます。

担当作業エリアら承認に関する決定を行う方法について詳しくは、[ホームエリアからの作業の承認](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area)または[作業の承認](../../../review-and-approve-work/manage-approvals/approving-work.md)の[作業の承認](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area)を参照してください。
