---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーの操作
description: ワークロードバランサーを使用して、リソースの空き時間を把握し、作業をユーザーに割り当てます。この記事では、ワークロードバランサーのビューを更新したり、ワークロードバランサーを操作するために利用できるアイコンや設定の使用方法について詳しく説明します。
author: Lisa
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '4146'
ht-degree: 89%

---

# ワークロードバランサーの操作

Adobe Workfront のワークロードバランサーを使用すると、空き時間に基づいて作業をユーザーに割り当てることができます。この記事では、設定やオプションを使用して、ワークロードバランサーを操作し、自分に関連する情報を表示する方法について説明します。この記事で紹介されている他の記事では、ワークロードバランサーを使用してリソースや、リソースの作業の配分を管理する方法について説明しています。

ワークロードバランサーは、Adobe Workfront の複数の領域で使用できます。操作方法はすべての領域で同様です。

ワークロードバランサーの場所について詳しくは、[ワークロードバランサーの検索](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer.html?lang=ja)を参照してください。


## アクセス要件

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
<td><p>Current license: Standard </p>
    Or 
<p>Legacy license:</p>
    <ul>
    <li><p>Plan, when using the Workload Balancer for a team or in the Resourcing area </p></li>
    <li><p>Work, when using the Workload Balancer of a project </p></li>
    </ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>プラン、リソース領域でワークロードバランサーを使用する場合</p>
   <p>ワーク、チームまたはプロジェクトのワークロードバランサーを使用する場合</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の項目に対する表示以上のアクセス権：</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>イシュー</p> </li> 
    </ul> <p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、「<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシューに対する表示またはそれ以上の権限 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## ワークロードバランサーでの項目の表示に関する考慮事項

ワークロードバランサーを表示する際は、次の項目を考慮してください。

