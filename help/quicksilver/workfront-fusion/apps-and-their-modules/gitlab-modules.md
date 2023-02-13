---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: GitLab モジュール
description: Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: d55ddd97a69f00a1f42d84dc55a12d2017855776
workflow-type: tm+mt
source-wordcount: '4370'
ht-degree: 0%

---


# [!UICONTROL GitLab] モジュール

Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL GitLab]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

>[!NOTE]
>
>この記事では、API ドキュメントおよび [!DNL GitLab] 機能全般に関する情報です。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 接続 [!DNL GitLab] から [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. 任意の [!DNL Workfront Fusion] [!DNL Gitlab] モジュール、クリック **[!UICONTROL 追加]** をクリックします。
1. 次のフィールドを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 接続名 ]</td> 
      <td> <p>接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>の URL を入力します。 [!DNL GitLab] インスタンス。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL アクセストークン ]</td> 
      <td><p>[!UICONTROL プライベートトークン ] または [!UICONTROL 個人用アクセストークン ] を入力します。</p><p>での個人用アクセストークンの特定または作成に関する情報 [!DNL GitLab]詳しくは、「個人用アクセストークンの作成」( <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">個人用アクセストークン</a> 内 [!DNL GitLab] ドキュメント。</p></td> 
     </tr> 
    </tbody> 
   </table>


1. クリック **[!UICONTROL 続行]**.
1. クリック **[!UICONTROL 許可]** 接続を作成し、モジュールに戻ります。

## [!DNL GitLab] モジュールとそのフィールド

設定時に [!DNL GitLab] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL GitLab] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### トリガー

+++**[!UICONTROL ビルドステータスを見る]**

このインスタントトリガーモジュールは、ビルドのステータスが変更されたときにシナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>ビルドステータスの変更を Webhook で監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL コミット/MR/issue/snippet コメントを見る]**

このインスタントトリガーモジュールは、コミット、結合リクエスト、問題、またはコードスニペットでコメントが行われたときにシナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Webhook でコメントを監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 監視コミット（プッシュ）]**

このインスタントトリガーモジュールは、コミットがリポジトリにプッシュされると、シナリオを開始します。 タグがプッシュされた場合、このモジュールはシナリオを開始しません。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Webhook でコミットを監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 問題のコメントを見る]**

このインスタントトリガーモジュールは、問題に対するコメントが行われると、シナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Webhook でイシューコメントを監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 問題を見る]**

この [!UICONTROL 即時トリガー] モジュールは、問題が作成されたとき、または既存の問題が更新、閉じたとき、または再び開かれたときに、シナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Webhook で問題を監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 結合リクエストの監視]**

このインスタントトリガーモジュールは、次のいずれかが発生した場合にシナリオを開始します。

* 新しい結合リクエストが作成されます
* 既存の結合リクエストが更新、結合または閉じられました
* ソースブランチにコミットが追加されます


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>結合リクエストを Webhook で監視するプロジェクトです</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL 結合要求のコメントを監視する]**

このインスタントトリガーモジュールは、結合リクエストでコメントが行われるとシナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>結合要求のコメントを Webhook で監視するプロジェクトです。</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL パイプラインステータスを見る]**

このインスタントトリガーモジュールは、パイプラインのステータスが変更されたときにシナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>パイプラインステータスの変更を Webhook で監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL プロジェクトを見る]**

このスケジュール済みトリガーモジュールは、新しいプロジェクトが追加されると、シナリオを開始します。このシナリオのうち、認証済みユーザーがメンバーです。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL GitLab] アカウント [!DNL Workfront] Fusion（を参照） <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">接続 [!DNL GitLab] から [!DNL Workfront] 統合</a> 」を参照してください。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">最大結果数</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが監視するレコードの最大数を入力またはマッピングします。</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL リポジトリブランチを監視]**

このスケジュールトリガーモジュールは、新しいブランチがリポジトリに追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL GitLab] アカウント [!DNL Workfront] Fusion（を参照） <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">接続 [!DNL GitLab] から [!DNL Workfront] 統合</a> 」を参照してください。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">最大結果数</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが監視するレコードの最大数を入力またはマッピングします。</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL リポジトリタグを監視する]**

このインスタントトリガーモジュールは、リポジトリでタグが作成または削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Webhook でタグを監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL スニペットコメントを見る]**

このインスタントトリガーモジュールは、スニペットに対して新しいコメントが作成されると、シナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Webhook でコメントを監視するプロジェクト</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL トードを見る]**

