---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront for Jira] の設定'
description: ' [!DNL Jira]  および  [!DNL Workfront]  システムを統合するには、 [!DNL Adobe Workfront for Jira]  を使用できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '2373'
ht-degree: 85%

---

# [!DNL Adobe Workfront for Jira] の設定

<!-- Audited: 12/2023 -->

[!DNL Jira] および [!DNL Workfront] システムを統合するには、[!DNL Adobe Workfront for Jira] を使用できます。

アドオンをインストールした後、[!DNL Workfront] 作業アイテムが作成される場合に、[!DNL Jira] のイシューを自動的に作成するワークフローを定義できます。両方のアプリケーションの項目がリンクされ、両方のシステムで情報の一部が自動的に更新されます。

[!DNL Workfront] のすべてのユーザーおよび [!DNL Jira] は、この統合からメリットを得ることができます。最も頻繁に作業するシステムのライセンスのみ必要で、両方のシステムのライセンスが必要になるわけではありません。

このアドオンは、[!UICONTROL サーバー]および[!UICONTROL OnDemand]（または[!UICONTROL クラウド]）の [!DNL Jira] ソフトウェアのバージョンの両方で使用できます。

[!DNL Workfront for Jira] が現在サポートしている [!DNL Jira] のバージョンのリストについて、](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview)[!DNL Atlassian Marketplace] での [[!DNL Workfront for Jira] を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] plan]</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在： [!UICONTROL Pro] 以降</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規： [!UICONTROL Standard] </p>
       <p>または</p> 
       <p>現在： [!UICONTROL プラン ] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：ユーザーに関連付けられている既存のアカウントを使用するのではなく、この統合専用のシステム管理者アカウントを [!DNL Jira] と [!DNL Workfront] に個別に作成することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

設定する前に [!DNL Workfront for Jira]を使用する場合は、次の操作を行う必要があります。

* インストール [!DNL Workfront for Jira].
[!DNL Workfront for Jira] のインストールの手順については、[ [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md) をインストールを参照してください。

## [!DNL Workfront for Jira] の設定

設定 [!DNL Workfront for Jira]を使用すると、次のことができます。

* [!DNL Workfront] 項目が作成される場合、[!DNL Jira] 項目を作成するトリガーを定義します。
* [!DNL Jira] および [!DNL Workfront] の間にリンクされた項目間で同期するフィールドを指定します。

>[!NOTE]
>
>* [!DNL Jira] 環境で [!DNL Workfront for Jira] を設定した後に、すべての [!DNL Jira] ユーザーは、[!DNL Jira] の項目上に [!DNL Workfront] の右側のパネルが表示されることを確認できます。パネルには、[!DNL Workfront] からリンクされる項目に関する情報が含まれています。または、[!DNL Jira] 項目にリンクされる [!DNL Workfront] 項目は、何もないことを指定します。
>* [!DNL Jira Server] インストールを使用時に、Workfront 統合のトリガーとして識別されたプロジェクトに関連するイシューに対してのみ、Workfront パネルが表示されます。[!DNL Workfront to Jira] ワークフローのトリガーの設定の詳細については、[ [!DNL Jira]  および  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront) 間の項目を自動的にリンクするトリガーを設定を参照してください。
>

[!DNL Workfront for Jira] を設定するには、以下を実行します。

1. [!DNL Jira] に [!DNL Jira] 管理者としてログインします。
1. メインの [!DNL Jira] のメニューで「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL アドオン]**」を選択し、次に「**[!UICONTROL アドオンの管理]**」をクリックします。

1. **[!DNL Workfront]** アドオンを展開します。
1. 「**[!UICONTROL 設定]**」をクリックします。
1. 画面の指示に従って、[!DNL Workfront] にログインします。

   >[!NOTE]
   >
   >ユーザーは、接続を成功させるには、[!UICONTROL Workfront]で有効な`apiKey`何かを持つ必要があります。

   [!DNL Workfront] 管理者として [!DNL Workfront] にログインする必要があります。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront]は、ほとんどの web ベースの統合で、ユーザーの認証と承認に使用される標準である OAuth 2.0 を使用した [!DNL Jira] に接続します。
   >* [!DNL Workfront] アカウントのドメインの入力を求められたら、次の形式で入力します。*yourCompany&#39;sDomain.my.workfront.com*&#x200B;会社のドメインは通常、会社の名前です。
   >* 拡張認証は、[!DNL Workfront] 管理者が拡張認証をこの統合に対して有効にするまで使用できません。