* ワークロードバランサーは、割り当てに応じて、2 つの別々のエリアに作業アイテムを表示します。作業アイテムとユーザーは、次の領域に表示されます。

   * **未割り当て作業**：割り当てがない項目、あるいは担当業務またはチームにのみ割り当てられている項目。
   * **割り当てられた作業**：1 人以上のユーザーに割り当てられている項目。割り当てられた項目は、割り当てられたユーザーの名前の下に表示されます。

  >[!NOTE]
  >
  >* ジョブの役割またはチームに割り当てられ、さらにユーザーに割り当てられた作業項目は、「未割り当て作業」領域と「割り当てられた作業」領域の割り当てられたユーザーの名前の両方に表示されます。
  >* ユーザーに割り当てられ、ジョブロールがアイテムの主な担当者として選択されているジョブロールに対して、「未割り当ての作業」領域に表示されます。
  >* 複数のユーザーに割り当てられた作業項目は、「割り当てられた作業」領域の割り当てられたユーザーの名前のすべてに表示されます。

  詳細は、「ワークロード・バランサの割り当て領域」( [ワークロードバランサーでの作業割り当ての概要](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

* ある期間、プロジェクトにタスクがない場合、その時間のプロジェクトレベルのバーは空白になります。

  ![期間中にタスクがないプロジェクト](assets/wb-no-tasks-in-time-period.png)

* 特定の項目を表示する権限がない場合は、「**アクセス不能な作業アイテム**」または「**アクセス不能なプロジェクト**」として表示されます。

  ![アクセスできない作業項目](assets/wb-inaccessible-work-items.png)

* 作業アイテムの名前が左側に、タイムラインが右側に表示されます。
* 各作業アイテムの予定時間数の合計は、作業アイテム名の右側と、作業アイテムのタイムラインを表すバーの左側に表示されます。
* 各プロジェクトの予定時間数の合計は、プロジェクト名の右側と、プロジェクトのタイムラインを表すバーの左側に表示されます。

  プロジェクトの予定時間数の情報は、ワークロードバランサーにリストされているすべての項目の予定時間数の合計であり、プロジェクトの予定時間数の合計ではありません。

ワークロードバランサーの情報の表示について詳しくは、次の記事も参照してください。

* [ワークロードバランサーの使用場所](../workload-balancer/locate-workload-balancer.md)
* [ワークロードバランサーでの情報のフィルタリング](../workload-balancer/filter-information-workload-balancer.md)
* [リンクによるワークロードバランサーの共有](../workload-balancer/share-link-for-workload-balancer.md)
* [概要を使用したワークロードバランサーでの作業項目の更新](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

ワークロードバランサーを使用したリソース管理については、次の記事も参照してください。

* [ワークロードバランサーでの作業割り当ての概要](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer.html?lang=ja)
* [ワークロードバランサーでのユーザー割り当ての管理](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer.html?lang=ja)


## リソース領域での複数のプロジェクトを対象とするワークロードバランサーのナビゲーション

ワークロードバランサーのナビゲーションは、どの領域からアクセスする場合も同様です。

以下の各節では、ワークロードバランサーで複数のプロジェクトの情報を表示する方法について説明します。

ワークロードバランサーの様々な設定やオプションを調整して、自分にとって最も意味のある時間枠内で注目すべき情報を表示できます。

表示に適用する設定を選択したら、ワークロードバランサーは、任意のブラウザーまたはデバイスからアクセスされるたびにこれらの設定を記憶します。

### リソース領域での複数のプロジェクトを対象とするワークロードバランサーへのアクセス

複数のプロジェクトを対象とするワークロードバランサーをナビゲートするには、次の手順に従います。

1. Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、「**リソース**」をクリックします。
1. 左パネルの「**ワークロードバランサー**」をクリックします。

   ![ワークロードバランサー](assets/nwe-balancer-global.png)

   ワークロードバランサーでは、現在の週から始まる作業割当情報を次の 2 つの領域に表示します。

   * **未割り当て作業**&#x200B;領域には、次の作業項目が表示されます。

      * 役割やチームに割り当てられた作業項目（タスクとイシュー）または未割り当ての作業項目が、フィルターの適用後に表示されます。
未割り当て作業領域には、デフォルトでは作業項目は表示されません。フィルターを使用して、自分に関係のある情報をこの領域に表示することをお勧めします。

        フィルターの使用については、[ワークロードバランサーでの情報のフィルタリング](../workload-balancer/filter-information-workload-balancer.md)を参照してください。

      * 「プロジェクトでグループ化」設定を有効にした場合にのみ、プロジェクトが表示されます。詳しくは、この記事の[表示のカスタマイズ](#customize-the-view)の節を参照してください。

   * **割り当てられた作業**&#x200B;領域には、次の作業項目が表示されます。

      * デフォルトで、システム内のアクティブなユーザーがすべて、この領域に表示されます。フィルターを使用して、この領域に表示される情報の量を制限することをお勧めします。ユーザーが項目に割り当てられている場合は、その作業項目もユーザー名の下に表示されます。

      * 少なくとも 1 人のユーザーに割り当てられているタスクとイシューが、ユーザー名の下に表示されます。

        割り当てられた作業領域でユーザー名の下に表示される作業項目は、次の基準に従って下記の順に並べ替えられます。

         1. 予定開始日（古い順）
         1. 予定完了日（古い順）
         1. プロジェクト名のアルファベット順（最初の 2 つの基準が複数の作業項目で同じ場合のみ）

            >[!TIP]
            >
            >* プロジェクトの並べ替えは、「プロジェクト並べ替え基準」設定からオプションを選択することでカスタマイズできます。
            >
            >* プロジェクトは、「プロジェクトでグループ化」設定を有効にした場合にのみ表示されます。
            > 
            >設定のカスタマイズについては、この記事の「[表示のカスタマイズ](#customize-the-view)」の節を参照してください。

1. （オプション） **フィルター** アイコン ![フィルターアイコン](assets/filter-icon.png) （内） **割り当てられた作業** 「 」領域で、「 **デフォルトのフィルター** （内） **推奨** 領域を選択します。

   デフォルトのフィルターを適用すると、任意のチームに属するユーザーとその作業項目が表示されます。このフィルターのコピーを編集できます。

   >[!TIP]
   >
   >デフォルトのフィルターは、リソース領域のワークロードバランサーでのみ使用できます。

1. 引き続き次の手順に従って、ワークロードバランサーをナビゲートします。

   * [ワークロードバランサーでの時間枠の選択](#select-a-time-frame-in-the-workload-balancer)
   * [表示のカスタマイズ](#customize-the-view)
   * [作業項目の割り当てとユーザー割り当ての調整](#assign-work-items-and-adjust-user-allocations)
   * [割り当てのグラフ表示](#view-allocations-in-a-chart)

### ワークロードバランサーでの時間枠の選択

1. この記事の[リソース領域での複数のプロジェクトを対象とするワークロードバランサーへのアクセス](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節に従って、**リソース**&#x200B;領域でワークロードバランサーにアクセスします。

   ワークロードバランサーには、現在の週から始まる作業割当情報が表示されます。

1. 作業項目のタイムラインが画面の表示限度を超える場合、すべてのタイムラインを表示するには、水平スクロールを使用します。
1. 次をクリック： **後ろまたは前に** アイコン ![戻るアイコンと進むアイコン](assets/back-and-forward-icons.png) 左上隅でタイムラインに移動し、「 **今日** 現在の週に戻る
1. ツールバーの&#x200B;**時間枠ドロップダウンメニュー**&#x200B;をクリックし、表示する期間の開始日をクリックします。デフォルトでは、カレンダーで選択された最初の週が移動先の週になります。

   ![カレンダーの選択](assets/calendar-date-picker-wb.png)

1. 次のオプションから、ワークロードバランサーに一度に表示する週数を選択します。
   * 1 週間
   * 2 週間
   * 4 週間. これはデフォルトの設定です。
   * 6 週間
   * 3 か月

   ![週を選択](assets/3-months-12-weeks-drop-down-wb.png)

1. ツールバーで次のオプションのいずれかをクリックすると、様々な時間枠別に情報が表示されます。
   * **日**：デフォルトでは、今日の日付から 4 週間分の情報を日別に表示します。
   * **週**：4 週間の情報を週別に表示します。
   * **月**：3 か月間の情報を月別に表示します。

1. 以降の節で説明するように、引き続きワークロードバランサーをナビゲートします。

### 表示をカスタマイズ

1. **リソース**&#x200B;エリアでワークロードバランサーにアクセスします。この記事の[リソースエリアでの複数のプロジェクト用のワークロードバランサーへのアクセス](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)を参照してください。

   作業アイテムの名前は、ワークロードバランサーの左側にリストされ、右側のバーで表示されます。バーの長さは、作業アイテムのタイムラインを表します。

1. （オプションおよび推奨）「未割り当て」および「割り当て済み」の作業エリアのフィルターを使用して、関連する作業アイテムまたはユーザーのみを表示します。

   詳しくは、[ワークロードバランサーの情報をフィルタリング](../workload-balancer/filter-information-workload-balancer.md)を参照してください。

   デフォルトでは、青いバーはプロジェクトとタスクのタイムラインを表し、栗色のバーはイシューを表します。

   プロジェクトに合わせてカラーテーマを選択すると、プロジェクトとタスクのバーの色を変更できます。詳しくは、この手順を引き続きお読みください。

   「割り当てられた作業」エリアの作業アイテムは、次の基準に従って、プロジェクトごとに次の順序で並べ替えられます。
   1. 予定開始日（古い順）
   1. 予定完了日（古い順）
   1. プロジェクト名のアルファベット順（最初の 2 つの基準が複数の作業項目で同じ場合のみ）

1. 「未割り当て」エリアまたは「割り当て済み」エリアの左側にある&#x200B;**右向き矢印**&#x200B;をクリックすると、プロジェクト名の下（「未割り当て」エリア内）およびユーザー名の下（「割り当て済み」エリア内）のすべての項目を展開できます。

   >[!TIP]
   >
   >作業アイテムは、「プロジェクト別にグループ化」設定を有効にした場合にのみ、「未割り当て」エリアのプロジェクト名の下に表示されます。

1. 「未割り当て」エリアまたは「割り当て済み」エリアの左側にある&#x200B;**下向き矢印**&#x200B;をクリックすると、プロジェクト名の下（「未割り当て」エリア内）およびユーザー名の下（「割り当て済み」エリア内）のすべての項目を折りたためます。

1. 左パネルとタイムラインエリアの間にある&#x200B;**分離線**&#x200B;をドラッグ＆ドロップして、左パネルのサイズを調整します。

   ![分離線](assets/wb-adjust-panel-size.png)

1. 次をクリック： **設定** アイコン ![設定アイコン](assets/settings-gear-icon.png).

   右側に設定パネルが表示されます。

   ![設定パネル](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   以下に表示されているオプションから選択して、ワークロードバランサーで表示する情報を更新し、設定ボックスの右上にある **X アイコン** をクリックしてボックスを閉じます。

   * **プロジェクト別にグループ化**：このオプションを選択すると、「未割り当て」および「割り当て済み」作業エリアの項目がプロジェクト別にグループ化されます。これはデフォルトで選択されています。

   * **イシューの時間を含める**：このオプションを選択すると、ユーザーに割り当てられたイシューが「割り当てられた作業」エリアのユーザー名に表示され、ユーザーに割り当てられていないイシューが「未割り当ての作業」エリアに表示されます。イシューの予定時間数は、プロジェクトおよび「割り当てられた作業」エリアのユーザーの予定時間数にカウントされます。
   * **見込日を表示**：このオプションを選択すると、予定タイムラインに加えて、作業アイテムの見込みタイムラインが表示されます。次の点に注意してください。
      * プロジェクト、タスク、イシューの見込みタイムラインは、タスク、イシュー、プロジェクトバーの上に濃い青色の線で表示されます。
      * 以下に説明するように、カラーテーマを更新した場合でも、予定タイムラインの外側にある見込みタイムラインは、薄い青色で表示されます。
      * 表示するアクセス権がない項目の予定タイムラインは、下に線が付いた薄いグレーで表示されます。
      * タスクまたはイシューが予定完了日より前に完了すると、残りの日数に割り当てられた数値に取り消し線が引かれ、ユーザーの割り当てにはカウントされません。これは、「見込日を表示」設定と「割り当てを表示」アイコンの両方が有効な場合にのみ表示されます。

     >[!TIP]
     >
     >選択した時間枠内に、予定または（必ずしも両方が同時に発生するわけではない）見込みタイムラインが発生すると、ワークロードバランサーに作業アイテムが表示されます。

   * **完了した作業の表示**：このオプションを有効にすると、完了したタスクとイシューが「割り当てられた作業」エリアに表示されます。これはデフォルトで有効になっています。

     タスクまたはイシューが完了すると、タスクまたはイシューバーの右上隅に緑色のチェックマークアイコンが表示されます。プロジェクトの選択した時間枠のタスクまたはイシューが完了すると、同じアイコンがプロジェクトに表示されます。
   * **残り時間を表示**：これを有効にすると、Workfront には、ユーザーのスケジュールに基づいて、ユーザーが作業できる毎日の時間と、ユーザーの「割り当てられた作業」エリアで割り当てられている時間との差が表示されます。これはデフォルトで無効になっており、割り当てられた時間がデフォルトで表示されます。
   * 「**カラーテーマを選択**」セクションで、プロジェクトとタスクバーに使用する色を選択します。

     >[!TIP]
     >
     >カラーテーマを選択するための設定は、イシューバーの色には影響しません。イシューは常に栗色のバーで表示されます。

     次の中から選択します。
      * **デフォルト**：すべてのプロジェクトとその作業アイテムのバーの色は、青で表示されます。
      * **プロジェクト**：各プロジェクトとそのタスクに関連付けられたバーの色は、プロジェクト名に応じて変わります。そのプロジェクトに属するすべてのタスクは、プロジェクトと同じ色のバーで表示されます。プロジェクトのバーは、タスクと区別するために明るい色で表示されます。割り当てを表示しないことを選択した場合は、プロジェクトバーにプロジェクトアイコンも表示されます。
      * **プロジェクトステータス**：各プロジェクトとその作業アイテムに関連付けられたバーの色は、プロジェクトステータスの色に変わります。

        プロジェクトステータスは、プロジェクトのグループに関連付けられています。グループにグループ固有のステータスがない場合、作業アイテムのバーの色は、システムレベルのプロジェクトステータスの色になります。システムステータスとカスタムステータスの両方が表示されます。グループステータスについて詳しくは、[グループステータスの作成または編集](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。

   * 「**ユーザー割り当ての表示**」セクションで、次のいずれかを選択します。
      * **時間数**：割り当てられた時間を時間単位で表示します。これがデフォルトです。
      * **割合**：割り当てられた時間を使用可能な合計時間に対する割合で表示します。
   * 「**並べ替え環境設定**」セクションで、ワークロードバランサーでアイテムを並べ替える方法を選択します。次のオプションから選択します。
      * **プライマリの役割でのユーザーの並べ替え**：ユーザーは「割り当てられた作業」エリアでプライマリの役割のアルファベット順に表示されます。
      * **ユーザーをアルファベット順に並べ替え**：ユーザーは「割り当てられた作業」エリアでファーストネームのアルファベット順に表示されます。
      * **プロジェクトを並べ替え**：プロジェクトは「未割り当ての作業」エリアまたは「割り当てられた作業」エリアで、ドロップダウンメニューから選択したプロジェクトフィールドのアルファベット順に表示されます。

   >[!TIP]
   >
   >プロジェクトで並べ替えをできるのは、「プロジェクトでグループ化」の設定が有効になっている場合のみです。それ以外の場合は、この設定は淡色表示になります。

1. （オプションおよび条件付き）カラーテーマを「プロジェクトステータス」に変更する場合、左側のプロジェクト名にカーソルを合わせるとプロジェクトステータスが表示されます。

   ![プロジェクトステータスのツールチップ](assets/hover-over-project-status-tooltip-350x115.png)

### 作業項目の割り当てとユーザー割り当ての調整

1. リソースエリアのワークロードバランサーにアクセスします。詳しくは、この記事の[リソースエリアの複数のプロジェクト用のワークロードバランサーへのアクセス](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)を参照してください。
1. 次をクリック： **割り当てアイコンを表示** ![割り当てアイコンを表示](assets/show-allocations-icon-small.png) ：作業項目の日次または週次の計画時間を表示します。

   これにより、作業アイテムのバーの名前が、「未割り当ての作業」エリアと「割り当てられた作業」エリアの日次または週次の予定時間数に置き換えられます。この設定は、デフォルトで無効になっています。

   配分超過を示す日は赤で表示されます。

   >[!TIP]
   >
   >* 「割り当てを表示する」オプションは、プロジェクト、タスク、イシュー、アクセスできないアイテムに対して表示される内容にのみ影響します。ユーザーの日次の予定時間数はデフォルトで表示され、非表示にすることはできません。
   >* プロジェクトの日次の予定時間数を表示するには、「プロジェクト別のグループ」設定を有効にする必要があります。
   >* ワークロードバランサーを週次で表示すると、表示される時間数は週次の予定時間数になります。


1. （オプション）ユーザー行の割り当て済み時間数にカーソルを合わせると、ユーザーのキャパシティと配分がわかります。キャパシティは、ユーザーのスケジュールに応じた空き状況です。

   ![割り当て済み時間の詳細](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. （オプション）**割り当てアイコンを非表示にする** ![](assets/show-allocations-icon-small.png) をクリックすると、作業アイテムのバーにタスクとイシューの名前が表示されます。
1. タスク名またはイシュー名の右にある&#x200B;**その他のメニュー**&#x200B;アイコン ![](assets/more-icon.png) をクリックして、以下のオプションのいずれかをクリックします。

   ![その他のメニュー](assets/more-menu-right-of-task-350x104.png)

   * 「**割り当て先:**」をクリックしてから、「**担当者、役割、またはチームの検索**」フィールドに作業アイテムを割り当てるユーザー、役割、チームの名前を入力します。

     次のショートカットを使用して、タスクやイシューを割り当てることもできます。

      * Windows の場合：Ctrl キーを押しながらタスクまたはイシューバーをクリックします。
      * Mac の場合：Cmd キーを押しながらタスクまたはイシューバーをクリックします。

     ワークロードバランサーでユーザーに作業アイテムを割り当てる方法について詳しくは、[ワークロードバランサーでの作業割り当ての概要](../workload-balancer/assign-work-in-workload-balancer.md)を参照してください。

     >[!TIP]
     >
     >お使いの環境で Workfront 管理者またはグループ管理者が委任を有効にしている場合は、「割り当て」タブを使用して、ユーザーをタスクまたはイシューに割り当てます。作業の委任について詳しくは、[タスクとイシューの委任を管理](../../manage-work/delegate-work/how-to-delegate-work.md)を参照してください。

   * 「**割り当てを編集する**」。そのユーザーの日次または週次の割り当てを編集します。ユーザー割り当ての管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

   * **概要を開く**. 右側に概要パネルが開きます。「割り当て」フィールドをクリックしてから、「**担当者、役割、またはチームの検索**」フィールドに作業アイテムを割り当てるユーザー、役割、チームの名前を入力します。詳しくは、この記事のセクション[タスクとイシューに関する詳細情報を表示](#display-more-information-about-tasks-and-issues)を参照してください。

1. （オプション）作業項目のバー内でユーザーの日次または週次の配分をダブルクリックして、割り当てられた時間数を編集し、 **保存** アイコン ![保存アイコン](assets/save-allocations-wb.png) 割り当てまたは **キャンセル** アイコン ![キャンセルアイコン](assets/cancel-allocations-wb.png) 調整した配分を削除します。

   >[!TIP]
   >
   >保存アイコンとキャンセルアイコンは、タスクまたはイシューのタイムラインバーの端に表示されます。
   >
   >![手動割り当てを保存またはキャンセル](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   ユーザー割り当ての管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

1. 「**一括割り当て**」をクリックして、作業アイテムを一括で割り当てます。

   詳しくは、[ワークロードバランサーを使用して作業を一括で割り当てる](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md)を参照してください。
1. **未割り当ての作業**&#x200B;エリアまたはユーザーから項目をドラッグして、別のユーザー上にドロップして割り当てます。

   詳しくは、[ドラッグ&amp;ドロップによりワークロードバランサーで作業を割り当てる](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)を参照してください。

### 割り当てのグラフ表示

日次数または週次数で割り当てを表示する代わりに、グラフで表示できます。

1. この記事の[リソースエリアの複数のプロジェクト用のワークロードバランサーへのアクセス](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節で説明されるように、リソースエリアのワークロードバランサーにアクセスします。
1. 次をクリック： **グラフアイコン** ![グラフアイコン](assets/user-allocation-chart-icon.png) をクリックして、ユーザーの配分をグラフ形式で表示します。

   ユーザーの割り当てが超過する日は、赤色のブロックで表示され、ユーザーの割り当てが過少する日または容量は、青色のブロックで表示されます。

   ブロックのサイズは、割り当ての量を示します。ボックスが大きいほど、その日または週の作業アイテムに割り当てられる時間が多くなります。

   ![グラフとしてのユーザーの配分](assets/wb-allocation-as-chart.png)

### タスクとイシューに関する詳細情報を表示する

ワークロードバランサーのタスクとイシューに関する詳細を表示できます。

1. この記事の[リソースエリアの複数のプロジェクト用のワークロードバランサーへのアクセス](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節で説明されるように、リソースエリアのワークロードバランサーにアクセスします。
1. 概要パネルに詳細情報を表示するには、次のいずれかの操作を行います。

   * タスクまたはイシューのバーをクリックして、右側の概要パネルを開きます。
   * **概要を開く**&#x200B;アイコン ![](assets/summary-panel-icon.png) をクリックし、タスクまたはイシューのバーをクリックして、概要パネルを開きます。
   * タスクまたはイシューの右側にある&#x200B;**その他**&#x200B;メニューをクリックして、「**概要を開く**」をクリックします。

   ワークロードバランサーの概要でタスク情報を更新する方法について詳しくは、[概要を使用してワークロードバランサーの作業アイテムを更新する](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)を参照してください。

1. タスクまたはイシューの名前の上にポインタを合わせると、タスクまたはイシューの詳細が表示されます。タスクまたはイシューの上に次の情報が表示されるボックスです。

   * タスクまたはイシューの名前。
   * プロジェクトの名前。
   * 予定開始日と完了日。
   * 予定時間数。
   * タスクの場合は、先行の番号。
   * タスクには、ボックスの上隅にタスクが作業可能かどうかを示すインジケーターが表示されます。

   ![タスクの詳細](assets/task-bar-hover-over-detail-wb.png)

1. 左側の作業アイテムの名前をクリックしてアクセスします。作業アイテムが新しいブラウザーのタブで開きます。

### ワークロードバランサーを全画面表示する

1. この記事の[リソースエリアの複数のプロジェクト用のワークロードバランサーへのアクセス](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節で説明されるように、リソースエリアのワークロードバランサーにアクセスします。

1. 次をクリック： **全画面表示** アイコン ![全画面表示アイコン](assets/full-screen.png) ワークロードバランサーをフルスクリーンで表示します。

   ワークロードバランサーが画面全体に表示されます。ブラウザーウィンドウとタブは、表示から除外されます。

1. 次をクリック： **全画面を終了** アイコン ![全画面表示を終了アイコン](assets/exit-full-screen.png) をクリックしてデフォルトの画面に戻り、ブラウザ・タブ内にワークロード・バランサを表示します。


## チームのワークロードバランサーの操作

チームのワークロードバランサーの操作は、複数のプロジェクトに対するワークロードバランサーの操作方法と似ています。詳しくは、この記事の[複数のプロジェクトに対するワークロードバランサーの操作](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節を参照してください。

1. 次をクリック： **メインメニュー** アイコン ![メインメニュー](assets/main-menu-icon.png)を選択し、次に **チーム**.
ホームチームのページがデフォルトで表示されます。
1. 左側のパネルの「**ワークロードバランサー**」をクリックします。チームのワークロードバランサーは、デフォルトで表示される必要があります。

   ![チームのワークロードバランサー](assets/nwe-balancer-team-350x172.png)

   チームのワークロードバランサーには、デフォルトで次の情報が表示されます。

   * **未割り当ての作業**&#x200B;エリア：チームまたはチームと担当業務に割り当てられた作業アイテム、ユーザーに割り当てられていない作業アイテム。
   * **割り当てられた作業**&#x200B;エリア：ユーザーに割り当てられた作業アイテムは、ユーザー名の下に表示されます。

1. この記事の[リソース領域での複数のプロジェクトを対象とするワークロードバランサーのナビゲーション](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節に従って、引き続き、チームのワークロードバランサーをナビゲートします。

## 単一プロジェクトのワークロードバランサーのナビゲーション

1. 次をクリック： **メインメニュー** アイコン ![メインメニュー](assets/main-menu-icon.png)を選択し、次に **プロジェクト**.
1. プロジェクトの名前をクリックして、プロジェクトページを開きます。
1. 左側のパネルの&#x200B;**ワークロードバランサー**&#x200B;をクリックします。「**さらに表示**」をクリックしてから&#x200B;**ワークロードバランサー**&#x200B;をクリックする必要がある場合があります。

   ![プロジェクトのワークロードバランサー](assets/nwe-balancer-project-350x152.png)

   プロジェクトのワークロードバランサーには、デフォルトで次の情報が表示されます。

   * **未割り当て作業**&#x200B;領域内：プロジェクトの作業項目のうち、役割またはチームに割り当てられ、ユーザーに割り当てられていないもの。
   * **割り当てられた作業**&#x200B;領域内：プロジェクトの作業項目のうち、少なくとも 1 人のユーザーに割り当てられているもの。

   フィルターを使用して、自分にとって重要なユーザーのみを表示することをお勧めします。

   例えば、自分のチームまたはグループに属するユーザーのみを表示することを検討します。詳しくは、[ワークロードバランサーでの情報のフィルタリング](../workload-balancer/filter-information-workload-balancer.md)を参照してください。

1. （オプション） **フィルター** アイコン ![フィルターアイコン](assets/filter-icon.png) 「割り当てられた作業」領域で、 **このプロジェクトの作業項目** オプションを **推奨** フィルターパネルの領域。 このフィルターは、デフォルトでは選択されていません。

   このオプションを選択すると、選択したプロジェクトのユーザーに割り当てられた項目のみが表示されます。

   このオプションを選択しない場合、アイテムが属しているプロジェクトに関係なく、プロジェクトのユーザーに割り当てられたすべての項目が表示されます。

1. （オプションおよび推奨）割り当てられた作業領域にフィルターを適用して、ユーザーが重要で、プロジェクトの項目に割り当てられていない可能性のあるユーザーを表示し、 **すべてのユーザーを表示** アイコン ![すべてのユーザーを表示アイコン](assets/show-all-users-icon-project-workload-balancer.png).

   すべてのユーザーを表示することで、プロジェクトの作業や他の役割にまだ割り当てられていない Workfront 内のすべてのユーザーを表示できます。

   最初にフィルターを適用して、表示するユーザーの数を減らすことができます。

   例えば、まず自分のチームまたはグループに属しているユーザーをフィルタリングして抜き出し、次にそれらのユーザーをすべて表示するといった具合です。

   フィルターの作成方法については、[ワークロードバランサーでの情報のフィルタリング](../workload-balancer/filter-information-workload-balancer.md)を参照してください。

   >[!NOTE]
   >
   > 「すべてのユーザーを表示」オプションは、プロジェクトのワークロードバランサーでのみ使用できます。

1. （オプション） **ロールの割り当てを表示** アイコン ![役割割り当てアイコンを表示](assets/show-role-allocation-icon.png).

   役割の配分パネルが表示されます。

   プロジェクトの担当業務に関連付けられている予定時間数と、シナリオプランナからプロジェクトにリンクされたイニシアチブに関連付けられている担当業務に関する情報を表示できます。

   詳しくは、[プロジェクトとイニシアチブ間でのリソース割り当て調整の概要](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)を参照してください。


   >[!NOTE]
   >
   >組織が Workfront シナリオプランナのライセンスを購入していない場合は、イニシアチブの担当業務情報を表示できません。この場合は、プロジェクトの担当業務に関連付けられている予定時間数のみ表示できます。詳しくは、[シナリオプランナの使用に必要なアクセス権](../../scenario-planner/access-needed-to-use-sp.md)を参照してください。

1. この記事の[複数のプロジェクトを対象とするワークロードバランサーのナビゲーション](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area)の節に従って、引き続き、プロジェクトのワークロードバランサーをナビゲートします。

<!--old content below - this used to be a one-large-procedure article - outdated, and rewrote it above with several smaller procedures: 

# Navigate the Workload Balancer

<!-drafted note for 22.4 release: remove all production/ preview references at Prod release>

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

Use the Workload Balancer to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the Workload Balancer.

>[!NOTE]
>
>The Workload Balancer is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the Workload Balancer for scheduling your resources.

The Workload Balancer is available in multiple areas of Adobe Workfront. Navigating it is similar in all areas. This article describes how to navigate the Workload Balancer for multiple projects in the Resourcing area. For more information about where the Workload Balancer is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

For information about managing resources using the Workload Balancer, also consider reading the following articles:

* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in all areas in the Production environment</p>
   <p><span class="preview">Work, when using the Workload Balancer of a project, in the Preview environment</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for viewing items in the Workload Balancer

Consider the following when viewing the Workload Balancer:

* Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.
* Mousing over a task or an issue displays the following additional information about the task or issue:

  * Project name

  * Task or issue name

  * Parent task

  * Planned Start and Completion Dates

  * Number of Planned Hours

  * Ready to start or Not ready status

  ![task-pop-up-with-additional-info-in-workload-balancer](assets/task-pop-up-with-additional-info-in-global-wb.png)

* When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color.

  ![](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* When you don't have permissions to see certain items, they display as **Inaccessible work items** or **Inaccessible projects**.

  ![](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* The names of the work items display on the left and within the timeline selected on the right. 
* The total of Planned Hours for each work item displays to the right of the name of the work items on the left. 
* The total of the Planned Hours for each project displays to the right of the name of the project on the left.

  The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project.

## Overview of the Unassigned Work and Assigned Work areas

The Workload Balancer displays work items in two separate areas, depending on their assignments.

The two areas of the Workload Balancer display the following information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks <span class="preview">and issues</span> unassigned to users. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area.  </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the Workload Balancer

You can update the view in the Workload Balancer to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the Workload Balancer remembers these settings every time you access it from any browser or device.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Resourcing**.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the Workload Balancer within their respective timelines. By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.

   >[!TIP]
   >
   >You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure.

   The work items that display under the name of users in the Workload Balancer are sorted by the following criteria, in this order:

   1. Planned Start Date (oldest first)
   1. Planned Completion Date (oldest first)
   1. Alphabetical by project (only when the first two criteria are identical for multiple work items)

1. Click the right-pointing arrow to the left of the Unassigned or Assigned areas to expand all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Click the down-pointing arrow to the left of the Unassigned or Assigned areas to collapse all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Use the horizontal scroll to navigate the timelines of work items that extends beyond the limits of the screen. 
1. Use the vertical scroll to display additional users and work items. 
1. Drag and drop the separation line between the left panel and the timeline areas to adjust the size of the left panel.

   ![](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to select the type of information to display in the Workload Balancer.

   For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md). 

1. Click the right-pointing arrow next to **Unassigned Work** to expand this area or the down-pointing arrow to collapse it.

   >[!TIP]
   >
   >No items display in this area by default. You must apply a filter to view unassigned work items.

1. Drag and drop the separation line between the **Unassigned Work** and **Assigned Work** areas to adjust their size.

   ![](assets/modern-scheduler-separation-line-between-areas-350x278.png)

1. Click the back or forward icons ![](assets/back-and-forward-icons.png) to navigate the timeline, then click **Today** to return to the current week. 

1. Click the **time frame drop-down menu** on the toolbar, then click the beginning date of the period you want to display. By default, the first week selected on the calendar is the week you navigated to.

   ![](assets/calendar-date-picker-wb.png)


1. Click one of the following options in the toolbar to display information by different time frames:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Day</td> 
      <td>Displays information by day for four weeks starting with today's date, by default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Week</td> 
      <td>Displays information by week for four weeks. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Month</td> 
      <td> <p><span>Displays information by month for three months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Select the number of weeks you want to display at one time in the Workload Balancer from the following options:

   * 1 week
   * 2 weeks
   * 4 weeks. This is the default setting.
   * 6 weeks
   * 3 months
   ![](assets/3-months-12-weeks-drop-down-wb.png)     

1. Click the **Settings** icon ![](assets/settings-gear-icon.png).

   The Settings panel displays.

   ![](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Select from the options listed below to update the information you view in the Workload Balancer, then click the **X icon** in the upper-right of the Settings box to close it.

   * **Group by Project**: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default.

     ![](assets/group-by-project-350x530.png)

   * **Include hours from issues**: When this is selected, issues assigned to users display under the user's name in the Assigned Work area <span class="preview">and issues that are not assigned to users display in the Unassigned Work area</span>. The Planned Hours from the issues count towards the Planned Hours for the project and for the user in the Assigned Work area. 

        ![](assets/issue-on-workload-balancer-350x20.png)

   
      * **Show Projected Dates**: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following:

         * The projected timeline of project, tasks, and issues displays as a dark blue line above the task, issue, and project bars.
         * The projected timeline that is outside of the planned timeline displays in light blue, even when you update the color theme, as described below.
         * The projected timeline for the items that you have no access to view displays in light gray with a line underneath.
         * When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled.

         ![](assets/task-issue-projected-timelines-350x91.png)

         >[!TIP]
         >
         >Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected.

   * **Show completed work**: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default.

     A green checkmark icon ![](assets/green-checkmark-icon.png) displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. 
   
   * **Show remaining time**: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default.

   * In the **Select color theme** section, select the color that you want for the project and task bars.  

      >[!NOTE]
      >
      >The setting for selecting the color theme  does not affect the color of the issue bars. Issues always display in a maroon-color bar. 


      Select from the following:

      * **Default**: The bars for all projects and their work items display in blue.  
      * **Project**: The bars associated with each project and its tasks change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. The project bars display in a lighter shade to distinguish them from the tasks. The project bars also include a project icon when choosing not to display allocations.
      * **Project Status**: The bars associated with each project and its work items change to the color of the status of the project.

        >[!TIP]
        >
        >* The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
        
   * In the **Display user allocation in** section, select from the following:

      * **Hours**: Displays allocated time as hours. This is the default. 
      * **Percentage**: Displays allocated time as a percentage of the total available time

   * In the **Sorting preferences** section, select how you want the items to be sorted in the Workload Balancer. Select from the following options: 

      * **Sort users by Primary Role**: Users display in the alphabetical order of their Primary Roles in the Assigned Work area.

      * **Sort users alphabetically**: Users display in the alphabetical order of their first names in the Assigned Work area.

      * **Sort projects by**: Select a project field from the drop-down menu to sort projects alphabetically by that field in the Unassigned or Assigned Work areas. 

      >[!TIP]
      >
      >You can sort by projects only when the Group by Project setting is enabled. Otherwise, this setting is dimmed.


1. (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project.

   ![](assets/hover-over-project-status-tooltip-350x115.png)

1. <span class="preview">(Conditional and recommended) In the Workload Balancer of a project, apply a filter in the Assigned Work area to display users that are important to you but might not be assigned to items on the project, then click the **Show all users** icon ![](assets/show-all-users-icon-project-workload-balancer.png). This displays other users in the system that are not yet assigned on the project. For information about how to build a filter, see [Manage filters in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md).</span>

 
   >[!TIP]
   >
   ><span class="preview">The Show all users icon is available only for the Workload Balancer of a project.</span> 

1. Click the **Chart icon** ![](assets/user-allocation-chart-icon.png) to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week.

   ![](assets/user-allocation-chart-350x237.png)

1. Click the **Show allocations icon** ![](assets/show-allocations-icon-small.png) to view the daily or weekly Planned Hours for work items.

   This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default.

   >[!TIP]
   >
   >* The Show allocations setting only affects what displays for projects, tasks, issues and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.
   >* You must enable the Group by Project setting to display daily Planned Hours for projects. 
   >* When you view the Workload Balancer by week, the hours displayed are the weekly Planned Hours. 

   Days that show overallocations display in red. 

1. (Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule.

   ![](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Optional) Click the **Hide allocations icon** ![](assets/show-allocations-icon-small.png) to display the name of the tasks in the bars of the work items. 
1. Click the **More menu** icon ![](assets/more-icon.png) to the right of a task or issue name, then click one of options below. 

   ![](assets/more-menu-right-of-task-350x104.png)

      * **Assign this to**, then start typing the name of a user, role, or team you want to assign the work item to in the **Search people, role, or teams** field.
    
      >[!TIP]
      >
      >You can also use the following shortcuts to assign tasks or issues:
      >
      >* In Windows: CTRL+click the task or issue bar.
      >* In Mac: CMD+click the task or issue bar.

      For more information about assigning work items to users in the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md). 

      >[!TIP]
      >
      >If your Workfront or group administrator enabled delegations in your environment, use the Assignments tab to assign users to the task or issue. For information about delegating work, see [Manage task and issue delegation](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edit allocations**, then edit the daily or weekly allocations for the user. For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

1. Click the bar of a task or issue to open the Summary panel on the right

   Or

   Click **Open Summary** icon ![](assets/summary-panel-icon.png), then click the bar of a task or issue to open the Summary panel

   Or

   Click the **More** menu ![](assets/more-icon.png) to the right of a task or issue, then click **Open Summary**.

   For information about updating task information in the Summary in the Workload Balancer, see [Update work items in the Workload Balancer using the Summary](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

    The Summary panel opens on the right. 

1. Click **Bulk Assignments** to assign work items in bulk.

   For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

1. Click the **Full screen** icon ![](assets/full-screen.png) to display the Workload Balancer in full screen, then click the **Exit full screen** icon ![](assets/exit-full-screen.png) to return to the default screen. 
1. (Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours, then click the **Save** icon ![](assets/save-allocations-wb.png) to save the allocations or the **Cancel** icon ![](assets/cancel-allocations-wb.png) to remove the allocations you adjusted.

   >[!TIP]
   >
   >The Save and Cancel icons display towards the end of a task or an issue's timeline bar.

   For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md). 

1. Click the name of a work item on the left to access it. 
1. Click the **Shareable link icon** ![](assets/wb-shearable-link-icon-small.png) to copy the direct URL for the Workload Balancer to your clipboard. 
1. (Optional) Share the link with any user who does not have direct access to the Workload Balancer.

   For information about sharing the Workload Balancer with a link, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md). 

1. (Conditional) From the Workload Balancer of a project, click the **Show role allocations** icon ![](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the Scenario Planner. For more information, see [Overview of reconciling resource allocations between projects and initiatives](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!TIP]
   >
   >You cannot view initiative job role information if your organization has not purchased a license for the Workfront Scenario Planner. In this case, you can only view the planned hours associated with job roles on the project. For more information, see [Access needed to use the Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

-->