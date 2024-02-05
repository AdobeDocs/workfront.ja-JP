---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: ' [!DNL Jira]  と  [!DNL Adobe Workfront] 間のリンクされた項目を更新'
description: ' [!DNL Jira]  のイシューを  [!DNL Adobe Workfront]  のタスクまたはイシューにリンクすると、1 つのアプリケーションの項目を更新できます。また、2 つ目のアプリケーションで作業しているユーザーの項目を更新することもできます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 97%

---

# [!DNL Jira] と [!DNL Adobe Workfront] 間のリンクされた項目を更新

[!DNL Jira] のイシューを [!DNL Adobe Workfront] のタスクまたはイシューにリンクすると、1 つのアプリケーションの項目を更新できます。また、2 つ目のアプリケーションで作業しているユーザーの項目を更新することもできます。

[!DNL Workfront] と [!DNL Jira] の項目間のリンクについて詳しくは、[Adobe Workfront と Jira 間の項目のリンク](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)を参照してください。

[!DNL Jira] のシステム管理者として、[!DNL Jira] 用に [!DNL Workfront] を設定する際に、単一のアプリケーションの特定のフィールドを、他のアプリケーションのリンクされた項目のフィールドと同期するように設定することができます。

リンクされた [!DNL Jira] と [!DNL Workfront] の項目間のフィールドの同期について詳しくは、[ [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) の設定を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在： [!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規： [!UICONTROL Standard]</p>
       <p>または</p>
       <p>現在： [!UICONTROL プラン ]</p> </td> 
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

次の間で項目をリンクする前に： [!DNL Workfront] および [!DNL Jira]を使用する場合は、次の操作を行う必要があります。

* [!DNL Workfront for Jira] をインストールする。

  [!DNL Workfront for Jira] をインストールする手順については、「[ [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md) をインストール」を参照してください。

* [!DNL Workfront for Jira] を設定する。

  [!DNL Workfront for Jira] の設定手順については、[ [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) の設定を参照してください。

* [!DNL Workfront] と [!DNL Jira] の間の項目をリンクさせる。

  手順については、「[ [!DNL Adobe Workfront]  と  [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md) の間にの項目をリンクさせる」を参照してください。

## [!DNL Workfront] 内のリンクされた項目を更新する。

主に [!DNL Workfront] で作業している場合、[!DNL Workfront] で作業アイテムを更新すると、[!DNL Jira] の作業アイテムも更新されます。このアップデートは、[!DNL Jira] のライセンスを必要としない [!DNL Jira] 用に [!DNL Workfront] の統合によって行われます。

[!DNL Workfront] の管理者がリンクされた項目間でフィールドを同期するように [!DNL Workfront for Jira] を設定している場合に限り、[!DNL Workfront] で更新した特定のフィールドは、リンクされた [!DNL Jira] のイシューでも更新されます。[!DNL Workfront] の項目の更新について詳しくは、[イシューを編集](../../manage-work/issues/manage-issues/edit-issues.md)および[タスクを編集](../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

次のリストは、どの [!DNL Workfront] フィールドがリンクされた項目の [!DNL Jira] フィールドと同期するかを示しています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>更新された [!DNL Workfront] フィールド</strong> </th> 
   <th><strong>同期された [!DNL Jira] フィールド／更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>[!DNL Jira] イシューの「<strong>[!DNL Workfront]</strong>」タブに、名前の変更に関するコメントが追加されました。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>[!DNL Jira] イシューの「<strong>[!DNL Workfront]</strong>」タブに、更新された説明に関するコメントが追加されました。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>メモ：外部サーバーから [!DNL Workfront] 内の項目にリンクされたドキュメントは [!DNL Jira] 内のイシューには転送されません。[!DNL Workfront] 内の項目に直接アップロードされたドキュメントのみ、リンクされた [!DNL Jira] 内のイシューにもアップロードされます。</p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>[!DNL Jira] イシューの <strong>[!DNL Workfront]</strong> タブに、アップロードされた添付ファイルに関するコメントが追加されました。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>[!UICONTROL Due Date] の変更に関するコメントが [!DNL Jira] イシューの「[!DNL Workfront]」タブに追加されました。</p> <p>メモ：このフィールドが [!UICONTROL Jira] で更新されるのを確認するには、[!DNL Jira] イシューの <strong>[!UICONTROL Due Date]</strong> を有効にする必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td>カスタムフォームとカスタムフィールド</td> 
   <td> <p> [!DNL Jira] イシューの [!DNL Workfront] 右側のパネルに表示されます。<br>実際の値を持つカスタムフィールドのみがパネルに表示されます。<br></p> <p>メモ：カスタムフォームのセクションは、[!DNL Workfront] 管理者のアクセスレベルで表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>[!DNL Jira] イシューの [!DNL Workfront] 右側のパネルに表示されます。<br>[!DNL Jira] のイシュー<strong>[!UICONTROL Priority]</strong>フィールドは更新されません。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time]</td> 
   <td> <p>記録した時間に関するコメントが [!DNL Jira] のイシューの「<strong>[!DNL Workfront]</strong>」タブに追加されました。これには、時間を記録するユーザーと記録されるユーザーの名前が異なる場合に、それらの名前も含まれます。[!DNL Jira] の「<strong>[!UICONTROL Work log]</strong>」タブには時間が記録されません。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>[!DNL Jira] のイシューの「<strong>[!DNL Workfront]</strong>」タブにコメントが追加されました。[!DNL Jira] のイシューの「<strong>[!UICONTROL Comments]</strong>」タブには追加されません。</p> <p>メモ：2 つの既存のアイテムを手動でリンクすると、[!DNL Jira] にリンクする前に [!DNL Workfront] アイテムに追加されたコメントは [!DNL Jira] のイシューと同期しません。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!DNL Jira] のリンクされたアイテムの更新

主に [!DNL Jira] で作業している場合は、[!DNL Jira] の作業アイテムを更新すると、[!DNL Workfront] の対応する作業アイテムも更新されます。[!DNL Jira] で行っている更新を受け取るために、[!DNL Jira] のイシューにリンクされている [!DNL Workfront] アイテムの [!DNL Workfront] ライセンスを保有している必要はありません。

リンクされたアイテム間のフィールドを同期するように、[!DNL Workfront] 管理者が [!DNL Jira] の [!DNL Workfront] を設定していることを条件として、[!DNL Jira] で更新する特定のフィールドは、リンクされた [!DNL Workfront] アイテムでも更新されます。

次のリストは、リンクされたアイテムのどの [!DNL Jira] フィールドが [!DNL Workfront] フィールドと同期するかを示しています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>更新された [!DNL Jira] フィールド</strong> </th> 
   <th><strong>同期された [!DNL Workfront] フィールド/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>[!DNL Jira] のイシューステータスは、Workfront の次のステータス、または次のステータスと同等のステータスと同期します。</p> 
    <ul> 
     <li> <p>[!UICONTROL New]（[!UICONTROL NEW]）</p> </li> 
     <li> <p>[!UICONTROL In Progress]（[!UICONTROL INP]）</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete]（[!UICONTROL CLS]/[!UICONTROL CPL]）</p> </li> 
    </ul> <p>メモ：[!DNL Jira] ステータスは、適切なステータスに相当する最初の [!DNL Workfront] ステータスと同期します。</p> <p>[!DNL Workfront] のアイテムのステータスについて詳しくは、<a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">ステータスの作成または編集</a>を参照してください。</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>[!DNL Jira] での新しいドキュメントのアップロードに関するコメントが、[!DNL Workfront] のイシューまたはタスクの「[!UICONTROL Updates]」タブに追加されました。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> [!DNL Jira] の[!UICONTROL Due Date]の変更に関するコメントが、[!DNL Workfront] のイシューまたはタスクの「[!UICONTROL Updates]」タブに追加されました。</p> <p>メモ：[!DNL Workfront] のイシューまたはタスク上の日付は変更されません。</p> </td> 
  </tr> 
  <tr> 
   <td> [!DNL Workfront] の右側のパネル、または [!DNL Jira] のイシューの[!UICONTROL More]メニューから時間を記録します。<br></td> 
   <td> <p>時間数<br>[!DNL Workfront] のリンクされたアイテムに Jira に記録された時間数を追加することに加えて、時間の記録に関するコメントが [!DNL Workfront] のアイテムの「[!UICONTROL Updates]」タブに追加されました。</p> <p>リンクされた [!DNL Jira] のイシューの時間の記録について詳しくは、[!DNL Workfront] でその時間を記録する [!DNL Jira] ユーザーの更新を含め、<a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">リンクされた [!DNL Jira] アイテムと [!DNL Workfront] アイテムの時間の記録</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> コメント <br><br></td> 
   <td> <p>コメントは、「[!UICONTROL Setup]」タブの「[!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT]」セクションの「<strong>[!UICONTROL Comments]</strong>」設定が「<strong>[!UICONTROL Always]</strong>」である場合に、[!DNL Workfront] のイシューまたはタスクの「[!UICONTROL Updates]」タブに追加されます。</p> <p>[!DNL Jira] での Workfront の設定については、<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">設定：[!DNL Workfront for Jira]</a> を参照してください。</p> <p>リンクされた [!DNL Jira] イシューからのアイテムへのコメントについては、<a href="#comment-from-a-linked-jira-issue" class="MCXref xref">リンクされた [!DNL Jira] イシューからのコメント</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## リンクされた [!DNL Jira] イシューからの時間の記録

[!DNL Jira] で [!DNL Jira] アイテムに記録した時間は、[!DNL Jira] のどこで時間を記録したかに関係なく、リンクされた [!DNL Workfront] アイテムにも転送されます。\
[!DNL Workfront] パネルで Jira の時間を記録すると、その時間は [!DNL Workfront] にのみ記録されます。\
[!DNL Workfront] に記録した時間は、リンクされた [!DNL Jira] のイシューの時間には影響しません。

>[!NOTE]
>
>[!DNL Workfront] タスクにリンクされた [!DNL Jira] アイテムに時間が追加されると、[!DNL Workfront] の時間の[!UICONTROL 時間タイプ]は[!UICONTROL タスク時間]になります。[!DNL Workfront] イシューにリンクされた [!DNL Jira] アイテムに時間が追加されると、[!DNL Workfront] の時間の[!UICONTROL 時間タイプ]は[!UICONTROL 問題時間]になります。

[!DNL Jira] の「**[!DNL Workfront]**」タブと [!DNL Workfront] のアイテムの「**[!UICONTROL 更新]**」タブにコメントが追加され、時間が記録されます。\
時間は、[!DNL Workfront] アイテムの「**[!UICONTROL 時間数]**」タブにも表示されます。

* [リンクされた [!DNL Jira] アイテムと [!DNL Workfront] アイテムの時間を記録](#log-time-for-linked-jira-and-workfront-items)
* [ [!DNL Jira] から [!DNL Workfront] アイテムに時間を記録](#log-time-from-jira-to-a-workfront-item)

### リンクされた [!DNL Jira] アイテムと [!DNL Workfront] アイテムの時間を記録

[!DNL Workfront] アイテムにリンクされた [!DNL Jira] イシューから時間を記録でき、その時間は [!DNL Jira] イシューと [!DNL Workfront] アイテムの両方に記録されます。

>[!IMPORTANT]
>
>[!DNL Jira] で時間を記録しているユーザーが [!DNL Workfront] に存在しない場合、「**[!UICONTROL [!DNL Jira] ユーザーに&#x200B;*[!DNL Workfront] アカウントがない場合、[!DNL Workfront] にユーザーを自動的に作成]**」が「**[!UICONTROL &#x200B;常に&#x200B;]**」に設定されていれば、統合により Workfront に新しいアクティブユーザーが作成されます。このユーザーは [!DNL Workfront] ライセンスを所有していません。アクティブなユーザーを [!DNL Workfront] の作業アイテムに割り当てることはできますが、更新に含めることはできません。[!DNL Jira] からの [!DNL Workfront] ユーザーの自動作成の設定については、[設定： [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) を参照してください。

[!DNL Jira] のアイテムの時間を記録し、[!DNL Jira] と [!DNL Workfront] の両方に記録するには、次の手順に従います。

1. [!DNL Jira] にログインします。
1. [!DNL Workfront] アイテムにリンクされている [!DNL Jira] イシューに移動します。
1. **[!UICONTROL その他]**&#x200B;メニューを展開し、「**[!UICONTROL 作業の記録]**」をクリックします。

1. このイシューの作業に費やした時間を「**[!UICONTROL 消費時間]**」フィールドに指定します。次の期間を使用して時間を指定する必要があります。

   * [!UICONTROL 週数]（w）
   * [!UICONTROL 日数]（d）
   * [!UICONTROL 時間数]（h）

1. 続いて、「**[!UICONTROL 作業の説明]**」などの情報を時間エントリに追加したあと、「**[!UICONTROL ログ]**」をクリックします。\
   その時間が、[!DNL Jira] アイテムの「**[!UICONTROL 作業ログ]**」タブと、そのアイテムにリンクされている [!DNL Workfront] アイテムに追加されます。\
   時間エントリの作業説明は、[!DNL Workfront] で時間エントリのメモとして記録されます。

### [!DNL Jira] から [!DNL Workfront] アイテムに時間を記録

[!DNL Jira] イシューに時間を記録せずに、[!DNL Jira] イシューからリンクされた [!DNL Workfront] アイテムにのみ時間を記録できます。

1. [!DNL Jira] にログインします。
1. [!DNL Workfront] アイテムにリンクされている [!DNL Jira] イシューに移動します。

   [!DNL Workfront] アイテムの詳細が、イシューの右側の [!DNL Workfront] パネルに表示されます。

1. **[!UICONTROL 時間の記録]**&#x200B;アイコンをクリックします。

1. イシューについて記録する&#x200B;**[!UICONTROL 時間数]**&#x200B;と&#x200B;**[!UICONTROL 分数]**&#x200B;を指定します。

1. 「**[!UICONTROL 時間の記録]**」をクリックします。

   [!DNL Workfront] アイテムに時間が追加されます。

   この時間は、[!DNL Jira] イシューの「[!UICONTROL 作業の記録]」タブには追加されません。

## リンクされた [!DNL Jira] イシューからコメント {#comment-from-a-linked-jira-issue}

[!DNL Jira] で右側の [!DNL Workfront] パネルから [!DNL Jira] アイテムにコメントすると、そのコメントはリンクされた Workfront アイテムの「[!UICONTROL 更新]」タブにも追加されます。

[!DNL Jira] から [!DNL Workfront] アイテムにコメントするには、次の手順に従います。

1. [!DNL Jira] にログインします。
1. [!DNL Workfront] アイテムにリンクされている [!DNL Jira] イシューに移動します。

   [!DNL Workfront] アイテムの詳細が、イシューの右側の [!DNL Workfront] パネルに表示されます。

1. [!DNL Workfront] パネルまたは「**[!UICONTROL コメント]**」タブで&#x200B;**[!UICONTROL コメント]**&#x200B;アイコンをクリックします。

1. コメントを入力したあと、「**[!UICONTROL 送信]**」をクリックします。

   コメントが以下に追加されます。

   * [!DNL Jira] イシューの「**[!DNL Workfront]**」タブ
   * [!DNL Jira] イシューの「**[!UICONTROL コメント]**」タブ
   * リンクされた Workfront アイテムの「[**[!UICONTROL 更新]**」タブ
