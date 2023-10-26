---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfrontと Frame.io のネイティブ統合アルファ：機能'
description: Adobe Workfrontおよび Frame.io ネイティブ統合アルファ用に計画されている機能
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Adobe Workfrontと Frame.io のネイティブ統合アルファ：機能

## 使用例と機能テスト

この統合を通じて、クリエイティブが任意のツール（CC または Frame.io）でコンテンツの作成とピアレビューを行い、プロジェクトマネージャーが作業を調整し、正式なレビュープロセスをWorkfront内で初期化および監視できるようにすることが目標です。 これは、Workfrontが提供するコンテンツレビュー機能と組み合わせて、コンテンツ承認を管理するための新しいドキュメント承認を Frame.io という両方のソリューションを利用することで実現できます。 新しいドキュメント承認と Frame.io をまとめて、新しいエンドツーエンドのコンテンツレビューと承認エクスペリエンスを形成します。 

アルファが機能する方法と参加する方法について詳しくは、 [Adobe Workfrontと Frame.io の統合アルファ：概要](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>このアルファプログラムに参加していない会社でこれらのページに遭遇した場合は、こちらの情報を慎重に扱い、詳しくはWorkfrontまたは Frame.io 管理者にお問い合わせください。

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## 機能プラン

対処しようとしている主な使用例と、それをおこなう予定の機能に関する情報を以下に示します。 <!--, along with documentation to get you started testing.-->


### Workfrontの管理者は、Workfrontグループと Frame.io アカウント間の接続を設定できます

* _Workfront内で、Workfrontグループを Frame.io アカウントに接続できます_

* 新しい Frame.io チームが Frame.io 内に作成され、接続されているWorkfrontグループを表します。

**今後のリリースでの潜在的な改善点：**

* Frame.io アカウントからWorkfrontグループを切断する

* Workfrontグループを既存の Frame.io チームに接続する

### プロジェクトコーディネーターは、Frame.io に送信するWorkfrontプロジェクトを設定し、Workfrontのクリエイティブを Frame.io のプロジェクトに追加することができます。

* Frame 接続グループを割り当てることで、Workfrontプロジェクトを Frame.io 有効としてマークする機能

* _機能強化： Workfrontプロジェクト内のタスクを Frame タスクとして切り替える機能。Frame.io 内にタスクフォルダーが順番に作成されます。_

* Workfrontプロジェクトのステータスが「現在」に設定されている場合、対応する接続済みプロジェクトが Frame に作成され、Workfrontが割り当てたユーザーが Frame プロジェクトに追加され、Frame.io から電子メール通知が送信されます

   * すべてのWorkfrontプロジェクトメンバー（ユーザーおよびチーム）は、Frame.io プロジェクト（プロジェクトの作成時以降）に共同作業者として追加されます

   * _変更： Frame が有効なWorkfrontタスクに割り当てられたユーザーとチームは、Collaborators として Frame.io プロジェクトに追加され、（プロジェクトの作成時以降に）通知されます。_

* プロジェクトが作成されると (トリガー：プロジェクトのステータスが [ 現在 ] に設定されている )、プロジェクトに追加されたドキュメント（クリエイティブブリーフ）と Frame が有効なタスクは、Frame.io プロジェクト（各作業フォルダ内）にプッシュされます

   * Frame.io に複数の不要なドキュメントを送信しないように、クリエイティブブリーフに対してのみアクティブになる前に、プロジェクトに追加するドキュメントの量を制限することをお勧めします。

* _機能強化：フレームが有効なWorkfrontタスクから明示的に割り当てられていないユーザー/チームは、Frame.io プロジェクトから削除されます_

**今後のリリースでの潜在的な改善点：**

* プロジェクトテンプレートに対してフレーム有効タスクを設定できます

* クリエイティブブリーフへの新しいバージョンのアップロードがフレームにプッシュされます

* 最適化されたプロジェクトの同期（プロジェクトの切断、プロジェクトとドキュメントの再同期など）

### Frame.io 内で、クリエイティブは、正式なレビューを受けるために、作成したアセットをWorkfrontプロジェクトに送信できます

* 単一の Frame.io アセットを WF プロジェクトまたはタスクに接続する機能。 アセット参照がWorkfront内に作成されます

* Frame.io 内の新しいバージョンのアップロードでは、Connected Assets 上のWorkfront内に新しいドキュメントバージョンが自動的に作成されます。

* _機能強化： Frame.io 内から参照先のWorkfrontタスクを完了済みとしてマークする機能_

* _機能強化：接続されたWorkfrontドキュメントが削除された場合、そのドキュメントは Frame.io 内に残り、同じプロジェクトタスクや他のプロジェクトタスクに再接続できます_

**今後のリリースでの潜在的な改善点：**

* 複数の Frame.io アセットを一度にWorkfrontに送信可能

* Frame.io 内からのWorkfrontプロジェクト/タスクに対するタイムログ

### プロジェクトコーディネーターは、Frame.io からリンクされたドキュメントに正式な承認プロセスを割り当てることができます

* Workfrontのユーザーとチームを、Frame.io 接続ドキュメントの新しいドキュメント承認に追加できます

* _機能強化：ユーザー/チームが Frame 対応ドキュメントから共有を解除すると、Frame.io Viewer でのアセットへのアクセス権も失われます。_

**今後のリリースでの潜在的な改善点：**

* 複数のアセットを 1 つのレビューとして送信

* Workfrontドキュメントに承認者/レビュー担当者を一括で割り当てる

### 関係者は、Frame.io Viewer 内でレビューと承認を実行できます。

* 関係者には通知が送信され、Frame.io ビューア内で Frame 接続ドキュメントを表示できます。

* Frame.io Viewer は、Workfront内の様々な場所 ( ドキュメントリスト、ドキュメントの詳細、Workfrontホームなど ) からアクセスできます。

* Workfrontの更新ストリームと同期される Frame.io ビューアが提供する既存のレビューおよびコメント機能を利用する機能

* _Frame.io ビューア内から新しいドキュメントの承認を決定する機能_

### Frame.io 内では、クリエイティブは、接続された Frame.io アセットに対しておこなわれた全体的な決定について通知されます。

* _機能強化：ドキュメントの全体的な承認ステータスは、Frame.io 内のアセットに表示されます。_

### プロジェクトコーディネーターは、最終アセットをAEMに送信できます

* _機能強化：既存のWorkfront + AEM Asset CS コネクタを使用して、メタデータを含むフレーム接続ドキュメントをAEMに送信できます_