このスケジュールトリガーモジュールは、新しい TODO が追加されるとシナリオを開始します。 フィルターが適用されない場合、トリガーは、新しい保留中の TODO が追加されたときに実行されます。

フィールドについて詳しくは、 [DOS のリストを取得](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL Wiki ページを見る]**

このインスタントトリガーモジュールは、Wiki ページが作成または編集されたときにシナリオを開始します。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>このトリガーで使用する Webhook を選択するか、新しい Webhook を追加します。 </p><p>新しい Webhook を追加するには、次の手順に従います。 <ol><li>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL webhook] フィールドの横にある</li><li>以下を入力します。 <ul><li>ウェブフックの名前</li><li>このウェブフックに使用する接続</li><li>Wiki ページで Webhook が監視するプロジェクトです</li></ul></li><li>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。 </td> 
   </tr> 
   </tbody> 
</table>

+++

### アクション

+++**[!UICONTROL 結合リクエストを受け入れる]**

このアクションモジュールは、送信された変更を指定された結合リクエストと結合します。

フィールドについて詳しくは、 [結合リクエストを受け入れる](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL ビルドのキャンセル]**

このアクションモジュールは、プロジェクトの単一のビルドをキャンセルします。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL GitLab] アカウント [!DNL Workfront] Fusion（を参照） <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">接続 [!DNL GitLab] から [!DNL Workfront] 統合</a> 」を参照してください。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>キャンセルするビルドを含むプロジェクトを選択またはマッピングします。</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ビルド ID]</td> 
   <td>キャンセルするビルドを選択またはマッピングします。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL コミットメッセージを結合 ]</td> 
   <td> マージのコミットメッセージを入力またはマップします。
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ソースブランチを削除する ]</td> 
   <td>結合が完了したときにソースブランチを削除するかどうかを選択します。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ビルドが成功した場合の結合 ]</td> 
   <td>ビルドが完了したら、すぐに結合リクエストを結合するかどうかを選択します。</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>存在する場合、この SHA はソースブランチのHEADと一致する必要があります。 一致しない場合、結合は失敗します。</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL パイプラインのビルドをキャンセルする]**

このアクションモジュールは、単一のパイプラインのビルドをキャンセルします。

フィールドについて詳しくは、 [パイプラインのジョブのキャンセル](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL パイプラインが成功した場合に結合をキャンセル]**

パイプラインの成功時に結合リクエストが結合に設定されている場合、このアクションモジュールはそのアクションをキャンセルします。