1. Jira で、 **[!UICONTROL トリガー]** タブをクリックして、 [!DNL Jira] 新規項目 [!DNL Workfront] 項目が作成されます。

   ワークフロントから [!DNL Jira] へのトリガーの設定について詳しくは、[ [!DNL Jira]  と  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront) の間で項目を自動的にリンクするためのトリガーを設定を参照してください。

1. 「**[!UICONTROL 設定]**」タブを選択して、リンクされた [!DNL Jira] 項目と [!DNL Workfront] 項目の間のフィールドの同期を設定します。

   [!DNL Jira] と [!DNL Workfront] の間のフィールドの同期の設定について詳しくは、[ [!DNL Jira]  項目と  [!DNL Workfront]  項目の間のフィールド同期を設定](#configure-field-synchronization-between-jira-and-workfront-items)を参照してください。

   >[!NOTE]
   >
   >2 つのトリガー間のアプリケーションとフィールドの同期を定義した後、 [!DNL Workfront] タスクや問題を作成できるユーザーは、 [!DNL Jira]. ユーザーは、作成する項目の条件が [!DNL Jira] のトリガーと一致する場合、ユーザーは、[!DNL Jira] ライセンスがない場合でも項目を作成できます。また、[!DNL Jira] ユーザーはすぐに [!DNL Jira] 項目の作業を開始し、[!DNL Workfront] ライセンスがなくても [!DNL Workfront] で更新を確認できます。[!DNL Workfront] での更新は、[!DNL Jira] にも表示されます。

1. （オプション）「**[!UICONTROL アクティビティログ]**」タブを選択して、統合中に発生した可能性のあるエラーを確認します。

   [!UICONTROL アクティビティログ]について詳しくは、[ [!DNL Jira] [!UICONTROL アクティビティログ]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md)を表示を参照してください。

## [!DNL Jira] と [!DNL Workfront] の間で項目を自動的にリンクするためのトリガーを設定

[!DNL Jira] のシステム管理者は、[!DNL Workfront] の項目が特定の条件を満たしたときに [!DNL Jira] にイシューを自動的に作成するトリガーを定義できます。

>[!NOTE]
>
>統合が [!DNL Jira] で新しいイシューを作成するまでに最大 10 分かかる場合があります。

[!DNL Workfront] 項目が作成されたときに、[!DNL Jira] 項目の作成をトリガーするように設定する場合は、以下を考慮してください。

* 統合は単方向です。[!DNL Workfront] で作成した項目のみが [!DNL Jira] で自動的に作成されるようにトリガーできます。[!DNL Jira] で作成した項目を [!DNL Workfront] で自動的に作成するようにトリガーすることはできません。
* 使用できるトリガー数に制限はありません。
* [!DNL Workfront] で作成した項目が複数のトリガーに一致する場合、[!DNL Jira] には 1 つの項目だけが作成されます。項目は、最初のトリガーに従って（[!DNL Jira] で定義された順序で）[!DNL Jira] に作成されます。その他のすべてのトリガーは無視されます。
* [!DNL Workfront] の中の 1 つの項目のみが、Jira 内の 1 つの項目にリンクできます。1 つの [!DNL Workfront] 項目を複数の [!DNL Jira] イシューにリンクしたり、1 つの [!DNL Jira] イシューを複数の [!DNL Workfront] 項目にリンクしたりすることはできません。

[!DNL Jira] で項目を自動的に作成するためのトリガーを構成するには、以下のように行います。

1. システム管理者として [!DNL Jira] にログインします。
1. メイン [!DNL Jira] メニューで「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL アドオン]**」、「**[!UICONTROL アドオンを管理]**」の順にクリックします。
1. **[!DNL Workfront]** アドオンを展開します。
1. 「**[!UICONTROL 設定]**」をクリックします。
1. システム管理者として [!DNL Workfront] にログインします。

   The **[!UICONTROL トリガー]** Jira では、デフォルトで「 」タブが選択されています。

1. 「**[!UICONTROL トリガーを追加]**」をクリックして、新しいトリガーを追加します。
1. 「**[!UICONTROL Workfront チーム/ユーザー/役割]**」フィールドで、[!DNL Workfront] チーム、ユーザー、または担当業務の名前を指定し、リストに表示されたらクリックして選択します。

   >[!NOTE]
   >
   >同じチーム、ユーザー、役割に複数のトリガーを設定することはできません。

   ユーザーがタスクまたはイシューを作成し、これらのエンティティのいずれかに割り当てると、イシューが [!DNL [!DNL Jira]] に自動的に作成されます。

