---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 設定 [!DNL Adobe Workfront for Jira]
description: 以下を使用できます。 [!DNL Adobe Workfront for Jira] を [!DNL Jira] および [!DNL Workfront] システム。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: d2c366a69b986bd8d559a18994810011c6d33441
workflow-type: tm+mt
source-wordcount: '2413'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Jira]

以下を使用できます。 [!DNL Adobe Workfront for Jira] を [!DNL Jira] および [!DNL Workfront] システム。

アドオンをインストールした後、 [!DNL Jira] が [!DNL Workfront] 作業項目が作成されます。 両方のアプリケーションの項目がリンクされ、両方のシステムで情報の一部が自動的に更新されます。

のすべてのユーザー [!DNL Workfront] および [!DNL Jira] は、この統合のメリットを受けることができます。 彼らが最も多く機能するシステムのライセンスを必要とするだけで、両方のシステムに対しては必要ありません。

このアドオンは、 [!UICONTROL サーバー] および [!UICONTROL OnDemand] ( または [!UICONTROL クラウド]) のバージョン [!DNL Jira] ソフトウェア。

のリスト [!DNL Jira] バージョン [!DNL Workfront for Jira] は現在、をサポートしています。 [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 時刻 [!DNL Atlassian Marketplace].

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 計画]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：で別々のシステム管理者アカウントを作成することをお勧めします。 [!DNL Jira] および [!DNL Workfront] ユーザーに付随する可能性のある既存の統合を使用するのではなく、この統合専用にする場合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

設定する前に [!DNL Workfront for Jira]を

