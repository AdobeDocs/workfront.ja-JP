---
title: プロジェクトの正常性の概要
content-type: reference
description: プロジェクトヘルス機能は、AI アシスタントの機能を活用して、プロジェクトのパフォーマンスを即座に評価します。
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
hide: true
hidefromtoc: true
source-git-commit: 16e8213197e881d4d7b1a4b1bf8d3a43438ab938
workflow-type: tm+mt
source-wordcount: '1488'
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

AI アシスタントの詳細については、「[AI アシスタントの概要 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)」を参照してください。

+++ 展開すると、アクセス要件が表示されます。 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>PrimeまたはUltimateを選択 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>標準</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>プロジェクト正常性設定を管理する管理者 </p>
   <p>を編集して、プロジェクトの正常性設定を適用します </p>
     <p>プロジェクトの正常性構成を表示するビュー </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## プロジェクト正常性ベータ版への登録

プロジェクトの正常性を利用するには、組織で AI アシスタントを有効にする必要があります。

組織の AI アシスタントとプロジェクトの正常性を有効にするには、次のすべてを適用する必要があります。

* 組織がAdobe IMS（Identity Management System）に移行している必要があります。
* 組織には Select、Prime、UltimateのいずれかのWorkfront プランが必要です
* Adobe統合エクスペリエンスを有効にする必要があります。
* Adobeには、Adobe生成 AI 契約がファイルに署名済みである必要があります。
* Workfront管理者は、組織内のユーザーに対して AI アシスタントを有効にする必要があります。 AI アシスタントはアクセスレベルで有効になります。
* 設定/環境設定の AI 環境設定セクションで、「AI を有効にする」オプションと「プロジェクトの正常性」オプションの両方を選択する必要があります。

  ![AI 環境設定セクション ](assets/ai-preferences.png)

詳しくは、[AI アシスタントの概要 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) および [ システム環境設定の設定 ](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md) を参照してください。

## AI アシスタント プロンプト リスト

アカウントのプロジェクト、プログラム、またはすべてのプロジェクトについて、AI 評価にプロジェクトの正常性の評価を生成するよう依頼する際に使用できるプロンプトのリストを以下に示します。

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


## プロジェクトとプログラムの条件のリスト

以下は、プロジェクトの状態評価を生成する際に、AI アシスタントがプロジェクトまたはプログラムを割り当てる条件です。

<table>
    <tr>
        <td><b>プロジェクト状況</b></td>
        <td><b>プロジェクトの進捗ステータス</b></td>
        <td><b>プロジェクト状況の要因</b></td>
    </tr>
    <tr>
        <td>目標どおり</td>
        <td>この分析は、次の要因の平均リスクレベルが正常なしきい値の範囲内にある場合に割り当てられます。
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
        <td>この分析は、次の要因の平均リスクレベルが正常なしきい値を下回った場合に割り当てられます。</td>
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
        <td>この分析は、次の要因の平均リスクレベルが正常なしきい値を下回った場合に割り当てられます。</td>
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

## プロジェクト正常性設定の管理

プロジェクトの正常性の構成には、プロジェクトの正常性の計算方法を決定する特定の条件が含まれています。 設定を作成したら、それをプロジェクトに適用できます。

>[!NOTE]
>
>プロジェクトの正常性設定を管理するにはシステム管理者である必要があります。

{{step-1-to-setup}}

1. 左側のパネルで **プロジェクト環境設定** をクリックし、表示されるドロップダウンで **プロジェクトの正常性** を選択します。

1. ページの右上隅にある「**新規設定**」を選択します。

1. （オプション）設定の詳細ページで、*名称未設定* を新しい設定 **名前** に置き換えます。

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

1. **完全性をチェックするフィールドはどれか？「」セクション**、プロジェクトの完全性を判断するためにチェックされる 1 つ以上のフィールドを選択します。

   ![ プロジェクト完全性フィールド ](assets/project-completeness-fields.png)


1. 右上隅の **保存** をクリックします。

## プロジェクトの正常性設定の適用

管理者がプロジェクトの正常性設定を作成すると、編集アクセス権を持つユーザーはプロジェクトに適用できます。


