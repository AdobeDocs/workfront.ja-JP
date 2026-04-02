---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: ビジネスルールの作成と編集
description: ビジネスルールを使用すると、Workfront オブジェクトに検証を適用し、特定の条件が満たされた場合にオブジェクトを作成、編集または削除できないようにすることができます。 ビジネスルールは、データの整合性を損なう可能性のあるアクションを防ぐことで、データ品質と業務効率の向上に役立ちます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '1823'
ht-degree: 5%

---

# ビジネスルールを作成および編集

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

-->

ビジネスルールを使用すると、Workfront オブジェクトに検証を適用し、特定の条件が満たされた場合にオブジェクトを作成、編集または削除できないようにすることができます。 ビジネスルールの検証は、データの整合性を損なう可能性のあるアクションを防止することで、データの品質と運用効率を向上させるのに役立ちます。

<!--

<div class="preview">

Organizations that have the Workflow Ultimate package can also configure business rules to automate actions for the created, edited, or modified object when certain conditions are met. Available actions include sharing the object or attaching a custom form to the object.  

</div>

-->

1つのビジネスルールは、1つのオブジェクトにのみ割り当てることができます。 例えば、特定の条件でプロジェクトを編集しないビジネスルールを作成した場合、同じルールをタスクに適用することはできません。 タスクに対して同じ条件を持つ別のビジネスルールを作成する必要があります。

アクセスレベルとオブジェクト共有は、ユーザーがオブジェクトとやり取りする際のビジネスルールよりも優先されます。 例えば、ユーザーがプロジェクトの編集を許可しないアクセスレベルまたは権限を持っている場合、特定の条件でプロジェクトの編集を許可するビジネスルールよりも優先されます。

1つのオブジェクトに複数のビジネスルールが適用される場合、ルールはすべてフォローされますが、特定の順序で適用されません。 例えば、2つのビジネスルールがあります。 2月の月に費用を作成することを制限します。 2つ目は、プロジェクトのステータスが「完了」の場合に、プロジェクトを編集できないようにします。 ユーザーが6月に完了したプロジェクトに費用を追加しようとすると、2つ目のルールがトリガーされたため、費用を追加できません。

ビジネスルールは、APIおよびWorkfront インターフェイスを使用したオブジェクトの作成、編集、削除に適用されます。

>[!NOTE]
>
>ビジネスルールは特定のアクションをブロックするため、実稼動環境で有効にする前に、必ずサンドボックスまたはプレビュー環境でビジネスルールを最初に設定し、徹底的にテストする必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
   <td> <p>ビジネスルール検証：<ul><li><p>Ultimate</p></li><li>
    <p>ワークフロー Ultimate</p></li></ul></p><p>ビジネスルールの自動化：<ul><li>
    <p>ワークフロー Ultimate</p></li><ul></p>
   </td>
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr>  
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ビジネスルールのシナリオ

