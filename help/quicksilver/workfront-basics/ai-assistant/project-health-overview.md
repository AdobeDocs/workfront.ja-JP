---
title: プロジェクトの正常性の概要
content-type: reference
description: プロジェクトヘルス機能は、AI アシスタントの機能を活用して、プロジェクトのパフォーマンスを即座に評価します。
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: b95be2e0917b53195ac327880a2ea7399c1485de
workflow-type: tm+mt
source-wordcount: '2060'
ht-degree: 4%

---

# プロジェクトの正常性の概要

>[!IMPORTANT]
>
>プロジェクトの正常性機能は、現在、ベータ版のステージに参加しているユーザーのみが使用できます。

Adobe Workfrontのプロジェクトヘルス機能は、AI アシスタントの機能を活用して、プロジェクトのパフォーマンス、注意が必要な領域、時間とコストがかかる問題を回避する方法を即座に評価します。

AI アシスタントは、次のオブジェクトに対してプロジェクトの正常性の評価を生成できます。

* 単一のプロジェクト
* 単一のプログラム
* 複数のプロジェクト

AI アシスタントの詳細については、「[AI アシスタントの概要 &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)」を参照してください。

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
<p>Select 以上 </p> 
<p>ワークフローの選択またはそれ以上</p>
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>プロジェクト正常性設定を管理するにはシステム管理者である必要があります </p>
   <p>プロジェクトへのアクセスを編集してプロジェクトの正常性の構成を適用する </p>
     <p>プロジェクトへのアクセスを表示して、プロジェクトの正常性の構成を表示します </p>
     <p>プログラムへのアクセスを表示して、プログラム内のすべてのプロジェクトのプロジェクトの正常性の表示を使用します</p>
  </td> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>プロジェクト正常性設定を適用するための、プロジェクトに対する権限の管理 </p>
     <p>プロジェクトの正常性設定を表示する、プロジェクトへの権限を表示します。 </p>
  </td> 
  </tr> 
  </tr>  
    </tr>  
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## プロジェクト正常性ベータ版への登録

プロジェクトの正常性を使用するには、組織の AI アシスタントが有効である必要があります。

組織の AI アシスタントとプロジェクトの正常性を有効にするには、次のすべてを適用する必要があります。

