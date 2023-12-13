---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfrontと Frame.io のネイティブ統合アルファ：機能'
description: Adobe Workfrontおよび Frame.io ネイティブ統合アルファ用に計画されている機能
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 31adfeffeda9fc6aa4e76ceae7ef410d9c4c178c
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 0%

---

# Adobe Workfrontと Frame.io のネイティブ統合アルファ：機能とテスト

この統合を通じて、クリエイティブが任意のツール（CC または Frame.io）でコンテンツの作成とピアレビューを行い、プロジェクトマネージャーが作業を調整し、正式なレビュープロセスをWorkfront内で初期化および監視できるようにすることが目標です。 これは、Workfrontが提供するコンテンツレビュー機能と組み合わせて、コンテンツ承認を管理するための新しいドキュメント承認を Frame.io という両方のソリューションを利用することで実現できます。 新しいドキュメント承認と Frame.io をまとめて、新しいエンドツーエンドのコンテンツレビューと承認エクスペリエンスを形成します。 

アルファが機能する方法と参加する方法について詳しくは、 [Adobe Workfrontと Frame.io の統合アルファ：概要](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>このアルファプログラムに参加していない会社でこれらのページに遭遇した場合は、こちらの情報を慎重に扱い、詳しくはWorkfrontまたは Frame.io 管理者にお問い合わせください。

## 基本的なテストシナリオ

アルファプログラムの新機能を簡単にテストできるように、新しいテスト Frame.io アカウントを作成し、新しいグループ ( ) に接続しました。 `Frame.io alpha testing` 既存のWorkfrontプレビューまたはサンドボックス環境で使用できます。

この機能をテストするには、Workfront Preview または Sandbox インスタンスにログインし、次の手順を実行してください。

>[!NOTE]
>
><span class="preview">ハイライト表示されたテキスト</span> 以下は、まだテスト用に実装されていないが、今後のリリースに含まれる機能を指します。
>

1. **コーディネーター：** Workfront内で、 `Frame.io alpha testing` プロジェクトグループとして割り当てられたグループ。

1. **コーディネーター：** Workfront内で、クリエイティブをプロジェクトに割り当てます。 <span class="preview">またはフレームが有効なタスク（サブタスクをフレームが有効になっているとマークすることはできません）</span> プロジェクトのステータスを「現在」に変更します。

1. **クリエイティブ：** メールで、新しく作成した Frame.io プロジェクトへの招待を確認してください

1. **クリエイティブ：** 招待メール内の「プロジェクトに参加」ボタンをクリックして Frame.io プロジェクトに参加し、プロジェクト内のクリエイティブの概要を確認し、選択したCreative Cloudツール内でコンテンツの作成を開始します。

1. **クリエイティブ：** 作成したアセットを Frame.io にアップロードし、リンクされたWorkfrontプロジェクトに追加します。 <span class="preview">（またはフレームが有効なタスクを割り当てました）。</span>

1. **コーディネーター：** Workfront内で、プロジェクト内でリンクされた Frame.io アセットを見つけ、レビュー担当者/承認者を割り当てます ( レビュー/承認者の割り当てについて詳しくは、 [ドキュメントに追加の承認者またはレビュー担当者を追加する](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)) をクリックします。

1. **関係者：** Workfront内で、承認リクエストをホームまたはドキュメントの詳細で表示し、Frame.io ビューアで Frame に接続されたドキュメントを確認し、フィードバックを含むコメントを残します。

1. <span class="preview">**コーディネーター：** Workfront内で、Frame.io 接続ドキュメントの「更新」セクションに、関係者が作成したコメントを表示します。</span>

1. <span class="preview">**関係者：** Frame.io ビューア内で決定を行います。</span>

1. <span class="preview">**クリエイティブ：** Frame.io 内では、アセットに対する全体的な承認の決定に注目します。</span>

1. **クリエイティブ：** Frame.io 内で、接続されたアセットのバージョンスタックに更新されたバージョンを追加して、要求された変更を適用します。

1. **コーディネーター：** Workfront内で、新しくアップロードされたバージョンに承認者/レビュー担当者を割り当て、サインオフになるまで進行状況を監視します。

## 詳細なテストシナリオ

追加機能のテストを検討している参加者向けに、より複雑なテストシナリオを作成しました。 この詳細なテストシナリオのガイドは、次の場所からダウンロードできます。 [WF + Frame.io 詳細なテストシナリオのチュートリアル](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## 機能プラン

対処しようとしている主な使用例と、それをおこなう予定の機能に関する情報を以下に示します。 <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">ハイライト表示されたテキスト</span> 以下は、まだ実装されていないが、今後のリリースに含まれる機能を指します。
>
>下の箇条書き **「今後のリリースでの潜在的な改善点」** アルファフィードバックや進化する開発計画に応じて、ヘッダーは将来のリリースに含まれる場合と含まれない場合があります。
>


### Workfrontの管理者は、Workfrontグループと Frame.io アカウント間の接続を設定できます

* <span class="preview">Workfront内で、Workfrontグループを Frame.io アカウントに接続できます</span>

* 新しい Frame.io チームが Frame.io 内に作成され、接続されているWorkfrontグループを表します。

**今後のリリースでの潜在的な改善点：**

* Frame.io アカウントからWorkfrontグループを切断する

* Workfrontグループを既存の Frame.io チームに接続する

### プロジェクトコーディネーターは、Frame.io に送信するWorkfrontプロジェクトを設定し、Workfrontのクリエイティブを Frame.io のプロジェクトに追加することができます。

* Frame 接続グループを割り当てることで、Workfrontプロジェクトを Frame.io 有効としてマークする機能

* <span class="preview">機能強化： Workfrontプロジェクト内のタスクを Frame タスクとして切り替える機能。Frame.io 内にタスクフォルダーが順番に作成されます。</span>

* Workfrontプロジェクトのステータスが「現在」に設定されている場合、対応する接続済みプロジェクトが Frame に作成され、Workfrontが割り当てたユーザーが Frame プロジェクトに追加され、Frame.io から電子メール通知が送信されます

   * すべてのWorkfrontプロジェクトメンバー（ユーザーおよびチーム）は、Frame.io プロジェクト（プロジェクトの作成時以降）に共同作業者として追加されます

   * <span class="preview">変更： Frame が有効なWorkfrontタスクに割り当てられたユーザーとチームは、Collaborators として Frame.io プロジェクトに追加され、（プロジェクトの作成時以降に）通知されます。</span>

* プロジェクトが作成されると (トリガー：プロジェクトのステータスが [ 現在 ] に設定されている )、プロジェクトに追加されたドキュメント（クリエイティブブリーフ）と Frame が有効なタスクは、Frame.io プロジェクト（各作業フォルダ内）にプッシュされます

   * Frame.io に複数の不要なドキュメントを送信しないように、クリエイティブブリーフに対してのみアクティブになる前に、プロジェクトに追加するドキュメントの量を制限することをお勧めします。

* <span class="preview">機能強化：フレームが有効なWorkfrontタスクから明示的に割り当てられていないユーザー/チームは、Frame.io プロジェクトから削除されます</span>

**今後のリリースでの潜在的な改善点：**

* プロジェクトテンプレートに対してフレーム有効タスクを設定できます

* クリエイティブブリーフへの新しいバージョンのアップロードがフレームにプッシュされます

* 最適化されたプロジェクトの同期（プロジェクトの切断、プロジェクトとドキュメントの再同期など）

### Frame.io 内で、クリエイティブは、正式なレビューを受けるために、作成したアセットをWorkfrontプロジェクトに送信できます

* 単一の Frame.io アセットを WF プロジェクトまたはタスクに接続する機能。 アセット参照がWorkfront内に作成されます

* Frame.io 内の新しいバージョンのアップロードでは、Connected Assets 上のWorkfront内に新しいドキュメントバージョンが自動的に作成されます。

* <span class="preview">機能強化： Frame.io 内から参照先のWorkfrontタスクを完了済みとしてマークする機能</span>

* <span class="preview">機能強化：接続されたWorkfrontドキュメントが削除された場合、そのドキュメントは Frame.io 内に残り、同じプロジェクトタスクや他のプロジェクトタスクに再接続できます</span>

**今後のリリースでの潜在的な改善点：**

* 複数の Frame.io アセットを一度にWorkfrontに送信可能

* Frame.io 内からのWorkfrontプロジェクト/タスクに対するタイムログ

### プロジェクトコーディネーターは、Frame.io からリンクされたドキュメントに正式な承認プロセスを割り当てることができます

* Workfrontのユーザーとチームを、Frame.io 接続ドキュメントの新しいドキュメント承認に追加できます

* <span class="preview">機能強化：ユーザー/チームが Frame 対応ドキュメントから共有を解除すると、Frame.io Viewer でのアセットへのアクセス権も失われます。</span>

**今後のリリースでの潜在的な改善点：**

* 複数のアセットを 1 つのレビューとして送信

* Workfrontドキュメントに承認者/レビュー担当者を一括で割り当てる

### 関係者は、Frame.io Viewer 内でレビューと承認を実行できます。

* 関係者には通知が送信され、Frame.io ビューア内で Frame 接続ドキュメントを表示できます。

* Frame.io Viewer は、Workfront内の様々な場所 ( ドキュメントリスト、ドキュメントの詳細、Workfrontホームなど ) からアクセスできます。

* Workfrontの更新ストリームと同期される Frame.io ビューアが提供する既存のレビューおよびコメント機能を利用する機能

* <span class="preview">Frame.io ビューア内から新しいドキュメントの承認を決定する機能</span>

### Frame.io 内では、クリエイティブは、接続された Frame.io アセットに対しておこなわれた全体的な決定について通知されます。

* <span class="preview">機能強化：ドキュメントの全体的な承認ステータスは、Frame.io 内のアセットに表示されます。</span>

### プロジェクトコーディネーターは、最終アセットをAEMに送信できます

* <span class="preview">機能強化：既存のWorkfront + AEM Asset CS コネクタを使用して、メタデータを含むフレーム接続ドキュメントをAEMに送信できます</span>