1. 「**[!UICONTROL [!DNL Jira]プロジェクト]**」フィールドで、[!DNL Jira] プロジェクトの名前を入力し、リストに表示されたらクリックして選択します。

   次の場合に [!DNL Jira] イシューが作成され、ここで選択したプロジェクトに配置されます。

1. ドロップダウンメニューから「**[!UICONTROL イシュータイプ]**」を選択します。

   これは、[!DNL Jira] の特定のプロジェクトの設定に基づいて、このトリガーの条件が満たされたときに、[!DNL Jira] で作成されるイシュータイプを示します。

1. 「**[!UICONTROL 保存]**」をクリックします。

   この設定を使用すると、[!DNL Workfront] ユーザーが指定されたトリガーに一致する項目を作成するたびに、新しいイシューが [!DNL Jira] に作成されます。

## [!DNL Jira] 項目と [!DNL Workfront] 項目間のフィールド同期を設定

を [!DNL Jira] 管理者は、次の間にリンクされた項目に対して、自動的に同期するフィールドを定義できます [!DNL Workfront] そしてジラ。 特定のフィールドは [!DNL Workfront] 項目から [!DNL Jira] 項目に同期でき、その他のフィールドは Jira から Workfront に同期します。

2 つのアプリケーション間でリンクされた項目でどのフィールドを自動的に同期するかを定義するには、以下のように行います。

