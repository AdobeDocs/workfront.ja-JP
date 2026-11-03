---
title: Adobe Workfront計画の環境推進
description: 環境プロモーション機能を使用して、Workfront計画ワークスペース、レコードタイプ、フィールド、ビューを1つのWorkfront環境から別の環境にコピーできます。 すべてを手作業で再構築する代わりに、設定をソース環境のパッケージに組み立て、ターゲット環境にインストールします。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 00706e8c7ed590cf112f4817da9740a970a4a4b3
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 4%
---

# Adobe Workfront計画の環境推進

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

<!--if Lilit says this is not for STA, break the intro and specify that; she is checking on this-->

環境プロモーション機能を使用して、Workfront計画ワークスペース、レコードタイプ、フィールド、ビューを1つのWorkfront環境から別の環境にコピーできます。

すべてを手作業で再構築する代わりに、設定をソース環境のパッケージに組み立て、ターゲット環境にインストールします。

PlanningでのEnvironment Promotionの使用は、Workfrontでの使用と同様です。 詳しくは、[Adobe Workfront testing environments](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md)の「Environment Promotion」の節を参照してください。

## Planningでの環境プロモーションの使用に関する考慮事項

* 環境プロモーションを使用するには、Workfront管理者である必要があります。
* 環境プロモーションを通じて以下を読み込みます。

  * ワークスペース
  * Workspace セクション
  * レコードタイプ
  * フィールド
  * ビュー
  * 階層
  * すべてのオブジェクトの設定の共有
  * 自動処理<!--this might not be part of it; Lilit is checking-->
  * リクエストフォーム
  * ビジネスルール
  * 接続オブジェクト
  * ワークスペースが依存するオブジェクト、またはグループ、チーム、ジョブロールなど、他のオブジェクトが共有されるオブジェクト。 次のシナリオが存在します。

    * 同じ名前のオブジェクトがターゲット環境に既に存在する場合、Workfrontは競合をフラグ付けし、その処理方法を決定します。
    * オブジェクトが共有されているチームまたはグループがターゲット環境に存在しない場合、プロモーションはそのグループを作成します。
* 各オブジェクトについて、次の操作を実行できます。

  * 新しいオブジェクトとして作成
  * 既存のオブジェクトを使用しますが、新しい名前で作成します
  * 既存のオブジェクトを上書きします。 上書きすると、ターゲット内の設定が置き換えられます。

* インストールには数分かかる場合があります。 必要に応じて、結果ページからインストールをロールバックできます。
* 可能であれば、続行する前にプロセスをテストすることをお勧めします。 実稼動環境に昇格する前に、サンドボックスまたはプレビュー環境にインストールできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>PrimeまたはUltimate Workflow パッケージと、PrimeまたはUltimate Planning パッケージ</p>
<p>スタンドアロン製品として購入した場合のPrimeまたはUltimate計画パッケージ</p>
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Workflow Standard</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>プランニングライセンス</p></td> 
   <td><p>計画標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>  
   <p>あなたはシステム管理者でなければなりません</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## 環境プロモーションを使用したプランニング設定のインポート

次の手順は、プランニング設定を別の環境に昇格させる主な手順です。