フィールドについて詳しくは、 [パイプラインが成功した場合に結合をキャンセル](https://docs.gitlab.com/ee/api/merge_requests.html) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL チェリーがコミットを選択]**

このアクションモジュールは、特定のブランチへのコミットを選択します。

フィールドについて詳しくは、 [チェリーがコミットを選択](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しいラベルを作成]**

このアクションモジュールは、指定されたリポジトリの新しいラベルを作成します。

フィールドについて詳しくは、 [新しいラベルを作成](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しいパイプラインの作成]**

このアクションモジュールは、指定されたプロジェクトの新しいパイプラインを作成します。

フィールドについて詳しくは、 [新しいパイプラインの作成](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しいリリースの作成]**

このアクションモジュールは、既存の Git タグにリリースノートを追加します。

フィールドについて詳しくは、 [リリースの作成](https://docs.gitlab.com/ee/api/releases/#create-a-release) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しいタグを作成]**

このアクションモジュールは、指定された参照を指す新しいタグをリポジトリに作成します。

フィールドについて詳しくは、 [新しいタグを作成](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL TODO を作成]**

このアクションモジュールは、選択した問題に対して現在のユーザーの TODO を作成します。 現在のユーザーは、このモジュールで使用される接続の資格情報で識別されるユーザーです。

フィールドについて詳しくは、 [タスクの作成](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 結合リクエストに対する TODO の作成]**

このアクションモジュールは、選択された結合リクエストに対して現在のユーザーの TODO を作成します。 現在のユーザーは、このモジュールで使用される接続の資格情報で識別されるユーザーです。

フィールドについて詳しくは、 [TODO の作成](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 結合リクエストの作成]**

このアクションモジュールは、プロジェクトに新しい結合リクエストを作成します。

フィールドについて詳しくは、 [結合リクエストの作成](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリに新しいファイルを作成]**

このアクションモジュールは、選択したリポジトリに新しいファイルを作成します。

フィールドについて詳しくは、 [リポジトリに新しいファイルを作成](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しい問題のメモを作成]**

このアクションモジュールは、単一のプロジェクトの問題に関する問題メモを作成します。

フィールドについて詳しくは、 [新しい問題のメモを作成](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しい結合リクエストメモを作成]**

このアクションモジュールは、単一の結合リクエストに対するメモを作成します。

フィールドについて詳しくは、 [新しい結合リクエストメモを作成](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しいマイルストーンを作成]**

このアクションモジュールは、プロジェクトの新しいマイルストーンを作成します。

フィールドについて詳しくは、 [新しいマイルストーンを作成](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新しいスニペットノートを作成]**

このアクションモジュールは、単一のスニペットに対して新しいメモを作成します。 スニペットノートは、ユーザーがスニペットに投稿できるコメントです。

フィールドについて詳しくは、 [新しいスニペットノートを作成](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリブランチを作成]**

このアクションモジュールは、1 つのリポジトリブランチを作成します。

フィールドについて詳しくは、 [リポジトリブランチを作成](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL ビルド変数を作成]**

このアクションモジュールは、新しいビルド変数を作成します。

フィールドについて詳しくは、 [変数を作成](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 結合リクエストの削除]**

このアクションモジュールは、管理者とプロジェクトの所有者専用です。 該当する結合リクエストを削除します

フィールドについて詳しくは、 [結合リクエストの削除](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリ内の既存のファイルを削除]**

このアクションモジュールは、リポジトリーから既存のファイルを削除します。

フィールドについて詳しくは、 [リポジトリ内の既存のファイルを削除](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリブランチを削除]**

このアクションモジュールは、リポジトリからブランチを削除します。

フィールドについて詳しくは、 [リポジトリブランチを削除](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 問題を編集]**

このアクションモジュールは、既存のプロジェクトの問題を更新します。 この呼び出しは、問題をクローズ済みとマークするためにも使用されます。

フィールドについて詳しくは、 [問題を編集](https://docs.gitlab.com/ee/api/issues.html#edit-issue) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL マイルストーンの編集]**
このアクションモジュールは、既存のプロジェクトマイルストーンを更新します。

フィールドについて詳しくは、 [マイルストーンを編集](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL ビルドを削除する]**

このアクションモジュールは、プロジェクトのビルドを消去します（ジョブアーティファクトとジョブログを削除します）。

フィールドについて詳しくは、 [ジョブの削除](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL TODO のリストを取得]**

この検索モジュールは、TODO 項目のリストを取得します。

フィールドについて詳しくは、 [DOS のリストを取得](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一のビルドの取得]**

このアクションモジュールは、プロジェクトの単一のジョブを取得します。

フィールドについて詳しくは、 [単一のジョブを取得](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一のリポジトリタグを取得]**

このアクションモジュールは、名前で決定された特定のリポジトリタグを取得します。

フィールドについて詳しくは、 [単一のリポジトリタグを取得](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 特定のデプロイメントの取得]**

このアクションモジュールは、特定のデプロイメントを取得します。

フィールドについて詳しくは、 [特定のデプロイメントの取得](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一のマイルストーンに割り当てられたすべての問題を取得する]**

この検索モジュールは、1 つのプロジェクトマイルストーンに割り当てられているすべての問題を取得します。

フィールドについて詳しくは、 [単一のマイルストーンに割り当てられたすべての問題を取得する](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリからファイルを取得]**

このアクションモジュールは、名前、サイズ、コンテンツなど、リポジトリ内のファイルに関する情報を取得します。

フィールドについて詳しくは、 [リポジトリからファイルを取得](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトユーザーの取得]**

この検索モジュールは、プロジェクトのユーザーを取得します。

フィールドについて詳しくは、 [プロジェクトユーザーの取得](https://docs.gitlab.com/ee/api/projects.html#get-project-users) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一の問題を取得]**

このアクションモジュールは、問題の詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>新しい接続を作成するには、 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL 接続 [!DNL GitLab] Workfront Fusion] に</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロジェクト ]</td> 
   <td> <p>詳細を取得する問題を含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 問題 ID]</td> 
   <td> <p>詳細を取得する問題の名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 単一の問題のメモを取得する]**

このアクションモジュールは、特定のプロジェクトの問題に関する 1 つのメモを取得します。

フィールドについて詳しくは、 [単一の問題のメモを取得する](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一の結合リクエストの取得]**

このアクションモジュールは、単一の結合リクエストに関する情報を取得します。

フィールドについて詳しくは、 [単一の結合リクエストの取得](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一の結合リクエストの変更の取得]**

この検索モジュールは、ファイルと変更を含む結合リクエストに関する情報を取得します。