* インストール [!DNL Workfront for Jira]\
   インストールの手順 [!DNL Workfront for Jira]を参照してください。 [インストール [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 設定 [!DNL Workfront for Jira]

設定 [!DNL Workfront for Jira] 次の操作を実行できます。

* 作成するトリガーを定義 [!DNL Jira] 項目： [!DNL Workfront] 項目が作成されます。
* 次の間にリンクされた項目間で同期するフィールドを指定 [!DNL Jira] および [!DNL Workfront].

>[!NOTE]
>
>* 設定後 [!DNL Workfront for Jira] を [!DNL Jira] 環境、すべて [!DNL Jira] ユーザーに表示される [!DNL Workfront] 全員の右パネル [!DNL Jira] 項目。 パネルには、リンク元の項目に関する情報が含まれています [!DNL Workfront] または次の条件を満たさないことを指定します。 [!DNL Workfront] 項目は次にリンクされます： [!DNL Jira] 項目。
>* を使用する場合、 [!DNL Jira Server] インストール時に、Workfront統合のトリガーとして識別されたプロジェクトに関連する問題に対してのみ、Workfrontパネルが表示されます。 のトリガー設定の詳細 [!DNL Workfront to Jira] ワークフローについては、 [項目を自動的にリンクするトリガーを設定 [!DNL Jira] および [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




を設定するには、以下を実行します。 [!DNL Workfront for Jira]:

1. ログイン [!DNL Jira] as a [!DNL Jira] 管理者。
1. クリック **[!UICONTROL 設定]** メイン [!DNL Jira] メニュー
1. クリック **[!UICONTROL アドオン]**&#x200B;を選択し、「 **[!UICONTROL アドオンの管理]**.

1. を展開します。 **[!DNL Workfront]** アドオン。
1. クリック **[!UICONTROL 設定]**.
1. 画面の指示に従ってにログインします。 [!DNL Workfront].

   >[!NOTE]
   >
   >ユーザーは有効な `apiKey` in [!UICONTROL Workfront] 接続が成功した場合は、

   にログインする必要があります。 [!DNL Workfront] as a [!DNL Workfront] 管理者：設定を続行します。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] 接続先 [!DNL Jira] OAuth 2.0 を使用。これは、ほとんどの Web ベースの統合で、ユーザーの認証と承認に使用される標準です。
   >* のドメインの入力を求められたら、 [!DNL Workfront] アカウントに次の形式で入力します。 *yourCompany&#39;sDomain.my.workfront.com*. 会社のドメインは通常、会社の名前です。
   >* 拡張認証は、 [!DNL Workfront] 管理者がこの統合に対して有効にします。



1. を選択します。 **[!UICONTROL トリガー]** タブをクリックして、 [!DNL Jira] 新規項目 [!DNL Workfront] 項目が作成されます。

   Workfrontでの [!DNL Jira] ワークフローについては、 [項目を自動的にリンクするトリガーを設定 [!DNL Jira] および [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. を選択します。 **[!UICONTROL 設定]** タブをクリックして、リンクされたフィールド間の同期を設定します [!DNL Jira] および [!DNL Workfront] 項目。

   次の間のフィールドの同期の設定に関する詳細 [!DNL Jira] および [!DNL Workfront]を参照してください。 [次の間のフィールド同期の設定 [!DNL Jira] および [!DNL Workfront] 項目](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >2 つのトリガー間のアプリケーションとフィールドの同期を定義した後、 [!DNL Workfront] タスクや問題を作成できるユーザーは、 [!DNL Jira]. 作成した項目の条件が、 [!DNL Jira]( ユーザーが [!DNL Jira] ライセンス。 また、任意の [!DNL Jira] ユーザーは、すぐに [!DNL Jira] 項目と、その更新内容が [!DNL Workfront]そして、それらが [!DNL Workfront] ライセンス。 での更新 [!DNL Workfront] は、 [!DNL Jira] 項目。

1. （オプション） **[!UICONTROL アクティビティログ]** タブをクリックして、統合中に発生した可能性のあるエラーを確認します。

   詳しくは、 [!UICONTROL アクティビティログ]を参照してください。 [次を表示： [!DNL Jira] [!UICONTROL アクティビティログ]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## 項目を自動的にリンクするトリガーを設定 [!DNL Jira] および [!DNL Workfront]

を [!DNL Jira] システム管理者は、 [!DNL Jira] 項目が [!DNL Workfront] が特定の条件を満たしている。

>[!NOTE]
>
>統合がで新しい問題を作成するまでに最大 10 分かかる場合があります。 [!DNL Jira].

作成のトリガーを設定する際は、次の点を考慮してください。 [!DNL Jira] 項目 [!DNL Workfront] 項目が作成されます。

* 統合は単方向です。で作成したトリガー項目のみを [!DNL Workfront] 自動的に作成される [!DNL Jira]. で作成したトリガー項目は作成できません [!DNL Jira] 自動的に [!DNL Workfront].
* 使用できるトリガー数に制限はありません。
* 項目を [!DNL Workfront] が複数のトリガーに一致する場合、 [!DNL Jira]. 項目はで作成されます。 [!DNL Jira] 最初のトリガーに従って ( それらが [!DNL Jira]) をクリックします。 その他のトリガーは無視されます。
* 次の中の 1 つの項目のみ： [!DNL Workfront] は、Jira 内の 1 つの項目にリンクできます。 リンクできません [!DNL Workfront] 項目を複数に [!DNL Jira] 問題、または 1 つ [!DNL Jira] 複数の [!DNL Workfront] 項目。

でアイテムを自動的に作成するトリガーを設定するには [!DNL Jira]:

1. ログイン [!DNL Jira] をシステム管理者として設定します。
1. クリック **[!UICONTROL 設定]** メイン [!DNL Jira] メニュー
1. クリック **[!UICONTROL アドオン]**&#x200B;を、 **[!UICONTROL アドオンの管理]**.

1. を展開します。 **[!DNL Workfront]** アドオン。
1. クリック **[!UICONTROL 設定]**.
1. にログインします。 [!DNL Workfront] をシステム管理者として設定します。

   この **[!UICONTROL トリガー]** 「 」タブがデフォルトで選択されています。

1. クリック **[!UICONTROL 追加トリガー]** をクリックして新しいトリガーを追加します。
1. 内 **[!UICONTROL Workfrontチーム/ユーザー/ロール]** フィールドに、 [!DNL Workfront] チーム、ユーザー、またはジョブの役割。次に、リストに表示されるときにクリックして選択します。

   >[!NOTE]
   >
   >同じチーム、トリガー、またはロールに対して複数のユーザーを持つことはできません。

   任意のユーザーがタスクまたはイシューを作成し、それらのエンティティの 1 つに割り当てると、[!DNL [!DNL Jira]].

1. 内 **[!UICONTROL [!DNL Jira]プロジェクト]** フィールドに、 [!DNL Jira] をクリックし、リストに表示されるときにクリックして選択します。

   次の場合に [!DNL Jira] イシューが作成され、ここで指定したプロジェクトに配置されます。

1. を選択します。 **I[!UICONTROL スータイプ]** を選択します。

   これは、 [!DNL Jira] このトリガーの条件が満たされたとき ( [!DNL Jira].

1. 「**[!UICONTROL 保存]**」をクリックします。

   この設定を使用すると、 [!DNL Workfront] ユーザーが指定したトリガーに一致する項目を作成した場合、 [!DNL Jira].

## 次の間のフィールド同期の設定 [!DNL Jira] および [!DNL Workfront] 項目

を [!DNL Jira] 管理者は、間でリンクされた項目に対して、自動的に同期するフィールドを定義できます [!DNL Workfront] そしてジラ。 特定のフィールドを [!DNL Workfront] から [!DNL Jira] アイテムや他のアイテムは、ジラからWorkfrontに同期します。

2 つのアプリケーション間でリンクされた品目に対して、自動的に同期するフィールドを定義するには、次の手順に従います。

1. ログイン [!DNL Jira] Jira 管理者として。
1. クリック **[!UICONTROL 設定]** メイン [!DNL Jira] メニュー
1. クリック **[!UICONTROL アドオン]**&#x200B;を、 **[!UICONTROL アドオンの管理]**.

1. を展開します。 **[!DNL Workfront]** アドオン。
1. クリック **[!UICONTROL 設定]**.
1. にログインします。 [!DNL Workfront] Workfront管理者。
1. 次をクリック： **[!UICONTROL 設定]** タブをクリックします。

1. 内 **[!UICONTROL Jira からWorkfrontに同期]** 「 」セクションで、更新するフィールドを [!DNL Jira] Workfrontで更新されたとき。

   1. フィールドの同期頻度として、次のいずれかを選択します。

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL 作成時 ]</td>
              <td>指定したフィールドは、リンクされたWorkfrontと [!DNL Jira] 項目 (Workfrontで項目を作成する場合 )</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>指定したフィールドは、リンクされたWorkfrontと [!DNL Jira] 項目 (Workfrontでフィールドが更新されたとき ) </td>
          </tr>
          <tr>
              <td>[!UICONTROL なし ]</td>
              <td>指定したフィールドは、リンクされた [!DNL Workfront] および [!DNL Jira] 項目。 ～には何の表れもない。 [!DNL Jira] フィールドが [!DNL Workfront]. </td>
          </tr>
      </table>

   1. 次のフィールドのいずれかを同期する場合に選択します。 [!DNL Workfront] から [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL 名前 ]</td>
         <td><p>タスクまたはイシューの名前 ( [!DNL Workfront] は、リンク先の問題の名前になります。 [!DNL Jira].</p><p>注意：で新しい項目が作成されたとき [!DNL Jira] 自動的に [!DNL Workfront] 名前は常に [!DNL Jira] 項目を選択します。このフィールドをここで有効にするかどうかに関係なく設定します。 When a [!DNL Jira] 項目が手動で [!DNL Workfront] 項目、 [!DNL Workfront] 項目のみが更新されました [!DNL Jira] 選択した場合 <strong>常に</strong> このフィールドを同期します。 項目を手動または自動でリンクする方法について詳しくは、 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">項目をリンク [!DNL Adobe Workfront] および [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 説明 ]</td>
         <td>タスクまたはイシューの説明 ( [!DNL Workfront] は、リンク先の問題の説明になります。 [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">ドキュメント</td>
         <td><p>タスクまたはの問題に添付されたドキュメント [!DNL Workfront] は、Jira でリンクされている問題にも添付されています。 次の新しいドキュメントバージョン： [!DNL Workfront] は別の文書として Jira に追加され、 <i>_v&lt;version number=""&gt;</i> をクリックして、Workfrontの番号付きバージョンを示します。 </p><p>例えば、 [!DNL Workfront] が <strong>メイン広告</strong>新しいバージョンを [!DNL Workfront]に設定されていない場合、新しいバージョンはに転送されます [!DNL Jira] という名前の新しいドキュメント <strong>メイン Ad_v2</strong>.</p><p>重要: <p>ドキュメントを同期する際は、以下の点を考慮してください。</p>
           <ul>
            <li><p>5MB を超えるドキュメントは同期されません。 ドキュメントが大きすぎるのでドキュメントの同期に失敗した場合は、アクティビティログにエラーが記録されます。 </p><p>アクティビティログについて詳しくは、 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Jira アクティビティログの表示</a>.</p></li>
            <li><p>外部サーバーからのタスクや問題にリンクされたドキュメントは、 [!DNL Jira] 項目。 タスクまたは [!DNL Workfront] が [!DNL Jira].</p></li>
            <li><p>ドキュメントから配達確認を作成するには、 [!DNL Workfront]. </p><p>配達確認の生成について詳しくは、 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">既存のドキュメントの配達確認の作成 </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">ドキュメントの配達確認の作成</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 計画完了日 ]</td>
         <td><p>タスクまたはイシューの [!UICONTROL 予定完了日 ]( [!DNL Workfront] は、リンクされている問題の [!UICONTROL 期限 ] になります。 [!DNL Jira].</p><p>注意：次を表示していることを確認します。 <strong>[!UICONTROL 期限 ]</strong> オン [!DNL Jira] 問題（この値を同期するため）。</p></td>
        </tr>
       </tbody>
      </table>

1. 内 **[!UICONTROL 同期元 [!DNL Jira] から[!DNL Workfront]]** 「 」セクションで、更新するフィールドを [!DNL Workfront] で更新されたとき [!DNL Jira].

   1. フィールドの同期頻度として、次のいずれかを選択します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>指定したフィールドは、常にリンクされた [!DNL Workfront] および [!DNL Jira] 項目 ( [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL なし ]</td>
         <td><p>指定したフィールドは、リンクされた [!DNL Workfront] および [!DNL Jira] 項目。 ～には何の表れもない。 [!DNL Workfront] フィールドが [!DNL Jira]. </p><p>注意：「なし」を選択した場合、 [!DNL Workfront] フィールドは、次の場所から手動で更新できます： [!DNL Jira] 左に [!DNL Workfront] パネル [!DNL Jira] 問題。 これらの更新は次の日にのみ表示されます： [!DNL Workfront] 項目 [!DNL Jira] および [!DNL Workfront] ではなく [!DNL Jira] 項目。</p></td>
        </tr>
       </tbody>
      </table>

   1. 次のフィールドのいずれかを同期する場合に選択します。 [!DNL Jira] から [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL ステータス ]</td>
         <td>の問題の [!UICONTROL ステータス ] [!DNL Jira] は、タスクまたはタスクがリンクされている問題の [!UICONTROL ステータス ] になります。 [!DNL Workfront].<br>詳しくは、 [!DNL Workfront] ステータスについては、 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">ステータスの作成または編集</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 担当者 ]</td>
         <td><p>問題の [!UICONTROL 担当者 ] ( [!DNL Jira] は、タスクまたはタスクがリンクされている問題の [!UICONTROL 担当者 ] になります。 [!DNL Workfront].</p><p>重要：項目を [!DNL Jira] を [!DNL Workfront] アカウントを使用する場合、統合により、新しいアクティブユーザーが [!DNL Workfront] 次の場合のみ <strong>でユーザーを自動的に作成 [!DNL Workfront] ( [!DNL Jira] ユーザーが [!DNL Workfront] アカウント</strong> が <strong>[!UICONTROL Always]</strong>. このユーザーは [!DNL Workfront] ライセンス。 アクティブなユーザーは、 [!DNL Workfront]更新に含めることはできません。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 添付ファイル ]</td>
         <td>の問題の添付ファイル [!DNL Jira] は、タスクまたはタスクがリンクされているタスクまたはタスクにも添付されます [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL コメント ]</td>
         <td><p>に対するコメント [!DNL Jira] 問題はリンクされた [!DNL Workfront] 項目を [!UICONTROL Updates] 領域に追加しました。 反対に、[!UICONTROL Updates] 領域に投稿された、 [!DNL Workfront] タスクまたは発行の同期 [!DNL Jira]リンクされた問題に対するのネイティブコメントストリーム。 </p><p>これは <strong>[!UICONTROL Always]</strong> デフォルトでは。 次を選択した場合、 <strong>[!UICONTROL なし ]</strong> ここでは、 [!DNL Workfront] または [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. 内 **[!UICONTROL その他]** 「 」セクションで、リンクされた項目間で更新する追加のフィールドを選択します。

   1. 指定したフィールドを特定するオプションを選択します **[!UICONTROL 常に]** または **[!UICONTROL なし]** 更新 [!DNL Jira] または [!DNL Workfront] 変更時。

   1. 次のフィールドから選択して更新します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL コピー [!DNL Workfront] カスタムデータを [!DNL Jira]]</td>
         <td><p>次を表示： [!DNL Workfront] の項目のカスタムデータ [!DNL Workfront] 右パネル。</p><p>注意：カスタムフォームセクションは、 [!DNL Workfront] のアクセスレベルを持つ右側のパネル [!DNL Workfront] システム管理者。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL コピー [!DNL Workfront] の右パネルの優先度 [!DNL Jira]]</td>
         <td>次を表示： [!DNL Workfront] 内の項目の優先度 [!DNL Workfront] 右パネル。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL 更新を [!DNL Workfront] の期限変更に関する「更新」タブ [!DNL Jira]]</td>
         <td>[!UICONTROL Update] タブでコメントを追加します。 [!DNL Workfront] 項目 ([!UICONTROL 期限 ] がリンクされた [!DNL Jira] 項目。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront] ( [!DNL Jira] ユーザーが [!DNL Workfront] account]</td>
         <td><p>次のシナリオが存在します。</p>
          <ul>
           <li>次を選択した場合： <strong>[!UICONTROL Always]</strong> 統合を有効にすると、 [!DNL Jira] ユーザーが [!DNL Workfront] アカウントは、リンクされた [!DNL Jira] 問題：
            <ul>
             <li>次に割り当てられている： [!DNL Jira] 問題</li>
             <li><p>に時間を記録します。 [!DNL Jira] 問題</p><p>この新しいユーザーは [!DNL Workfront] ライセンス。 デフォルト設定は「常に」です。 ユーザーが次の方法で作成しました： [!DNL Workfront] には、名前に「[!UICONTROL Jira]」が追加されています。</p></li>
            </ul></li>
           <li>次を選択した場合： <strong>[!UICONTROL なし ]</strong>では、次のことが発生します。
            <ul>
             <li>次の項目は表示されません： [!DNL Jira] 割り当て [!DNL Workfront] 項目。 この場合、 [!DNL Workfront] 表示 [!DNL Workfront] 項目。</li>
             <li>リンクされた [!DNL Jira] を使用しないユーザーによる問題 [!DNL Workfront] アカウントは、リンクされた [!DNL Workfront] 項目。 ログイン後も、 [!DNL Workfront] の右パネルにある項目 [!DNL Jira] 問題。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

   これで、ユーザーが次のいずれかの項目に対して、この設定で指定されたフィールドを更新するたびに、 [!DNL Jira] または [!DNL Workfront]を指定した場合、他のアプリケーション内のリンクされた項目も更新されます。

## トラブルシューティング

### で項目を作成できません [!DNL Jira] 「 」とマークされたトリガーフィールドが原因で[!UICONTROL 見つかりませんでした]&quot;

#### 問題

次の [!DNL Workfront for Jira] アプリケーション [!DNL Workfront] これ以上の合併症を防ぐトリガーを無効にします。 これらのトリガーが無効な場合、「[!UICONTROL 見つかりませんでした]&quot;.

#### 解決策

エラーを見つけます。トリガー。 エラーは、 [!DNL Workfront for Jira] &quot;[!UICONTROL アクティビティログ]&quot;.

この動作の最も一般的な原因は、エラー「[!UICONTROL フィールド「duedate」を設定できません。 該当する画面に表示されていないか、不明です。]&quot;

このエラーは、「[!UICONTROL 計画完了日]から [!DNL Workfront] から [!DNL Jira]. これをおこなうには、 [!DNL Jira] オブジェクトには、「[!UICONTROL 期限]&quot;. このフィールドがない場合は、 [!DNL Workfront] は、計画完了日を次の日から同期できません： [!DNL Workfront] とは、トリガーを無効にします。

このエラーを解決するには、次のいずれかを試してください。

* 質問する [!DNL Jira] 影響を受ける管理者 [!DNL Jira] オブジェクトを使用して、期限フィールドが設定されていることを確認します。
* の同期を無効にする [!DNL Workfront]Workfrontでの予定完了日[!UICONTROL 設定]&quot;ページ