{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。

1. プロジェクト名の右側にある **その他** アイコン ![ その他のアイコン ](assets/more-icon.png) をクリックし、「**編集**」を選択します。 **プロジェクトを編集** サイドパネルが開きます。

1. 左側のパネルで「**プロジェクト設定**」を選択します。

1. 「**プロジェクトの正常性設定**」フィールドで、このプロジェクトに適用する設定を選択します。

   ![ プロジェクトの正常性の構成フィールド ](assets/project-health-configurations.png)

1. パネルの左下にある「**保存**」をクリックします。

## プロジェクトまたはプログラムのプロジェクト正常性評価を生成する

プロジェクトまたはプログラムの表示アクセス権を持っている場合は、AI アシスタントを使用して、そのプロジェクトの正常性の評価を生成できます。

プロジェクトの評価を生成する場合は、プロジェクトページから実行するか、プロジェクトのパフォーマンスをアシスタントに問い合わせる際にプロジェクト名を参照して実行できます。

プログラムの評価を生成する場合は、プログラムの詳細ページから実行できます。

>[!NOTE]
>
>プロジェクトが開始されるまで、プロジェクトの正常性アセスメントは生成できません。 プロジェクトが開始するイベントトリガーーをプロジェクト設定で指定できます。

詳しくは、この記事の次の節 [ プロジェクト正常性設定の管理 ](#manage-project-health-configurations) を参照してください。

1. プロジェクトの正常性評価を生成するプロジェクトまたはプログラムに移動します。

1. プロジェクト/プログラムの詳細ページで、画面の右上隅にある **AI アシスタント** アイコン ![AI アシスタント アイコン ](assets/ai-assistant-icon.png) をクリックします。 AI アシスタントが開きます。

1. **Workfrontについて確認** フィールドに「*このプロジェクトの正常性は何ですか？* と入力します。

   または

   **Workfrontについて尋ねる** フィールドに「*このプログラムの正常性は何ですか？* と入力します。

   >[!NOTE]
   >
   >Workfrontの別のページから AI アシスタントにアクセスする場合は、「*プロジェクト [ プロジェクト名 ] の正常性は？* または *プログラムの正常性は何ですか [ プログラム名 ]?* <br>
   >入力できる現在のプロンプトの完全なリストについては、この記事の次のセクションを参照してください。[AI アシスタント プロンプト リスト ](#ai-assistant-prompts-list)。

1. **送信** アイコン ![ 送信アイコン ](assets/send-icon.png) を押します。 プロジェクトの正常性の評価が生成され、パネルに表示されます。 各プロジェクトの正常性評価の上部に、プロジェクトの現在の状態を反映したバッジが表示されます。

   ![ プロジェクトの正常性の評価 ](assets/health-assessment.png)

   ポートフォリオの評価を生成している場合、プログラム内の各プロジェクトの状態を示す複数のバッジが表示されます。 バッジラベルについて詳しくは、この記事の次の節 [ プロジェクトとプログラムの条件のリスト ](#project-and-program-conditions-list) を参照してください。

1. （任意）評価ポイントの 1 つをクリックして、詳細を展開します。

1. （オプション）展開された詳細モードで、タスクリンクをクリックしてタスクの詳細を開きます。

   ![ 展開された詳細 ](assets/expanded-details.png)

1. プロジェクトの正常性の詳細を確認した後、AI アシスタントの右上隅にある **閉じる** アイコン ![ 閉じるアイコン ](assets/close-icon.png) をクリックします。

## 複数のプロジェクトに対してプロジェクト正常性評価を生成する

現在「表示」アクセス権（またはそれ以上）を持つすべてのプロジェクトについて、組み合わせたプロジェクトの正常性の評価を生成できます。

プロジェクトは、プロジェクトが開始された場合にのみ、結合されたプロジェクトの正常性の評価に含まれます。 プロジェクトが開始するイベントトリガーーをプロジェクト設定で指定できます。 詳しくは、この記事の次の節 [ プロジェクト正常性設定の管理 ](#manage-project-health-configurations) を参照してください。

1. 画面の右上隅にある **AI アシスタント** アイコン ![AI アシスタント アイコン ](assets/ai-assistant-icon.png) をクリックします。 AI アシスタントが開きます。

1. **Workfrontについて確認** フィールドに次のように入力します。*プロジェクトの正常性はどうなっていますか？*

   入力できる現在のプロンプトの完全なリストについては、この記事の次のセクションを参照してください。[AI アシスタント プロンプト リスト ](#ai-assistant-prompts-list)。

1. **送信** アイコン ![ 送信アイコン ](assets/send-icon.png) を押します。 プロジェクトの正常性の評価が生成され、パネルに表示されます。

   ![ 複数プロジェクトの評価 ](assets/multiple-projects-assessment.png)

   複数のプロジェクトに対して評価を生成する場合、AI アシスタントは、プロジェクトの現在のパフォーマンスに基づいて結果をグループ化します。

1. （任意）プロジェクトの健全性の状態を示すバッジの 1 つをクリックしてプロジェクトリストを展開し、特定のプロジェクトのリンクを選択してそのプロジェクトの詳細ページに移動します。

1. プロジェクトの正常性の詳細を確認した後、AI アシスタントの右上隅にある **閉じる** アイコン ![ 閉じるアイコン ](assets/close-icon.png) をクリックして、プロジェクトを閉じます。

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