1. にログインします。 [!DNL Jira] ジラの管理者として。
1. メイン [!DNL Jira] メニューで「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL アドオン]**」、「**[!UICONTROL アドオンを管理]**」の順にクリックします。
1. **[!DNL Workfront]** アドオンを展開します。
1. 「**[!UICONTROL 設定]**」をクリックします。
1. Workfront 管理者として [!DNL Workfront] にログインします。
1. Jira で、 **[!UICONTROL 設定]** タブをクリックします。
1. Adobe Analytics の **[!UICONTROL Workfrontから Jira に同期]** 「 」セクションで、更新するフィールドを [!DNL Jira] Workfrontで更新されたとき。

   1. フィールドの同期頻度として、次のいずれかを選択します。

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>Workfront で項目を作成された場合、指定したフィールドは、リンクされた Workfront と [!DNL Jira] 項目の間で同期されます。</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>指定したフィールドは、Workfront でフィールドが更新されると、リンクされた Workfront と [!DNL Jira] 項目の間で同期されます。 </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>指定したフィールドは、リンクされた [!DNL Workfront] および [!DNL Jira] 項目の間で同期されることはありません。[!DNL Jira] には、[!DNL Workfront] でフィールドが更新されたことを示すものはありません。 </td>
          </tr>
      </table>

   1. 次のいずれかを選択して、次のフィールドを同期します。 [!DNL Workfront] から [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>[!DNL Workfront] のタスクまたはイシューの名前は、[!DNL Jira] でリンク先のイシューの名前になります。</p><p>メモ：新しい項目が [!DNL Jira] で自動的に作成される場合、このフィールドがここで有効にされているかどうかに関係なく、[!DNL Workfront] 名は常に [!DNL Jira] 項目で更新されます。[!DNL Jira] 項目が手動で [!DNL Workfront] 項目にリンクされている場合、「<strong>常に</strong>」このフィールドを同期するように選択すると、[!DNL Workfront] 項目の名前のみが [!DNL Jira] で更新されます。項目を手動または自動でリンクする方法について詳しくは、<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">[!DNL Adobe Workfront] および [!DNL Jira]</a> の間の項目をリンクするを参照してください。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>[!DNL Workfront] でのタスクまたはイシューの説明は、[!DNL Jira] でリンク先のイシューの説明になります。</td>
        </tr>
        <tr>
         <td role="rowheader">ドキュメント</td>
         <td><p>[!DNL Workfront] でタスクまたはイシューに添付されたドキュメントは、Jira でリンクされているイシューにも添付されています。[!DNL Workfront] からの新しいドキュメントバージョンは、別のドキュメントとして Jira に追加され、<i>_v&lt;version number&gt;</i> が付加され、Workfront で番号付きバージョンを示します。 </p><p>例えば、[!DNL Workfront] でドキュメントの名前が <strong>Main Ad</strong> で、新しいバージョンを [!DNL Workfront] で追加する場合、新しいバージョンは、<strong>Main Ad_v2</strong> という名前の新しいドキュメントとして、[!DNL Jira] に転送されます。</p><p>重要： <p>ドキュメントを同期する場合、次の点を考慮してください。</p>
           <ul>
            <li><p>5MB を超えるドキュメントは同期されません。ドキュメントが大きすぎてドキュメントの同期が失敗した場合は、アクティビティログにエラーが記録されます。 </p><p>アクティビティログについて詳しくは、<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Jira アクティビティログの表示</a>を参照してください。</p></li>
            <li><p>外部サーバーからのタスクやイシューにリンクされたドキュメントは、[!DNL Jira] 項目に転送されません。[!DNL Workfront] でタスクまたはイシューに直接アップロードされたドキュメントのみが [!DNL Jira] でリンクされたイシューに転送されます。</p></li>
            <li><p>ドキュメントからプルーフを作成するには、[!DNL Workfront] でプルーフを生成する必要があります。 </p><p>プルーフの生成について詳しくは、<a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">ドキュメントのプルーフの作成</a>の<a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">既存のドキュメントのプルーフの作成</a>を参照してください。<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>[!DNL Workfront] でタスクまたはイシューの[!UICONTROL Planned Completion Date]は、[!DNL Jira] でリンクされているイシューの[!UICONTROL Due Date]になります。</p><p>メモ：この値を同期するには、[!DNL Jira] イシューの<strong>[!UICONTROL Due Date]</strong>を確実に表示します。</p></td>
        </tr>
       </tbody>
      </table>

1. 「**[!UICONTROL [!DNL Jira] から[!DNL Workfront]]** に同期」セクションで、[!DNL Jira] で更新された場合に [!DNL Workfront] で更新するフィールドを選択します。

   1. フィールドの同期頻度として、次のいずれかを選択します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>指定したフィールドは、[!DNL Jira] でフィールドが更新された場合、リンクされた [!DNL Workfront] 項目および [!DNL Jira] 項目の間で常に同期されます。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>指定したフィールドは、リンクされた [!DNL Workfront] 項目および [!DNL Jira] 項目の間で同期されることはありません。[!DNL Workfront] には、[!DNL Jira] でフィールドが更新されたことを示すものはありません。</p><p>メモ：「実行しない」を選択した場合、[!DNL Jira] イシューの左 [!DNL Workfront] パネルで [!DNL Workfront] フィールドは [!DNL Jira] から手動で更新できます。これらの更新は、[!DNL Jira] および [!DNL Workfront] で、[!DNL Jira] 項目ではなく、[!DNL Workfront] 項目にのみ表示されます。</p></td>
        </tr>
       </tbody>
      </table>

   1. [!DNL Jira] から [!DNL Workfront] の次のフィールドのいずれかを選択して同期します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>[!DNL Jira] のイシューの [!UICONTROL Status] は、[!DNL Workfront] でリンクされているタスクまたはイシューの [!UICONTROL Status] になります。<br>[!DNL Workfront] ステータスについて詳しくは、<a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">ステータスの作成または編集</a>を参照してください。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>[!DNL Jira] のイシューの [!UICONTROL Assignee] は、[!DNL Workfront] でリンクされているタスクまたはイシューの [!UICONTROL Assignee] になります。</p><p>重要： [!DNL Jira] を持たないユーザーに対して [!DNL Workfront] アカウントを使用する場合、統合により、新しいアクティブなユーザーが [!DNL Workfront] 次の場合のみ： <strong>でユーザーを自動的に作成する [!DNL Workfront] もし [!DNL Jira] ユーザーが [!DNL Workfront] アカウント</strong> が <strong>[!UICONTROL Always]</strong>. このユーザーは [!DNL Workfront] ライセンスを所有しません。アクティブユーザーは、[!DNL Workfront] で作業アイテムに割り当てることができますが、更新に含めることはできません。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>[!DNL Jira] のイシューの添付ファイルは、[!DNL Workfront] でリンクされているタスクまたはイシューにも添付されます。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>[!DNL Jira] イシューに対するコメントは、[!UICONTROL Updates] エリアのリンクされた [!DNL Workfront] 項目にも投稿されます。逆に、[!DNL Workfront] のタスクまたはイシューに関して [!UICONTROL Updates] エリアに投稿されたコメントは、リンクされたイシューに対する [!DNL Jira] のネイティブのコメントストリームに同期されます。 </p><p>デフォルトでは、<strong>[!UICONTROL Always]</strong> に設定されています。ここで <strong>[!UICONTROL Never]</strong> を選択した場合でも、[!DNL Workfront] または [!DNL Jira] でリンクされたアイテムに手動でコメントを投稿できます。</p></td>
        </tr>
       </tbody>
      </table>

1. Adobe Analytics の **[!UICONTROL その他]** 「 」セクションで、リンクされた項目間で更新する追加のフィールドを選択します。

   1. 指定したフィールドが更新されたとき、[!DNL Jira] または [!DNL Workfront] で&#x200B;**[!UICONTROL 常に]**&#x200B;更新するのか、**[!UICONTROL 決して]**&#x200B;更新しないのかを決定するオプションを選択します。

   1. 次のフィールドと更新から選択します。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Custom Data in the right panel in [!DNL Jira]]</td>
         <td><p>[!DNL Workfront] の右パネルにアイテムの [!DNL Workfront] カスタムデータが表示されます。</p><p>メモ：カスタムフォームセクションは、[!DNL Workfront] システム管理者のアクセスレベルで [!DNL Workfront] の右パネルに表示されます。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Priority in the right panel in [!DNL Jira]]</td>
         <td>[!DNL Workfront] の右パネルにアイテムの [!DNL Workfront] 優先度が表示されます。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Updates tab about Due Date changes in [!DNL Jira]]</td>
         <td>リンクされた [!DNL Jira] アイテムで [!UICONTROL Due Date] が変更された場合、[!DNL Workfront] アイテムの [!UICONTROL Update] タブにコメントを追加します。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] if the [!DNL Jira] user does not have a [!DNL Workfront] account]</td>
         <td><p>次のシナリオが存在します。</p>
          <ul>
           <li>次を選択した場合： <strong>[!UICONTROL Always]</strong>を有効にすると、統合を有効にして、 [!DNL Jira] ユーザーが [!DNL Workfront] アカウントは、リンクされた [!DNL Jira] 問題：
            <ul>
             <li>[!DNL Jira] イシューに割り当てられている</li>
             <li><p>[!DNL Jira] イシューに時間を記録する</p><p>この新しいユーザーは [!DNL Workfront] ライセンスを所有していません。デフォルト設定は「常に」です。[!DNL Workfront] でこのように作成されたユーザーには、名前に [!UICONTROL Jira] が追加されます。</p></li>
            </ul></li>
           <li>「<strong>[!UICONTROL Never]</strong>」を選択すると、次のようになります。
            <ul>
             <li>[!DNL Workfront] アイテムに対する [!DNL Jira] 割り当ては表示されなくなります。この場合、[!DNL Workfront] で行われた割り当てのみが [!DNL Workfront] アイテムに表示されます。</li>
             <li>[!DNL Workfront] アカウントを持たないユーザーが、リンクされた [!DNL Jira] イシューに記録した時間は、リンクされた [!DNL Workfront] アイテムには自動的に転送されません。[!DNL Jira] イシューの右パネルにある [!DNL Workfront] アイテムには引き続き時間を記録できます。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

   この設定で指定されたフィールドを [!DNL Jira] または [!DNL Workfront] のアイテムで更新するたびに、他のアプリケーションでリンクされたアイテムも更新されようになります。