* [ ソース環境でパッケージを作成](#create-a-package-in-the-source-environment)
* [パッケージをインストールする準備をしてください](#make-the-package-ready-to-install)
* [パッケージをターゲット環境にインストールします](#install-the-package-in-the-target-environment)
* [結果の検証](#verify-the-results)

次の節の手順に従って、2つのWorkfront環境間でPlanning設定をコピーします。

### ソース環境でのパッケージの作成

1. 必要な設定が配置されているソース環境を用意します。
1. ソース環境で、**メインメニュー** ![ メインメニュー](assets/main-menu-shell.png)をクリックし、**セットアップ** > **システム** > **環境プロモーション**に移動します。
**構成パッケージ**&#x200B;のリストには、ステータス、ソース環境、デプロイされた場所が含まれている既存のパッケージが表示されます。
1. 「**パッケージを作成**」をクリックします。

   >[!TIP]
   >
   >パッケージを組み立ててインストールするには、少なくとも1つのオブジェクトが必要です。
1. 「**パッケージの詳細**」タブで、パッケージの&#x200B;**名前**&#x200B;と&#x200B;**説明**&#x200B;を入力します。 ソース環境は、現在の（ソース）環境で既に入力されています。
1. 左側のオブジェクトタイプのリストで、**プランニングワークスペース**&#x200B;を選択します。
1. 昇格するワークスペースを検索し、そのワークスペースのチェックボックスを選択して、**プランニングワークスペースを追加**&#x200B;をクリックします。 ワークスペースは、**パッケージの内容**&#x200B;の下に表示されます。

   環境プロモーション用に![Workspaceが選択されました](assets/workspace-selected-for-environment-promotion.png)
1. 「**保存してアセンブリ**」をクリックします。

   Workfrontはパッケージをアセンブリし、パッケージの&#x200B;**更新** タブにエントリを追加します。 パッケージに含まれるものを確認するには、「コンテンツ」タブを使用します。
1. （条件付き、オプション）後で終了する場合は、代わりに&#x200B;**保存して閉じる**&#x200B;をクリックします。
1. （オプション）パッケージの内容を確認するには、**コンテンツ**&#x200B;をクリックするか、**デプロイメント**&#x200B;をクリックして、このパッケージが複数回デプロイされたかどうかを確認します。

   引き続き、パッケージをインストールする準備をしてください。

### パッケージをインストールする準備をしてください

パッケージをターゲット環境にインストールする前に、テスト環境でテストすることをお勧めします。

1. 前のセクションで説明したようにパッケージの構築が完了したら、**パッケージの詳細**&#x200B;をクリックし、**編集**&#x200B;をクリックし、**ステータス**&#x200B;を&#x200B;**テスト**&#x200B;に設定し、**保存して閉じる**&#x200B;をクリックします。

   >[!TIP]
   >
   >パッケージのビルド後、そのステータスは&#x200B;**ドラフト**&#x200B;に設定されます。 パッケージを最初にテストするまで、**アクティブ**&#x200B;状態は利用できません。
1. （推奨）「**インストール**」をクリックし、テスト環境のいずれかを選択してデプロイし、設定をテストします。

   >[!TIP]
   >
   >ステータスが&#x200B;**Testing**&#x200B;に設定されている場合、実稼動環境はオプションの1つとして使用できません。

1. テスト環境にインストールした後、**編集**&#x200B;をもう一度クリックし、**ステータス**&#x200B;を&#x200B;**アクティブ**&#x200B;に設定し、**保存して閉じる**&#x200B;をクリックします。

   >[!TIP]
   >
   >テスト環境でのパッケージのインストールは、次の節で説明するように、実稼動環境でのパッケージのインストールと似ています。

   次の節に進んで、パッケージをターゲット環境にインストールします。


### パッケージをターゲット環境にインストールします

1. パッケージページで、確認したら、**インストール**&#x200B;をクリックします。
1. **Target環境** リストで、デプロイ先の環境（実稼動環境など）を選択し、**続行**&#x200B;をクリックします。 デフォルトのターゲットは現在の環境です。
1. **パッケージ情報** ページで、ソース環境とデプロイ先の環境を確認します。
1. **オブジェクトマッピング** セクションで、**グループ**&#x200B;や&#x200B;**プランニングワークスペース**&#x200B;などの各オブジェクトグループを展開して、オブジェクトをレビューします。
1. 各オブジェクトについて、**コリジョン**&#x200B;と&#x200B;**ステータス**&#x200B;列を確認し、リストから&#x200B;**デプロイメントアクション**&#x200B;を選択します。 次のオプションから選択します。

   * **新規作成**: オブジェクトをターゲットに追加します。 衝突が検出されない場合に使用します。
   * **既存の**&#x200B;を使用：オブジェクトを、同じ名前のグループなど、ターゲットに既に存在するオブジェクトにマッピングします。
   * **新しい名前で作成**：指定した名前でオブジェクトを追加します。
   * **上書き**: ターゲット内の既存のオブジェクトを、パッケージ内のオブジェクトに置き換えます。
1. （オプション）複数のオブジェクトを一度に変更するには、そのチェックボックスを選択し、グループの上部にあるデプロイメントアクションリストでアクションを選択し、「選択したオブジェクトに適用」をクリックします。 エラーのみを表示など、リストの上にあるフィルターを使用して、特定のオブジェクトに焦点を当てます。
1. エラーインジケーターを解決する。 オブジェクトに「**既存の**&#x200B;を使用」を選択した場合は、マッピング先のオブジェクトも選択する必要があります。  それ以外の場合、ステータスにエラーが表示され、**デプロイ**&#x200B;は利用できません。
1. 「**デプロイ**」、「**デプロイ**」の順にクリックして確認します。

   Workfrontにインストールページが表示され、「**このパッケージはインストール中です**」というメッセージが表示されます。 これには数分かかる場合があります。

   インストールが完了すると、成功メッセージ、パッケージがインストールされた環境、インストールされたオブジェクトのリストがページに表示されます。各オブジェクトのステータスは、**既存のものを使用**&#x200B;または&#x200B;**インストール済み（新規作成）**&#x200B;です。
1. （オプション） インストールを元に戻し、ターゲット環境から設定を削除する必要がある場合は、**インストールをロールバック**&#x200B;をクリックします。

   インストールの結果を引き続き確認します。

### 結果の検証

1. ターゲット環境/**メインメニュー**/**計画**&#x200B;に移動して、インポートされたワークスペースを見つけます。
1. レコードタイプとビューを開いて、ソースに一致するフィールドとレイアウトを確認します。 レコードは含まれないので、テーブルは空です。


