---
product-area: projects
navigation-topic: manage-issues
title: イシューを編集
description: 自分が作成したイシューに関する情報や、他のユーザーとイシューを共有した場合は他のユーザーが作成したイシューに関する情報を編集できます。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '2506'
ht-degree: 100%

---

# イシューを編集

自分が作成したイシューに関する情報や、他のユーザーとイシューを共有した場合は他のユーザーが作成したイシューに関する情報を編集できます。

1 つのイシューを編集することも、リスト内の複数のイシューを編集することもできます。リスト内のイシューの編集について詳しくは、[リスト内のイシューの編集](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> <p>タスクまたはプロジェクトの「イシュー」セクションでイシューを編集する場合は、レビュー以上のライセンスが必要です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。自分のアクセスレベルでのイシューへのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">イシューへのアクセスの許可</a>を参照してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限を付与して、詳細エリアの次のフィールドを編集します。 </p>
   <ul>
   <li>説明</li>
   <li>ステータス</li>
   <li>重大度</li>
   </ul>
   <p>イシューに対する権限を管理して、詳細エリアまたは「イシューの編集」ボックスのすべてのフィールドを編集できるようにします。</p> <p> イシューに対する権限の付与について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>を参照してください。</p> <p>追加権限の要求については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権の要求</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者にお問い合わせください。

## イシューを編集する際の制限事項

いくつかの制限があり、イシューを編集できない場合があります。

* 「承認プロセス中」のイシューは編集できません。「承認保留中」のイシューに対してのみ、時間を記録したり、ステータスを更新したりできます。
* 完了、無効または承認保留中のステータスを持つプロジェクトのイシューに対するドキュメントの編集や追加は、Workfront 管理者またはグループ管理者がプロジェクト環境設定エリアでこの機能を有効にした場合にのみ行えます。プロジェクト環境設定について詳しくは、[システム全体のプロジェクト環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

## 単一のイシューの編集

イシューを編集するには、イシューの編集エリア、またはイシューの詳細エリアを使用します。次の手順では、イシューの編集ボックスでイシューを編集する方法を説明します。

1. **メインメニュー**&#x200B;に移動します。
1. 「**プロジェクト**」をクリックし、プロジェクトの名前をクリックして、プロジェクトを開きます。
1. （オプション）「**タスク**」をクリックし、タスクの名前をクリックして、タスクを開きます。
1. 左側のパネルで「**イシュー**」をクリックします。

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. （オプション）イシューに関する限定的な情報を編集するには、左側のパネルで「**イシューの詳細**」をクリックします。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者がレイアウトテンプレートをどのように変更したかに応じて、イシューの詳細エリアのフィールドが並べ替えられたり、表示されなかったりする場合があります。詳しくは、[レイアウトテンプレートを使用した詳細ビューのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

   「詳細」セクションの情報を編集するには、次の手順を実行します。

   1. （オプション）すべてのエリアを折りたたむには、右上隅の&#x200B;**すべて折りたたむ**&#x200B;アイコンをクリックします。
   1. （オプションおよび条件付き）領域が折りたたまれている場合、各領域の横にある&#x200B;**右矢印** ![](assets/right-pointing-arrow.png) をクリックして、編集する領域を展開します。
   1. （オプション）カスタムフォームを添付するには、**カスタムフォームを追加**&#x200B;フィールドにフォーム名を入力し、リストに表示されたフォームを選択して、「**変更を保存**」をクリックします。
   1. （オプション）概要およびカスタムフォームの情報を PDF ファイルに書き出すには、**書き出し**&#x200B;アイコン ![](assets/export.png) をクリックし、「**書き出し**」をクリックします。次の中から選択します。

      * すべてを選択（1 つ以上のカスタムフォームが添付されている場合にのみ表示）
      * 概要
      * 1 つまたは複数のカスタムフォームの名前

      PDF ファイルがお使いのコンピューターにダウンロードされます。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      詳しくは、[カスタムフォームとオブジェクトの詳細の書き出し](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)を参照してください。

   「イシューの詳細」セクションに表示されるフィールドの詳細を表示するには、下記に示す「イシューの編集」ボックスでイシューの編集を続けます。

1. イシューに関するすべての情報を編集するには、リストからイシューを選択し、リストの一番上の「**編集**」をクリックします。

   または

   リスト内のイシュー名をクリックし、イシュー名の横にある&#x200B;**詳細**&#x200B;メニュー、「**編集**」の順にクリックします。

   **イシューの編集**&#x200B;ダイアログボックスが表示されます。

   >[!IMPORTANT]
   >
   >編集リンクを表示するには、イシューに対する管理権限が必要です。

   すべてのイシューフィールドは、イシューの編集ボックスで使用でき、左側のパネルに表示されるエリアでグループ化されます。

1. 次のセクションのいずれかに情報を指定することを検討してください。

   * [イシュー名](#issue-name)
   * [概要](#overview)
   * [割り当て](#assignments)
   * [カスタムフォーム](#Custom%C2%A0F)
   * [設定](#settings)

   >[!NOTE]
   >
   >Workfront 管理者がレイアウトテンプレートをどのように設定したかに応じて、環境によってイシューの編集ボックスのフィールドが異なる場合があります。詳しくは、[レイアウトテンプレートを使用して詳細ビューをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。
   >
   >イシューを作成する際に、以下のセクションに一覧表示されるほとんどのフィールドは、新しいイシューボックスからもアクセスできます。フィールドが配置されているセクションは、新しいイシューボックスと一致していません。イシューの作成について詳しくは、[イシューを作成](../../issues/manage-issues/create-issues.md)を参照してください。

### イシュー名 {#issue-name}

1. 上記の説明に従って、イシューの編集を開始します。
1. 「**イシュー名**」をクリックします。

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. 「**イシュー名**」フィールドを更新します。
1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 概要 {#overview}

1. 上記の説明に従って、イシューの編集を開始します。
1. 「**概要**」をクリックします。

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. 以下の表のフィールドを更新または確認します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td> <p>イシューに関する追加情報を追加します。</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">「基本情報」セクション</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td> <p>イシューのステータスを選択します。イシューのステータスについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムイシューステータスのリストへのアクセス</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先度</td> 
      <td> <p>これは、イシューを優先順位付けできる視覚的なフラグです。</p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>なし</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p><strong>標準</strong> </p> </li> 
        <li> <p><strong>高</strong> </p> </li> 
        <li> <p><strong>緊急</strong> </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。優先順位の編集について詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">優先順位を作成およびカスタマイズ</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">重大度</td> 
      <td> <p>これは、イシューに記載されているイシューの重大度を示す視覚的なフラグです。重大度はイシューに特有のものです。次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: bold;">一時回避</p> </li> 
        <li> <p style="font-weight: bold;">混乱を招く</p> </li> 
        <li> <p style="font-weight: bold;">対処策のあるバグ</p> </li> 
        <li> <p style="font-weight: bold;">対処策のないバグ</p> </li> 
        <li> <p style="font-weight: bold;">致命的なエラー</p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクトの環境設定に応じて、重大度の名前が異なる場合があります。重大度の編集について詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">イシューの重大度を作成またはカスタマイズ</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>イシューに関する情報に関する web リンクを入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイプ</td> 
      <td> <p>プロジェクトマネージャーがプロジェクトのキューの詳細領域で選択したキューのプロパティに従って、イシューのタイプを指定できる場合があります。<b>タイプ</b>ドロップダウンメニューで次のオプションから選択します。 </p> 
       <ul> 
        <li> <p><strong>バグレポート</strong> </p> </li> 
        <li> <p><strong>変更依頼</strong> </p> </li> 
        <li> <p><strong>イシュー</strong> </p> </li> 
        <li> <p><strong>リクエスト</strong> </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクトの環境設定に応じて、イシューのタイプ名が異なる場合があります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プライマリ連絡先</td> 
      <td>デフォルトでは、イシューの作成者がプライマリの連絡先です。これを変更するには、Workfront でアクティブなユーザーの名前を入力し、リストから選択します。1 つのイシューのプライマリ連絡先は 1 つだけです。<br>プライマリ連絡先を変更しても、元のプライマリ連絡先には引き続き管理アクセス権が付与されます。イシューを共有する際は、イシューのアクセスボックスから手動でこのアクセスを削除する必要があります。

   <b>ヒント</b>

   <p>プライマリの連絡先ユーザーを追加する際には、アバター、ユーザーのプライマリの役割、メールアドレスに注意して、同じ名前のユーザーを区別してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。</p>
      <p> ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">ユーザーへのアクセス権の付与</a>を参照してください。</p>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コミット日時</td> 
      <td> <p>これは、イシューの割り当ての担当者がイシューが完了すると見積もる日付です。担当者のみがこのフィールドを編集できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定開始日</td> 
      <td>デフォルトでは、予定開始日はイシューが作成された日付と時刻です。イシューの<strong>予定開始日</strong>を更新できます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定完了日時</td> 
      <td> デフォルトでは、予定完了日はデフォルトの予定開始日から 24 時間です。デフォルトでは、イシューの期間は 1 日です。イシューの<strong>予定完了日</strong>を更新できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の開始日時</td> 
      <td>実際の開始日は、イシューのステータスを「<strong>処理中</strong>」に変更すると自動的に設定されます。イシューの<strong>実際の開始日</strong>を更新できます。必要に応じて、手動で日付を更新できます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の完了日時</td> 
      <td>「実際の完了日」は、イシューのステータスを「<strong>閉じる</strong>」または「<strong>解決済み</strong>」に変更すると自動的に設定されます。イシューの<strong>実際の完了日</strong>を更新できます。必要に応じて、手動で日付を更新できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">解決オブジェクト</td> 
      <td> <p>これは、イシューが別のオブジェクトによって解決されたかどうかを示します。ドロップダウンメニューから、このイシューをタスク、プロジェクト、または別のイシューのいずれで解決するかを選択し、このイシューを解決するタスク、プロジェクト、またはこのイシューの名前の入力を開始します。名前がリストに表示されたら、選択します。</p>

   <b>メモ</b>

   イシューを解決するオブジェクトを選択すると、イシューのステータスは解決オブジェクトのステータスにリンクされ、イシューで変更することはできません。オブジェクトの解決について詳しくは、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決および解決可能なオブジェクトの概要</a>を参照してください。

   <b>ヒント</b>

   システム管理者またはグループ管理者がイシューのカスタムヘッダーに「解決者」フィールドを追加すると、イシューに関連付けられた解決オブジェクトがある場合、フィールドは「イシューの解決」、「タスクの解決」、または「プロジェクトの解決」に変わります。

   このフィールドがイシューヘッダーに表示されている場合は編集できません。イシューヘッダーのカスタマイズについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ</a>を参照してください。
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">イシューの解決、タスクの解決、またはプロジェクトの解決</td> 
      <td>イシューを解決するイシュー、タスク、またはイシューのリンクされた名前。  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">これにより、次が解決されます。</td> 
      <td>アクセスしているイシューが解決されると完了する、イシューのリンクされた名前。  </td> 
     </tr>


   </tbody> 
   </table>





1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

#### 割り当て {#assignments}

1. 上記の説明に従って、イシューの編集を開始します。
1. 左側のパネルで「**割り当て**」をクリックします。

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. 「**ユーザー、役割、チームを検索**」をクリックして、タスクに割り当てるユーザー、役割、またはチームの名前の入力を開始し、リストに表示されたらクリックするか Enter キーを押します。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >ユーザーの名前に特殊文字が含まれている場合は、その特殊文字を検索フィールドに含める必要があります。

   >[!TIP]
   >
   >複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
   >
   >
   >ユーザー、担当業務、またはチームが非アクティブ化される前に割り当てられていた場合、それらは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
   >
   >* 作業アイテムをアクティブなリソースに再割り当てする。
   >* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。

1. （オプション）担当者の名前にポインタを合わせ、「**プライマリにする**」をクリックして、担当者がイシューのプライマリ担当者であるかどうかを示します。チームをイシューのプライマリ担当者にすることはできません。
1. 次のフィールドを更新します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">予定時間数</td> 
      <td> <p>これは、イシューの担当者がイシューを完了するのに実際にかかる時間です。イシューの予定時間数を入力します。<br></p> <p>メモ：イシューの予定時間数を変更しても、イシューの予定完了日は変更されません。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">割り当て先の役割</td> 
      <td> <p>個人を割り当て先として選択した場合は、「<strong>担当者の役割</strong>」ドロップダウンメニューから役割を選択します。これは、担当者がこのイシューで果たすことができる役割です。 </p> <p><b>ヒント</b>

   プロファイル内で各担当者に関連付けられている担当業務のみがドロップダウンメニューに表示されます。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### カスタムフォーム

1. 上記の説明に従って、イシューの編集を開始します。
1. 「**カスタムフォーム**」をクリックします。

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. 「**カスタムフォームを追加**」フィールドで、イシューに関連付けるカスタムフォームを選択します。このフィールドでカスタムフォームを選択できるようにするには、まずカスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。カスタムフォームの作成について詳しくは、[カスタムフォームを作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。1 つのイシューには、最大 10 個のカスタムフォームを追加できます。

1. （条件付き）カスタムフォームをイシューに添付した場合は、フォーム上の任意のフィールドを編集します。イシューを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront 管理者がカスタムフォーム内のセクションに権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰もが表示または編集できるわけではありません。カスタムフォームのセクション内のフィールドを編集する権限は、イシュー自体に対する権限によって異なります。カスタムフォームのセクションに対する権限の設定については、[カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。イシューの権限の設定については、[イシューの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)を参照してください。

1. 「**保存**」をクリックするか、次のセクションの編集に進みます。

### 設定 {#settings}

1. 上記の説明に従って、イシューの編集を開始します。
1. 「**設定**」をクリックします。

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   次の情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td> 
       <div> 
       <p>イシューに関連付ける承認プロセスを選択します。システムレベルの承認プロセスをイシューに関連付けるには、まず Workfront 管理者がそのプロセスを定義する必要があります。承認プロセスへの管理アクセス権を持つユーザー<span>は、グループ固有の承認プロセスを作成することもできます。</span>承認プロセスの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業アイテムの承認プロセスの作成</a>を参照してください。 </p> 
       <p>承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul> 
       <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
       <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。プロジェクトの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> <p>重要：プロジェクトのグループが変更されると、グループ固有の承認プロセスが 1 回限りの承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループや承認プロセスの変更が割り当て済みの承認プロセスに及ぼす影響</a>を参照してください。 </p> </li> 
       <li> <p>リクエストキューまたはキュートピックを作成する際にイシューに自動的に添付されるデフォルトの承認プロセスを定義できます。キューの詳細の更新については、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>を参照してください。キュートピックの作成については、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">キュートピックの作成</a>を参照してください。 </p> </li> 
       <li>イシューを一括編集する場合は、次のシナリオが存在します。 
       <ul> 
       <li><p>同じグループから複数のイシューを選択すると、このフィールドには、システムレベルとグループ固有の承認プロセスの両方が表示されます。</p></li> 
       <li><p>異なるグループから複数のイシューを選択すると、このフィールドには、システムレベルの承認プロセスのみが表示されます。</p></li> 
       <li><p>いずれかのイシューに 1 回限りの承認プロセスが添付されている場合は、選択したシステムレベルまたはグループレベルの承認プロセスに置き換えられます。 </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知</td> 
      <td> <p>このイシューに添付するリマインダー通知のチェックボックスをオンにします。イシューのすべてのリマインダー通知が表示されます。イシューでリマインダー通知を選択するには、まず Workfront 管理者がリマインダー通知を設定する必要があります。リマインダー通知の設定について詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

## イシューヘッダーでのイシューの編集（制限あり）

イシューヘッダーの限られた情報を編集することができます。

システム管理者またはグループ管理者は、イシューヘッダーに表示されるフィールドをカスタマイズできます。詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

![](assets/issue-header-350x19.png)

デフォルトでは、次のフィールドがイシューヘッダーに含まれています。

* イシュー名
* 完了率
* 割り当て
* 予定完了日時
* ステータス
* 現在の承認プロセスで承認者として設定されている場合、承認の決定を行う