## トラブルシューティング

### トリガーフィールドに「[!UICONTROL 見つかりませんでした]」とマークされているため、[!DNL Jira] ではアイテムを作成できません

#### 問題

次の条件で [!DNL Workfront for Jira] アプリケーション [!DNL Workfront] これ以上の合併症を防ぐためにトリガーを無効にします。 これらのトリガーが無効な場合、「[!UICONTROL 見つかりませんでした].&quot;

#### ソリューション

トリガーを無効にしたエラーを見つけます。エラーは、 [!DNL Workfront for Jira] [!UICONTROL アクティビティログ].

この動作の最も一般的な原因は、「[!UICONTROL フィールド &#39;duedate&#39; を設定できません適切な画面に表示されていないか、不明です。]」というエラーです。

このエラーは、「[!UICONTROL 予定完了日]」を [!DNL Workfront] から [!DNL Jira] に同期しようとしていることを意味します。これをおこなうには、 [!DNL Jira] オブジェクトには、「[!UICONTROL 期限].&quot; このフィールドがない場合、[!DNL Workfront] は [!DNL Workfront] から予定完了日を同期できず、トリガーが無効になります。

このエラーを解決するには、次のいずれかを試してください。

* [!DNL Jira] 管理者に、影響を受ける [!DNL Jira] オブジェクトを更新して、期限フィールドが確実に存在するように依頼してください。
* の同期を無効にする [!DNL Workfront]Workfrontでの予定完了日 [!UICONTROL 設定] ページに貼り付けます。
