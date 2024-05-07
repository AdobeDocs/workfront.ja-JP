---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 基本的なシナリオの作成： [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion を使用してシンプルな自動処理シナリオを作成する方法について説明します。 自動処理シナリオは、データの操作や変換を含む Workfront プロセスを自動化します。この例では、を検索するシナリオの作成手順を説明します [!DNL Workfront] Workfrontのタスクおよびがプロジェクトに変換します。
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 32%

---

# 基本的なシナリオの作成： [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] の役割は、同じタスクを何度も繰り返すのではなく、新しいタスクに集中できるようにプロセスを自動化することです。これは、アプリ内やサービス内、およびそれらの間でアクションをリンクし、データを自動的に転送および変換するシナリオを作成することで機能します。作成するシナリオは、アプリまたはサービス内のデータを監視し、そのデータを処理して必要な結果を提供します。

この例では、を検索するシナリオの作成手順を説明します [!DNL Workfront] Workfrontのタスクおよびがプロジェクトに変換します。

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## 練習シナリオを作成

### シナリオの作成を開始

1. が含まれる **シナリオ** エリア、クリック **新しいシナリオの作成**.

   <!--To locate the Scenarios area, see navigation article-->

   シナリオエディターが表示され、中央に空のモジュールが含まれます。

   <!--picture?-->

1. 「」を選択します **[!UICONTROL 新しいシナリオ]** 左上隅のプレースホルダー名を入力し、名前を入力します。
1. 続いて、以下の[最初のモジュールを追加して設定](#add-and-configure-the-first-module)を行います。

### 最初のモジュールを追加して設定

1. 空のモジュールをクリックして、モジュールを選択するアプリを選択します。

   アプリのリストがモジュールの右側に表示されます。

1. を選択 **[!DNL Adobe Workfront]**. 表示されない場合は、リストの下部にある検索バーをクリックして「Workfront」と入力し、リストに表示されたら選択します。

   リストが「すべて表示」に変わります [!DNL Workfront] 使用可能なモジュール。

1. 「」をクリックします **[!UICONTROL 検索]** モジュール。

   モジュール設定ウィンドウが開きます。

1. が含まれる [!UICONTROL 接続] ボックスで、Workfront接続を選択します。

   Workfrontに接続されていない場合は、を参照してください。 [への接続の作成 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. が含まれる [!UICONTROL レコードタイプ] ボックス、選択 **[!UICONTROL タスク]**. これにより、タスクのみを検索するようにモジュールが設定されます。

   次を見つけることができます **[!UICONTROL タスク]** 単語「」を入力し始めた場合は、リストで次の操作を行います。[!UICONTROL タスク].」と入力します。

1. が含まれる **[!UICONTROL 結果セット]** ボックス、選択 **[!UICONTROL 最初に一致したレコード]**.

   これにより、条件を満たす最初のレコードのみを返すようにモジュールが設定されます。
1. が含まれる **[!UICONTROL 検索条件]** エリアで、特定のタスクを返す条件を設定します。

   1. の下の最初のボックスに [!UICONTROL 検索条件]で、検索に含めるフィールドを選択します。 この例では、「**[!UICONTROL 名前]**」を選択します。

      次を見つけることができます **[!UICONTROL 名前]** 単語「」を入力し始めた場合は、リストで次の操作を行います。[!UICONTROL 名前].」と入力します。
   1. オペレーターの場合は、の横にあるドロップダウン矢印をクリックします。 **存在する** に変更します。 [!UICONTROL **含む（大文字と小文字を区別しない）**].

      これにより、名前全体を入力しない場合または名前に大文字と小文字を区別せずに入力した場合でも、モジュールは名前に選択した単語を含むプロジェクトを検索できます（すべて大文字など）。
   1. の下の最後のフィールド [!UICONTROL 検索条件]検索するタスクの名前に含まれていることがわかっている単語またはフレーズを入力します。

1. が含まれる **[!UICONTROL 出力]** リストから、モジュールで出力するフィールドを選択します。 この例では、「**[!UICONTROL ID]**」フィールドおよび「**[!UICONTROL 名前]**」フィールドを選択します。

   >[!TIP]
   >
   >**Cmd+F**（[!DNL Mac] OS）または **Ctrl+F**（[!DNL Windows] OS）を使用して、すばやくフィールドを検索できます。

1. クリック **[!UICONTROL OK]** モジュール設定を保存します。

1. モジュールを右クリックし、 **[!UICONTROL 名前を変更]**&#x200B;モジュールで実行する内容を示す名前（「タスクを検索」など）を入力し、 **[!UICONTROL OK]**.

   名前はモジュールのすぐ下に表示されます。その下に [!DNL Workfront Fusion] には、モジュールで実行されるアクションのタイプに関する簡単な説明が含まれます。

   ![](assets/module-renamed-wf.png)

1. [2 つ目のモジュールを追加して設定](#add-and-configure-the-second-module)に進みます。

## 2 つ目のモジュールを追加して設定

1. モジュールの右側にある円の上にマウスポインターを置き、クリックします **[!UICONTROL 別のモジュールを追加]**.
1. を選択 [!DNL Adobe Workfront] アプリケーションのリストから、モジュールを選択します **[!UICONTROL オブジェクトを変換]**.
1. が含まれる [!UICONTROL 接続] フィールドで、前のモジュールで使用したのと同じWorkfront接続を選択します。
1. が含まれる **[!UICONTROL レコードタイプ]** フィールド、選択 **[!UICONTROL タスク]**&#x200B;モジュールがタスクを変換するからです。
1. が含まれる **[!UICONTROL に変換]** フィールド、選択 **プロジェクト**.
1. 「タスク ID」フィールドの横にある「マップ」切替スイッチをクリックして有効にします。

   切替スイッチが有効になると青に変わります。 これにより、前のモジュールからタスク ID をマッピングできます。

   ![マップの切り替え](assets/map-toggle.png)
1. 「」をクリックします **[!UICONTROL タスク ID]** フィールド。

   パネルが開き、プロジェクトに変換するタスクの ID として使用するものを選択できます。 マッピングを有効にしたため、パネルには以前のモジュールからの出力が含まれます。 以前のモジュールの出力として ID を選択したので、パネルで使用できるようになりました。

   このパネルは、マッピングパネルと呼ばれます。 マッピングパネルについて詳しくは、 [モジュール間で情報をマッピングする](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. を選択 **ID** をマッピングパネルに表示します。

   「ID」フィールドに ID ブロックが表示されます。 マッピング元のモジュールの数と、マッピングされたフィールドが表示されます。

   ![マップ ID](assets/map-id.png)

1. 「」をクリックします **テンプレート ID** フィールドに、このプロジェクトに使用するWorkfront テンプレートの名前を入力し始め、リストに表示されたら選択します。
1. クリック **[!UICONTROL OK]** モジュール設定を保存します。

1. モジュールを右クリックし、 **[!UICONTROL 名前を変更]**&#x200B;モジュールで実行する内容を示す名前（「プロジェクトに変換」など）を入力し、 **[!UICONTROL OK]**.

1. 続行 [シナリオのテスト](#test-the-scenario).

## シナリオのテスト

シナリオをアクティベートする前にテストすることが重要です。少なくとも 1 回実行して結果を確認します。これは、シナリオにおけるデータの流れを理解し、エラーを見つけるのに役立ちます。

このシナリオでは、テストが成功すると、新しいタスクが見つかり、プロジェクトに変換されます。

1. シナリオエディターの左下隅にある「**[!UICONTROL 1 回実行]**」をクリックします。
1. シナリオの実行が完了したら、最初のモジュールの上にあるバブルをクリックして、モジュールが処理したデータのバンドルに関する情報（モジュールが返したタスクから取り込まれたデータを含む）を表示できます。

1. 2 番目のモジュールの上にある実行インスペクターのバブルをクリックして、入力（タスク）と出力（変換されたプロジェクト）を確認します。

   検査バブル内のデータの詳細については、以下を参照してください。

   * 詳しくは、[ [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md) でのシナリオ実行フローを参照してください。
   * 処理されたバンドルについて詳しくは、[ [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズを参照してください。

1. 対象： [!DNL Workfront Fusion]を選択し、 **[!UICONTROL 保存]** 左下隅付近にあるシナリオの進捗を保存します。

   >[!IMPORTANT]
   >
   >シナリオを改良、テストするたびに保存するようにしてください。

>[!TIP]
>
>各モジュールに関するメモを追加する方法として、任意ではあるものの便利な方法をお勧めします。
>
>1. [!DNL Workfront] モジュールを右クリックして、「**[!UICONTROL メモを追加]**」をクリックします。
>1. 表示されるメモに、モジュールの概要を入力します。
>
>    1 つのモジュールに複数のノートを追加できます。
>
>1. **[!UICONTROL メモ]**&#x200B;エリアを閉じます。
>
>     シナリオにメモを追加すると、シナリオエディターの下部の&#x200B;**[!UICONTROL メモ]**&#x200B;アイコン ![](assets/notes-icon-w-dot.png) にオレンジ色の点が表示されます。
>
>1. **[!UICONTROL メモ]**&#x200B;アイコン ![](assets/notes-icon-w-dot.png) をクリックして、メモを表示します。
>

## シナリオをアクティベート

シナリオを作成するための最後の手順は、シナリオをアクティブ化することです。

このシナリオでは特定のタスクを検索するので、アクティブ化する必要はありません。 シナリオをアクティブ化すると、スケジュールに従って、またはアプリケーションで特定のアクションが発生したときにシナリオが実行されます。 シナリオをアクティベートすると、デフォルトでは 15 分ごとに実行されます。これは、実行するタイミングと頻度を定義することで変更できます。

シナリオのアクティブ化について詳しくは、[[!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md) でのシナリオのアクティブ化または非アクティブ化を参照してください。

スケジュールについて詳しくは、[[!UICONTROL Adobe Workfront Fusion でのシナリオのスケジュール設定]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md)を参照してください。

## 次のステップ

* [トリガーモジュールを追加](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) これにより、シナリオで定期的に新しいリクエストを検索し、プロジェクトに変換できるようになります。
* Webhook を追加して、リクエストが入力されるたびにシナリオを実行できるようにします。
* フィルターを追加して、特定のリクエストのみがプロジェクトに変換されるようにします。
* 新しいプロジェクトの名前をカスタマイズする関数を追加します。
* エラー処理を追加し、シナリオがエラーに対して回復力を持つようにします。