* [ビジネスルール検証のシナリオ](#scenarios-for-business-rule-validation)
* [ビジネスルール自動化のシナリオ](#scenarios-for-business-rule-automation)

### ビジネスルール検証のシナリオ

ビジネスルール検証の形式は、「定義された条件が満たされた場合、ユーザーはオブジェクトに対するアクションから除外され、メッセージが表示されます」です。

ビジネスルールのプロパティおよびその他の関数の構文は、カスタムフォームの計算フィールドの構文と同じです。 構文について詳しくは、[ フォームデザイナーで計算フィールドを追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)を参照してください。

IF ステートメントについて詳しくは、[&quot;IF&quot; ステートメントの概要](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md)および[計算カスタムフィールドの条件演算子](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)を参照してください。

ユーザーベースのワイルドカードについて詳しくは、[ ユーザーベースのワイルドカードを使用してレポートを一般化する](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md)を参照してください。

日付ベースのワイルドカードについて詳しくは、[日付ベースのワイルドカードを使用してレポートを一般化する](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)を参照してください。

API ワイルドカードは、ビジネスルールでも使用できます。 `$$ISAPI`を使用して、API内でのみルールをトリガーします。 `!$$ISAPI`を使用して、ユーザーインターフェイスでのみルールを適用し、ユーザーがAPIを通じてルールをバイパスできるようにします。

* 例えば、このルールは、ユーザーがAPIを介して完了したプロジェクトを編集することを禁止します。 ワイルドカードが使用されていない場合、ルールはユーザーインターフェイスとAPIの両方でアクションをブロックします。

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

式では、`$$BEFORE_STATE`および`$$AFTER_STATE`のワイルドカードを使用して、編集前後にオブジェクトのフィールド値にアクセスします。

* これらのワイルドカードは、どちらも編集トリガーで使用できます。 編集トリガーのデフォルトのステート（ステートがエクスプレッションに含まれていない場合）は`$$AFTER_STATE`です。
* オブジェクト作成トリガーでは、before ステートが存在しないため、`$$AFTER_STATE`のみが許可されます。
* オブジェクト削除トリガーでは、後のステートが存在しないため、`$$BEFORE_STATE`のみが許可されます。

ビジネスルールのシナリオには、次のようなものがあります。

* ユーザーは2月の最後の週に新しい費用を追加することはできません。 この式は、次のように記述できます。

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* ユーザーは、プロジェクトのプロジェクト名を「完了」ステータスで編集することはできません。 この式は、次のように記述できます。

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

トリガーごとにオブジェクトごとに1つのビジネスルールを許可します。 例えば、1つのトリガールールを編集して問題を解決できます。 ただし、ネストされたIF ステートメントを使用して、数式に複数のルールを含めることができます。

ネストされたIF ステートメントを持つシナリオは次のとおりです。

ユーザーは完了したプロジェクトを編集できず、3月に完了予定日が設定されているプロジェクトを編集することはできません。 この式は、次のように記述できます。

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

### ビジネスルールでローカライズを有効にする

組織でカスタムローカライゼーションを使用している場合は、ビジネスルール内のビジネスルールメッセージの翻訳を有効にする必要があります。 翻訳が有効になっていない場合、メッセージのテキストがローカライゼーションリストに含まれ、ユーザーのブラウザーが適切な言語に設定されていても、メッセージは英語でリーダーに表示されます。

ルールを設定する場合は、メッセージの前にTRANSLATEという単語を挿入し、メッセージを括弧で囲みます。

>[!BEGINSHADEBOX]

例：

この例では、「完了したプロジェクトは編集できません」というメッセージが設定のローカライゼーション領域に含まれており、ユーザーのブラウザーがローカライズされた言語に設定されていることを前提としています。

* `IF({status} = "CPL", "You cannot edit completed projects.") `
メッセージは英語で表示されます。
* `IF({status} = "CPL", TRANSLATE("You cannot edit completed projects."))`
メッセージがローカライズされた言語で表示されます。

>[!ENDSHADEBOX]

カスタムローカライゼーションについて詳しくは、[ カスタムローカライゼーションの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md)を参照してください。

## ビジネスルール自動化のシナリオ

>[!NOTE]
>
>ビジネスルールの自動処理を使用するには、組織にWorkflow Ultimate パッケージが必要です。

ビジネスルール自動化の形式は、「定義された条件が満たされた場合、選択した自動化がトリガーされます」です。

ビジネスルールの自動化式では、エラーメッセージは必要ありません

プロジェクトの作成時など、選択したオブジェクトとアクションが発生するたびにオートメーションが実行されるようにするには、次の数式を使用します。

```
IF(true, true)
```

プロジェクトが承認されている場合にのみプロジェクトを共有するには、次のような数式を使用します。

```
IF({status} = "APR", true)
```

ビジネス ルールの検証[ シナリオ ](#scenarios-for-business-rule-validation)の節で説明しているように、ビジネス ルール アクションでワイルドカードを使用できます。


## 新しいビジネスルールの追加

{{step-1-to-setup}}

1. 左側のパネルで「**ビジネスルール**」をクリックします。
1. 「**新しいビジネスルール**」をクリックします。

1. ルールビルダーダイアログで、ビジネスルールの&#x200B;**名前**&#x200B;を入力します。
1. 「**はアクティブです**」フィールドで、ルールを保存するときにルールをアクティブにするかどうかを選択します。

   **No**&#x200B;を選択すると、ルールは非アクティブとして保存され、後でアクティブ化できます。

1. （オプション）ビジネスルールの&#x200B;**説明**&#x200B;と、それが適用されたときの処理を入力します。


1. ビジネスルールを割り当てるオブジェクトタイプを選択します。

   ![ オブジェクトを選択](assets/object-for-business-rule4.png)

   ビジネスルールは、次のオブジェクトに適用できます。

   * プロジェクト
   * タスク
   * イシュー/リクエスト
   * ポートフォリオ
   * ドキュメント
   * プログラム
   * 費用
   * 会社
   * イテレーション
   * 請求記録
   * グループ
   * 労力以外のリソース
   * リスク
   * レートカード
   * 割り当て
   * ユーザー
   * 役割
   * 時間
   * テンプレート
   * 休暇
   * リソースプール
   * 担当業務
   * 労力以外のリソースカテゴリ
   * リソースプール
   * 休暇
   * 時間
   * 人材の配置プラン
   * テンプレート
   * 人材の配置プランのリソース
<!--
   * <span class="preview">Team</span>
-->

1. ルールビルダーダイアログで、ビジネスルールの&#x200B;**名前**&#x200B;を入力します。
1. 「**はアクティブです**」フィールドで、ルールを保存するときにルールをアクティブにするかどうかを選択します。

   **No**&#x200B;を選択すると、ルールは非アクティブとして保存され、後でアクティブ化できます。

1. ビジネス ルールの&#x200B;**トリガー**&#x200B;を選択します。 オプションは次のとおりです。

   * **作成済み** ユーザーがオブジェクトを作成しようとすると、ルールが適用されます。
   * **編集済み** ユーザーがオブジェクトを編集しようとすると、ルールが適用されます。
   * **削除済み** ユーザーがオブジェクトを削除しようとすると、ルールが適用されます。

1. ビジネスルールダイアログの中央にある数式エディターで、数式を作成します。

   ビジネスルールの形式は、「定義された条件が満たされた場合、ユーザーはオブジェクトに対するアクションを禁止され、メッセージが表示されます」です。

   数式領域では、作成するビジネスルールの部分が条件であり、条件が満たされたときにWorkfrontに表示されるメッセージです。

   * 「オブジェクト」は、ビジネスルールの作成時に選択したオブジェクトタイプです。 ダイアログの見出しに表示されます。
   * 「アクション」は、ルールに対して選択したトリガー（オブジェクトの作成、編集、削除）です。
   * オブジェクトとアクションは既に定義されているため、数式に含めることはできません。
   * カスタムエラーメッセージ <span class="preview">は、ルールが検証用の場合にのみ含まれ、ビジネスルールをトリガーすると</span>がユーザーに表示されます。 問題の原因と修正方法について明確な指示を与える必要があります。

     エラーメッセージに静的URLを含めることで、ドキュメントやその他の便利なページにリンクし、ルールの制約の中でユーザーがアクションを変更する方法をガイドできます。

     この例では、「詳細情報」がURLにリンクされます。 `"You are not allowed to add a new project in November.[Learn more](http://url)"` URLは括弧で囲む必要がありますが、括弧内のリンクテキストは必要ありません。 完全なURLを表示することができ、クリック可能なリンクになります。

   ![ ビジネスルールダイアログを追加](assets/add-business-rule-new.png)

   この例は、プロジェクトのビジネスルールです。 現在の月が11月の場合、ユーザーは新しいプロジェクトを作成できません。このメッセージは、これを説明しています。

   ビジネスルールの詳細な例については、この記事の「[ ビジネスルールのシナリオ ](#scenarios-for-business-rules)」を参照してください。

1. （オプション）右側のパネルの式&#x200B;**式**&#x200B;と&#x200B;**フィールド**&#x200B;を使用して、ルールの作成を支援します。

   使用可能なアイテムのリストを絞り込む式またはフィールドを検索します。

   使用可能なフィールドのリストは、ビジネスルールのオブジェクトタイプに関連するフィールドに限定されます。

1. （条件付き）アクションを検証する場合、組織がWorkfront Ultimate パッケージ上にある場合は、「その後」領域で「**オブジェクトを検証する**」を選択します。

   その他のパッケージの場合、このオプションは事前に選択されています。

1. <span class="preview"> （条件付き）別のアクションを自動化するには、アクションを選択します。</span>

   <span class="preview">これらのアクションについて詳しくは、この記事の「[ ビジネスルールの自動化オプション ](#business-rule-automation-options)」の節を参照してください。</span>

   >[!NOTE]
   >
   ><span class="preview">検証以外のアクションを使用するには、組織がWorkflow Ultimate パッケージに属している必要があります。 これらの他のオプションが表示されない場合、組織はWorkflow Ultimate パッケージにありません。</span>

1. ビジネスルールの作成が完了したら、**保存**&#x200B;をクリックします。

>[!NOTE]
>
>ビジネスルールを追加したら、関連するオブジェクトを追加、編集、または削除してルールが適切に適用されていることを確認して、ルールをテストする必要があります。

<div class="preview">

### ビジネスルールの自動化オプション

>[!NOTE]
>
>検証以外のアクションを使用するには、組織がWorkflow Ultimate パッケージに属している必要があります。 その他のオプションが表示されない場合、組織はWorkflow Ultimate パッケージにありません。

これらのアクションは、ビジネスルールがトリガーされたときに自動化するように設定できます。 使用可能なアクションは、選択したオブジェクトタイプによって異なります。

| 自動化 | さらに設定 |
|---|---|
| カスタムフォームの添付 | 追加するカスタムフォームを選択します |
| オブジェクトを共有 | オブジェクトを共有するユーザー、役割、グループ、会社、またはアクセスレベルを選択します。 |

</div>

## ビジネスルールをアクティブ化

ビジネスルールが非アクティブの場合、ビジネスルールのリストの「アクティブです」フィールドに「False」と表示されます。 リスト ビューでルールのステータスを更新することはできません。

ビジネスルールをアクティブ化するには：

1. ルールのリストでビジネスルールを選択し、編集アイコンをクリックします。
1. ビジネスルールダイアログで「**はアクティブです**」の「**はい**」を選択します。
1. 「**保存**」をクリックします。