フィールドについて詳しくは、 [単一の結合リクエストの変更の取得](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一の結合リクエストコミットの取得]**

このアクションモジュールは、結合リクエストコミットのリストを取得します。

フィールドについて詳しくは、 [単一の結合リクエストコミットの取得](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一の結合リクエストのメモを取得する]**

このアクションモジュールは、指定された結合リクエストに対して 1 つのメモを返します。

フィールドについて詳しくは、 [単一の結合リクエストのメモを取得する](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL マイルストーンの取得]**

このアクションモジュールは、マイルストーンの詳細を取得します。

フィールドについて詳しくは、 [単一のマイルストーンを取得する](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一のプロジェクトを取得]**

このアクションモジュールは、プロジェクトの詳細を取得します。

フィールドについて詳しくは、 [単一のプロジェクトを取得](https://docs.gitlab.com/ee/api/projects.html#get-single-project) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 単一のリポジトリブランチを取得]**

このアクションモジュールは、リポジトリブランチの詳細を取得します。

フィールドについて詳しくは、 [単一のリポジトリブランチを取得](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL スニペットメモを取得]**

このモジュールは、指定されたスニペットに対して 1 つのメモを取得します。

フィールドについて詳しくは、 [1 つのスニペットノートを取得](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL コミットのコメントを取得]**

この検索モジュールは、プロジェクト内のコミットのコメントを取得します。

フィールドについて詳しくは、 [コミットのコメントを取得](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL コミットの差分を取得]**

このアクションモジュールは、プロジェクト内のコミットの差分を取得します。

フィールドについて詳しくは、 [コミットの差分を取得](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL アーティファクトを保持]**

有効期限が設定されている場合にアーティファクトが削除されるのを防ぎます。

フィールドについて詳しくは、 [アーティファクトを保持](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL すべての結合リクエストメモのリスト]**

この検索モジュールは、1 回の結合リクエストのすべてのメモのリストを取得します。

フィールドについて詳しくは、 [すべての結合リクエストメモのリスト](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL すべてのスニペットノートを一覧表示]**

このモジュールは、1 つのスニペットのすべてのメモのリストを取得します。 スニペットノートは、ユーザーがスニペットに投稿できるコメントです。

フィールドについて詳しくは、 [??](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL コミットビルドのリスト]**

この検索モジュールは、プロジェクト内の特定のコミットに対するビルドのリストを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>新しい接続を作成するには、 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL 接続 [!DNL GitLab] Workfront Fusion] に</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>ビルドの一覧を表示するコミットを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スコープ ]</td> 
   <td> 特定のステータスでビルドするように検索を制限するには、ステータスを選択します。 このフィールドを空白のままにすると、コミットのすべてのビルドが返されます。  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 問題のリスト]**

この検索モジュールは、指定されたフィルター設定に基づいてすべての問題を返します。