* 組織はAdobe Identity Management System （IMS）に移行している必要があります。
* 組織には、Workfrontまたはワークフローの選択、PrimeまたはUltimateのパッケージが必要です。
* Adobe統合エクスペリエンスを有効にする必要があります。
* Adobeには、Adobe生成 AI 契約がファイルに署名済みである必要があります。
* Workfront管理者は、組織内のユーザーに対して AI アシスタントを有効にする必要があります。 AI アシスタントはアクセスレベルで有効になります。
* 設定のシステム環境設定領域の AI 環境設定セクションで、「AI を有効にする」オプションと「プロジェクトの正常性」オプションの両方を選択する必要があります。

  ![AI 環境設定セクション &#x200B;](assets/ai-preferences.png)

詳しくは、[AI アシスタントの概要 &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) および [&#x200B; システム環境設定の設定 &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md) を参照してください。

## プロジェクトの正常性の計算方法

AI アシスタントを使用すると、使用可能なプロジェクトの正常性の状態の 1 つを割り当てることで、プロジェクトの全体的な状態をすばやく評価できます。

* 目標どおり
* リスクあり
* トラブル発生中

この状態は、プロジェクトの進捗や過小評価されている作業など、プロジェクトのコンポーネントを使用して計算されます。 プロジェクトの正常性の測定に使用するコンポーネントの完全なリストについては、[&#x200B; プロジェクトとプログラムの状態リスト &#x200B;](#project-and-program-states-list) の節を参照してください。

各プロジェクトコンポーネントには、（0 ～ 100）の数値リスクスコアが割り当てられ、このスコアが平均されて、プロジェクトの全体的な正常性の状態が作成されます。

* 目標どおり（75 以上）: プロジェクトのパフォーマンスが、期待されるしきい値の範囲内です。
* リスクあり（50 ～ 74）：プロジェクトのパフォーマンスに影響を与える可能性のある新たな問題が検出されました。
* 問題あり（49 以下）：プロジェクトのパフォーマンスが許容可能なしきい値を下回っており、早急な対応が必要です。

>[!NOTE]
>
>* AI アシスタントは現在、選択されたプロジェクトのデータのみを評価します。
>* プロジェクト間または履歴分析は、まだプロジェクトの正常性の計算に含まれていません。

### プロジェクトのプロジェクト正常性の計算例

最初の例では、4 つのプロジェクトコンポーネントが評価され、それらの個々のリスクスコアが次のように計算されます。

* 2 On Target （90 リスクスコア）
* 1 危険（45 リスクスコア）
* 1 件の問題（20 リスクスコア）

これらのスコアを平均すると、結果は 61 になります。 上記のプロジェクトの正常性の条件を使用すると、このプロジェクトは危険な状態になります。

次の例では、プロジェクトのタイムラインの早い段階で、スケジュールの変更が 1 日と発生しています。 このシナリオでは、AI アシスタントがプロジェクト全体の期間に対して、変更のタイミングと影響の両方を評価します。

* 60 日のプロジェクトタイムラインの初期における 1 日間のスケジュールシフトは、マイナーで、通常はターゲット通りとスコアが付けられます。
* プロジェクトの完了日付近で 1 日間のスケジュールシフトを行うと、より混乱が生じ、「危険あり」または「トラブル発生中」とスコアされる場合があります。

この変更は軽微で、プロジェクトタイムラインの初期に発生したので、プロジェクトは目標通りの状態になります。

プロジェクトのタイムライン内で複数のスケジュールの変更が発生した場合、これらの変更はスコアリングされ、プロジェクトの正常性の計算に適用される前に平均されます。

## プロジェクトの状態とプロジェクトの正常性の違いについて

プロジェクトの状態やプロジェクトの正常性は、Workfrontと似た概念で、プロジェクトの状態（目標どおり、危険あり、トラブル発生中）を示すデフォルトの名前は同じですが、目的が異なります。

プロジェクトの条件は、予定日、見込み日、推定日にのみ、プロジェクトの現在のパフォーマンスに関する基本的なスナップショットを提供します。 プロジェクトオーナーが手動で設定することも、Workfrontがプロジェクトのタスクに基づいて自動的に設定することもできます。 または、プロジェクトヘルスはより包括的で、追加の要因を評価し、パフォーマンスをより高いレベルで理解できるようにします。

プロジェクト条件について詳しくは、次の記事を参照してください。

* [プロジェクトの状況の更新](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-condition-on-project.md)
* [&#x200B; カスタム条件 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)。

## プロジェクトとプログラムのプロジェクト正常性の状態リスト

次の表に、プロジェクトの状態評価を生成する際に、AI アシスタントがプロジェクトまたはプログラムを割り当てる際に使用できる状態の分類を示します。

<table>
    <tr>
        <td><b>プロジェクトの状態</b></td>
        <td><b>定義</b></td>
        <td><b>要因</b></td>
    </tr>
    <tr>
        <td>目標どおり</td>
        <td>これは、次の要因の平均リスクレベルが正常なしきい値の範囲内にある場合に割り当てられます。
        </td>
        <td> 
        <ul><li>スコープクリープ</li>
        <li>フィールドがありません</li>
        <li>スケジュールの変更</li>
        <li>過小評価された仕事</li>
        <li>プロジェクト進行状況</li>
        <li>期限切れタスク</li>
        <li>予算</li>
        </ul></td>
    </tr>
    <tr>
        <td>リスクあり</td>
        <td>これは、次の要因の平均リスクレベルが正常なしきい値を下回る場合に割り当てられます。</td>
        <td>
        <ul><li>スコープクリープ</li>
        <li>フィールドがありません</li>
        <li>スケジュールの変更</li>
        <li>過小評価された仕事</li>
        <li>プロジェクト進行状況</li>
        <li>期限切れタスク</li>
        <li>予算</li>
        </ul></td>
    </tr>
    <tr>
        <td>トラブル発生中</td>
        <td>これは、次の要因の平均リスクレベルが正常なしきい値を下回ると割り当てられます。</td>
        <td>
        <ul><li>スコープクリープ</li>
        <li>フィールドがありません</li>
        <li>スケジュールの変更</li>
        <li>過小評価された仕事</li>
        <li>プロジェクト進行状況</li>
        <li>期限切れタスク</li>
        <li>予算</li>
        </ul></td>
    </tr>
    </tr>
   </table>

## AI アシスタント プロンプト リスト

表示するアクセス権のあるプロジェクト、プログラム、またはすべてのプロジェクトについて、AI アシスタントにプロジェクトの正常性の評価を生成するよう依頼するために使用できるプロンプトのリストを以下に示します。

<table>
    <tr>
        <td><b>Location</b></td>
        <td><b>プロンプト</b></td>
    </tr>
    <tr>
        <td>特定のプロジェクトの詳細ページ</td>
        <td><em>このプロジェクトの健全性はどうか。</em></td>
    </tr>
    <tr>
        <td>Workfrontの任意のページ </td>
        <td><em>プロジェクト [ プロジェクト名 ] の状態は？</em></td>
    </tr>
    <tr>
        <td>Workfrontの任意のページ </td>
        <td><em>プロジェクトの正常性はどうですか？</em></td>
    </tr>
       <tr>
        <td>特定のプログラムの詳細ページ</td>
        <td><em>このプログラムの正常性は何ですか？</em></td>
    </tr>
       <tr>
        <td>Workfrontの任意のページ </td>
        <td><em>プログラム [PROGRAM NAME] の状態は？</em></td>
    </tr>
   </table>

## プロジェクト正常性設定の管理

プロジェクトの正常性設定を管理するにはシステム管理者である必要があります。

プロジェクトの正常性の構成には、プロジェクトの正常性の計算方法を決定する特定の条件が含まれています。 Workfront管理者が設定を作成したら、その設定をプロジェクトに適用できます。

システムには複数のプロジェクトの正常性を設定できます。

{{step-1-to-setup}}

1. 左側のパネルで **プロジェクト環境設定** をクリックし、「**プロジェクトの正常性**」を選択します。

1. ページの右上隅にある「**新規設定**」をクリックします。

   **AI 設定** ページが開きます。

1. （オプション） **名称未設定** タイトル内をクリックして、設定の名前を変更します。

1. 「**プロジェクトの正常性に含める要因**」セクションで、プロジェクトの正常性の条件を決定する際に含めない要因の選択を解除します。
   * **範囲のクリープ**：プロジェクト範囲が開始以降に拡張された量。

   * **必須フィールド**：必須フィールドがない場合（プロジェクト説明など）。 これらの必須フィールドは、プロジェクトの完全性を判断するもので、**完全性をチェックするフィールドを選択してください。次** 設定の節を参照してください。


   * **スケジュールの変更**：プロジェクトが開始されてから発生したスケジュールの変更数。

   * **タスクの見積もり**：タスクの作業がどの程度正確に見積もられているか（例：期限切れタスクがプロジェクトに現在存在しない）。

   * **タスクのバーンダウン**：プロジェクトタイムラインと比較した、プロジェクトの作業の進行状況。

   * **期限切れタスク**：現在期限切れのタスクの数。

   * **コスト**：現在プロジェクトが予算を超過している場合。

1. **プロジェクトが正式に開始されるのはいつですか？** セクションで、ドロップダウンからプロジェクトの開始を示すイベントを選択します。

1. **プロジェクトの作業範囲を見積もるにはどうすればよいですか？** セクションでは、プロジェクトの範囲を広げるにつれて増加するプロジェクト要因を選択します。

1. **必須フィールドを確認する場所を選択してください。「」セクション**、プロジェクトの値を含む必要がある 1 つ以上のフィールドを選択します。

   ![&#x200B; プロジェクトの正常性のプロジェクト必須フィールド &#x200B;](assets/project-completeness-fields.png)

1. さらにネイティブまたはカスタムのプロジェクトまたはタスクフィールドに **追加** をクリックします。

1. 右上隅の **保存** をクリックします。

## プロジェクトの正常性設定の適用

Workfront管理者がプロジェクトの正常性設定を作成した後、プロジェクトに対する管理権限を持っている場合は、その設定をプロジェクトに適用できます。

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。

1. プロジェクト名の右側にある **その他** アイコン ![&#x200B; その他のアイコン &#x200B;](assets/more-icon.png) をクリックし、「**編集**」を選択します。 「**プロジェクトを編集**」ボックスが開きます。

1. 左側のパネルで、「**プロジェクト設定**」をクリックします。

1. 「**プロジェクトの正常性設定**」フィールドで、このプロジェクトに適用する設定を選択します。

   ![&#x200B; プロジェクトの正常性の構成フィールド &#x200B;](assets/project-health-configurations.png)

1. ページの左下にある「**保存**」をクリックします。

## プロジェクトまたはプログラムのプロジェクト正常性評価を生成する

次の領域で、AI アシスタントからプロジェクトの状態評価を生成できます。

* プロジェクトの場合は、プロジェクトページから、または特定のプロジェクトのパフォーマンスをアシスタントに確認する際にプロジェクト名を参照することで、評価を生成できます。

* プログラムの場合、プログラムの詳細ページで評価を生成できます。

>[!NOTE]
>
>* 評価を生成するには、プロジェクトまたはプログラムに対する表示権限が必要です。
>* プロジェクトが開始されるまで、プロジェクトの正常性アセスメントは生成できません。 プロジェクトの環境設定で、プロジェクトが開始するイベントトリガーーを設定できます

詳しくは、この記事の [&#x200B; プロジェクト正常性設定の管理 &#x200B;](#manage-project-health-configurations) の節を参照してください。

プロジェクトまたはプログラムのプロジェクト正常性評価を生成する

1. プロジェクトの正常性評価を生成するプロジェクトまたはプログラムに移動します。

1. プロジェクト/プログラムの詳細ページで、画面の右上隅にある **AI アシスタント** アイコン ![AI アシスタント アイコン &#x200B;](assets/ai-assistant-icon.png) をクリックします。 AI アシスタントが開きます。

1. **Workfrontについて確認** フィールドに「*このプロジェクトの正常性は何ですか？* と入力します。

   または

   **Workfrontについて尋ねる** フィールドに「*このプログラムの正常性は何ですか？* と入力します。

   >[!NOTE]
   >
   >Workfrontの別のページから AI アシスタントにアクセスする場合は、「*プロジェクト [ プロジェクト名 ] の正常性は？* または *プログラムの正常性は何ですか [ プログラム名 ]?* <br>
   >入力できる現在のプロンプトの完全なリストについては、この記事の [AI アシスタント プロンプト リスト &#x200B;](#ai-assistant-prompts-list) の節を参照してください。

1. **送信** アイコン ![&#x200B; 送信アイコン &#x200B;](assets/send-icon.png) をクリックします。 プロジェクトの正常性の評価が生成され、パネルに表示されます。 各プロジェクトの正常性評価の上部に、プロジェクトの現在の状態を反映したバッジが表示されます。

   ![&#x200B; プロジェクトの正常性の評価 &#x200B;](assets/health-assessment.png)

   プログラムの評価を生成する場合、プログラム内の各プロジェクトの状態を示す複数のバッジが表示されます。 バッジラベルについて詳しくは、この記事の [&#x200B; プロジェクトとプログラムの状態リスト &#x200B;](#project-and-program-states-list) の節を参照してください。

1. （任意）評価ポイントの 1 つをクリックして、詳細を展開します。

1. （任意）展開された詳細モードで、プロジェクトリンクをクリックしてプロジェクトの詳細を開きます。

   ![&#x200B; 展開された詳細 &#x200B;](assets/expanded-details.png)

1. プロジェクトの正常性の詳細を確認した後、AI アシスタントの右上隅にある **閉じる** アイコン ![&#x200B; 閉じるアイコン &#x200B;](assets/close-icon.png) をクリックします。

## 複数のプロジェクトに対してプロジェクト正常性評価を生成する

表示権限以上を現在持つすべてのプロジェクトについて、組み合わせたプロジェクトの正常性の評価を生成できます。

プロジェクトは、プロジェクトが開始された場合にのみ、結合されたプロジェクトの正常性の評価に含まれます。 プロジェクトが開始するイベントトリガーーをプロジェクト設定で指定できます。 詳しくは、この記事の [&#x200B; プロジェクト正常性設定の管理 &#x200B;](#manage-project-health-configurations) の節を参照してください。

1. 画面の右上隅にある **AI アシスタント** アイコン ![AI アシスタント アイコン &#x200B;](assets/ai-assistant-icon.png) をクリックします。 AI アシスタントが開きます。

1. **Workfrontについて確認** フィールドに次のように入力します。*プロジェクトの正常性はどうなっていますか？*

   入力できる現在のプロンプトの完全なリストについては、この記事の次のセクションを参照してください。[AI アシスタント プロンプト リスト &#x200B;](#ai-assistant-prompts-list)。

1. **送信** アイコン ![&#x200B; 送信アイコン &#x200B;](assets/send-icon.png) をクリックします。 プロジェクトの正常性の評価が生成され、パネルに表示されます。

   ![&#x200B; 複数プロジェクトの評価 &#x200B;](assets/multiple-projects-assessment.png)

   複数のプロジェクトに対して評価を生成する場合、AI アシスタントは、プロジェクトの現在のパフォーマンスに基づいて結果をグループ化します。

1. （任意）プロジェクトの健全性の状態を示すバッジの 1 つをクリックしてプロジェクトリストを展開し、特定のプロジェクトのリンクを選択してそのプロジェクトの詳細ページに移動します。

1. プロジェクトの正常性の詳細を確認した後、AI アシスタントの右上隅にある **閉じる** アイコン ![&#x200B; 閉じるアイコン &#x200B;](assets/close-icon.png) をクリックして、プロジェクトを閉じます。

<!--

## Build a Project Health table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md). 

You can add a table report to a Canvas Dashboard in order to easily visualize your Project Health data in a table format.  

### Prerequisites 

You must create a dashboard before you can build a table report. 

For more, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Build a Project Health table report 

There are many configuration options available for building a Project Health table report. In this section, we'll walk you through the process of creating one that displays the following columns: 

* **Name**: Contains the project name. 
* **Project Health Analysis**: Contains a summary of the Project Health assessment. 
* **Project Health Created At**: Contains the date/time when the Project Health assessment was last generated. 
* **Project Health Label**: Contains the project's label (e.g. On Target, At Risk, or In Trouble).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. In the upper-right corner, click **New Dashboard**. 
1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**. 
1. Click **Create**. 
1. In the **Add report** box, select **Create report**. 
1. On the left side, select **Table**. 
1. In the upper-right corner, click **Create report**. 
1. (Optional) Follow the steps below to configure the **Details** ![Details icon](assets/details-icon.png) section: 
    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
1. Follow the steps below to configure the **Build table** ![Build table icon](assets/drilldown-column.png) section: 
    1. In the left panel, click the **Table columns** icon. 
    1. Click **Add column**, then select **Project** > **Name**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Analysis**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Created At**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Label**. 

1. Follow the steps below to configure the **Filter** ![Filter icon](assets/filter-icon.png) section: 
    1. In the left panel, click the **Filter** icon. 
    1. Select **Edit filter**. 
    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.
    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** ![Group settings](assets/drilldown-group-icon.png) section: 
    1. In the left panel, click the **Group Settings** icon. 
    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report.

-->