フィールドについて詳しくは、 [問題のリスト](https://docs.gitlab.com/ee/api/issues.html#list-issues) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 結合時に閉じる問題のリスト]**

この検索モジュールは、指定された結合リクエストを結合することで解決されるすべての問題を取得します。

フィールドについて詳しくは、 [結合時に閉じる問題のリスト](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リストラベル]**

この検索モジュールは、プロジェクト内のすべてのラベルを取得します。

フィールドについて詳しくは、 [リストラベル](https://docs.gitlab.com/ee/api/labels.html#list-labels) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 結合リクエストのリスト]**

この検索モジュールは、すべての結合リクエストをフィルター設定で取得します。

フィールドについて詳しくは、 [結合リクエストのリスト](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 所有するプロジェクトのリスト]**

この検索モジュールは、認証済みユーザーが所有者として設定されているプロジェクトを取得します。

フィールドについて詳しくは、 [ユーザープロジェクトのリスト](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトビルドのリスト]**

この検索モジュールは、プロジェクト内のビルドのリストを取得します。

フィールドについて詳しくは、 [プロジェクトジョブのリスト](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトデプロイメントのリスト]**

この検索モジュールは、プロジェクト内のデプロイメントのリストを取得します。

フィールドについて詳しくは、 [プロジェクトデプロイメントのリスト](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトの問題に関するメモの一覧]**

この検索モジュールは、1 件のイシューに関するすべてのメモのリストを取得します。

フィールドについて詳しくは、 [プロジェクトの問題に関するメモの一覧](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトの問題のリスト]**

この検索モジュールは、指定したプロジェクトのすべての問題を返します。

フィールドについて詳しくは、 [プロジェクトの問題のリスト](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトマイルストーンの一覧]**

この検索モジュールは、プロジェクト内のすべてのマイルストーンを取得します。

フィールドについて詳しくは、 [プロジェクトマイルストーンの一覧](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトパイプラインのリスト]**

この検索モジュールは、プロジェクトのすべてのパイプラインを取得します。

フィールドについて詳しくは、 [プロジェクトパイプラインのリスト](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトリポジトリタグのリスト]**

この検索モジュールは、プロジェクトからリポジトリタグのリストを取得し、名前で逆アルファベット順に並べ替えます。

フィールドについて詳しくは、 [プロジェクトリポジトリタグのリスト](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクト変数のリスト]**

この検索モジュールは、プロジェクトの変数のリストを取得します。

フィールドについて詳しくは、 [プロジェクト変数のリスト](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL プロジェクトのリスト]**

この検索モジュールは、認証済みユーザーがメンバーであるすべてのプロジェクトを取得します。

フィールドについて詳しくは、 [すべてのプロジェクトのリスト](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリブランチをリスト]**

このモジュールは、検索語句でリポジトリブランチを検索します。

フィールドについて詳しくは、 [リポジトリブランチをリスト](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リストリポジトリのコミット]**

この検索モジュールは、プロジェクト内のリポジトリコミットのリストを取得します。

フィールドについて詳しくは、 [リストリポジトリのコミット](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリ寄稿者のリスト]**

この検索モジュールは、リポジトリ寄稿者リストを取得します。

フィールドについて詳しくは、 [寄稿者](https://docs.gitlab.com/ee/api/repositories.html#contributors) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リポジトリツリーのリスト]**

この検索モジュールは、プロジェクト内のリポジトリファイルとディレクトリのリストを取得します。

フィールドについて詳しくは、 [リポジトリツリーのリスト](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL TODO を完了済みとしてマーク]**

このアクションモジュールは、現在のユーザーの ID で指定された 1 つの保留中の todo 項目を「完了」とマークします。

フィールドについて詳しくは、 [To Do 項目を完了済みとしてマーク](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 既存の問題報告書を変更]**

問題の既存のメモを変更します。

フィールドについて詳しくは、 [既存の問題報告書を変更](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 既存の結合リクエストのメモを変更]**

結合リクエストの既存のメモを変更します。

フィールドについて詳しくは、 [既存の結合リクエストのメモを変更](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 既存のスニペットノートを変更する]**

このアクションモジュールは、スニペットの既存のメモを変更します。

フィールドについて詳しくは、 [既存のスニペットノートを変更する](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 新規問題]**

このアクションモジュールは、新しいプロジェクトの問題を作成します。

フィールドについて詳しくは、 [新しい問題](https://www.integromat.com/en/help/app/gitlab) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL ビルドを再生する]**

このアクションモジュールは、トリガーを開始するための手動のアクションを設定します。

フィールドについて詳しくは、 [ジョブを再生](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL コミットするコメントを投稿]**

このアクションモジュールは、コミットにコメントを追加します。

フィールドについて詳しくは、 [コミットするコメントを投稿](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 変数を削除]**

このアクションモジュールは、プロジェクトの変数を削除します。

フィールドについて詳しくは、 [変数を削除](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL ビルドを再試行]**

このアクションモジュールは、コミットで単一のビルドを再試行します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>新しい接続を作成するには、 <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL 接続 [!DNL GitLab] Workfront Fusion] に</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>再試行するビルドを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ビルド ID]</td> 
   <td> 再試行するビルドを選択します。 </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL パイプラインで失敗したジョブを再試行]**

このアクションモジュールは、パイプライン内の失敗したビルドを再試行します。

フィールドについて詳しくは、 [パイプラインでのジョブの再試行](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 変数の取得]**

このモジュールは、プロジェクトの特定の変数の詳細を取得します。

フィールドについて詳しくは、 [変数の詳細を表示](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL リリースの更新]**

このアクションモジュールは、リリースを更新します。

フィールドについて詳しくは、 [リリースの更新](https://docs.gitlab.com/ee/api/releases/#update-a-release) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 結合リクエストを更新]**

このアクションモジュールは、既存の結合リクエストを更新します。 ターゲットのブランチやタイトルを変更したり、MR を閉じたりすることもできます。

フィールドについて詳しくは、 [結合リクエストを更新](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) 内 [!DNL GitLab] ドキュメント。

+++

+++**[!UICONTROL 変数の更新]**

このアクションモジュールは、プロジェクトの変数を更新します。

フィールドについて詳しくは、 [変数を更新](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) 内 [!DNL GitLab] ドキュメント。

+++
