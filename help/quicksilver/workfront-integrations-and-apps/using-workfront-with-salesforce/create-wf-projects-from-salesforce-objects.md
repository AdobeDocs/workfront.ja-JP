---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: ' [!DNL Salesforce]  オブジェクトからの  [!DNL Adobe Workfront]  プロジェクトの作成'
description: ' [!DNL Adobe Workfront] for Salesforce をインストールした後、 [!DNL Salesforce] 商談とアカウントで特定の基準が満たされたときに [!DNL Workfront] プロジェクトを作成するトリガーを定義できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: ht
source-wordcount: '1506'
ht-degree: 100%

---

# [!DNL Salesforce] オブジェクトからの [!DNL Adobe Workfront] プロジェクトの作成

[!DNL Adobe Workfront]for Salesforce をインストールした後、[!DNL Salesforce] [!UICONTROL  の商談]と[!UICONTROL アカウント]で特定の基準が満たされたときに [!DNL Workfront] プロジェクトを作成するトリガーを定義できます。

## アクセス要件

この記事で説明されている機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Salesforce][!UICONTROL 商談]またはアカウントから [!DNL Workfront] リクエストを送信するには、
環境に次のものが存在することを確認してください。

* [!DNL Workfront] 管理者が [!DNL Workfront for Salesforce] を既にインストールしている。\
   [!DNL Workfront for Salesforce] のインストールについて詳しくは、[ [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) のインストールを参照してください。

* [!DNL Workfront] 管理者が、[!UICONTROL 商談]ページとアカウントページのレイアウトに「[!DNL Workfront]」セクションを
既に追加している。\
   ページレイアウトに「[!DNL Workfront]」セクションを追加する方法について詳しくは、[ [!DNL Salesforce] ユーザーへの「 [!DNL Adobe Workfront] 」セクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

* [!DNL Workfront] アカウントがあり、[!UICONTROL 商談]またはアカウント内の「[!DNL Workfront]」セクションからログインできる。


## [!DNL Salesforce] からの [!DNL Workfront] プロジェクトの作成の設定

* [プロジェクトの自動作成について](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [トリガーの設定](#configuring-triggers-configuring-triggers)
* [プロジェクト名について](#understanding-project-names-understanding-project-names)

### プロジェクトの自動作成について {#understanding-the-automatic-creation-of-projects}

[!DNL Salesforce] システム管理者は、[!DNL Salesforce] で次のことが発生したときに [!DNL Workfront] でプロジェクトを自動的に作成できるトリガーを定義できます。

* [!UICONTROL 商談]の[!UICONTROL ステージ]が更新された。
* アカウントの[!UICONTROL タイプ]の数が
更新された。

トリガーは、[!DNL Workfront for Salesforce] をインストールした後にのみ設定できます。  \
[!DNL Workfront for Salesforce] のインストールについては、[ [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) のインストールを参照してください。

[!DNL Salesforce] の項目が作成または更新されたときに [!DNL Workfront] プロジェクトを自動的に作成するようにトリガーを設定する場合は、以下を考慮してください。

* トリガーを設定するには、[!DNL Salesforce] および [!DNL Workfront] のシステム管理者である必要があります。
* 設定後、[!UICONTROL 商談]の[!UICONTROL ステージ]、またはアカウントの[!UICONTROL タイプ]を更新する人は誰でも、
[!DNL Workfront] プロジェクトの作成をトリガーできます。これには、[!DNL Workfront] アカウントを持たない [!DNL Salesforce] ユーザーも含まれます。
* 使用できるトリガー数に制限はありません。
* 同じ条件に基づいて複数のトリガーを作成することはできません。トリガーは、デフォルトで一意です。
* プロジェクトを作成すると、そのプロジェクトは自動的に商談または生成されたアカウントにリンクされます。一旦確立すると、このリンクは切断できません。
* 商談またはアカウントの存続期間中にトリガーされた条件が複数回満たされた場合、1 つの商談またはアカウントを [!DNL Workfront] の複数のプロジェクトにリンクできます。

  例えば、[!UICONTROL 商談]に対して複数の[!UICONTROL ステージ]を定義してプロジェクトをトリガーすると、プロジェクトは、その商談が存在する限り、その商談が到達する定義済みのステージごとに作成されます。また、[!UICONTROL 商談]の[!UICONTROL ステージ]を定義されたステージから別のステージに更新し、その後定義されたステージに戻すと、2 回目に「[!UICONTROL ステージ]」フィールドを同じ定義済みステージに更新したときに、そのステージに対して 2 つ目のプロジェクトが作成されます。

* [!DNL Workfront] の 1 つのプロジェクトは、常に [!DNL Salesforce] の 1 つの商談または 1 つのアカウントにのみリンクできますが、同時に両方にリンクすることはできません。

### トリガーの設定 {#configuring-triggers}

トリガーを設定すると、[!UICONTROL Salesforce Classic] または [!DNL Lightning Experience] の両方のフレームワークで [!DNL Workfront] プロジェクトの作成プロセスが有効になります。

[!UICONTROL Salesforce] でトリガーを設定するには：

1. システム管理者として [!DNL Salesforce] にログインします。
1. （条件付き）[!DNL Salesforce Classic] で、「**[!UICONTROL 設定]**」をクリックし、「**[!UICONTROL ビルド]**」セクションで&#x200B;**[!UICONTROL 稲妻]**&#x200B;を展開します。

   または

   [!DNL Salesforce] Lightning Experience で、**[!UICONTROL 設定]アイコン**、**[!UICONTROL 設定]**&#x200B;をクリックし、**[!UICONTROL プラットフォームツール]**&#x200B;で&#x200B;**[!UICONTROL アプリ]**&#x200B;を展開します。

1. **[!UICONTROL インストール済みパッケージ]**&#x200B;をクリックします。

   **[!DNL Workfront]** パッケージがインストールされます。

1. **[!DNL Workfront]** の横にある「**[!UICONTROL 設定]**」をクリックします。

1. [!DNL Workfront] にシステム管理者としてログインします。

   「**[!UICONTROL トリガー]**」ページが表示されます。

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. 「**[!UICONTROL 新規トリガー]**」をクリックします。
1. 「**[!UICONTROL [!DNL Salesforce]オブジェクト]**」ドロップダウンメニューから「**[!UICONTROL 機会]**」を選択します。

   必須フィールドです。

1. （条件付き）次の項目を指定します。

   1. 「**[!UICONTROL ステージ]**」ドロップダウンメニューから「**[!UICONTROL ステージ]**」を選択します。

      ここで指定された[!UICONTROL ステージ]に機会が到達すると、プロジェクトが [!DNL Workfront] に作成されます。必須フィールドです。

   1. 「**[!UICONTROL ポートフォリオまたはプログラム]**」フィールドで、[!DNL Workfront] 内でプロジェクトを配置するポートフォリオまたはプログラムの名前の入力を開始し、リストに表示されたらそれを選択します。\

      ポートフォリオまたはプログラムを指定しない場合、新しいプロジェクトが作成され、トリガーの設定時に [!DNL Workfront] にログインしているユーザーの[!UICONTROL 所有プロジェクト]リストに追加されます。このユーザーは、新しいプロジェクトのプロジェクト所有者でもあります。

   1. 新しい [!DNL Workfront] プロジェクトに関連付けるテンプレートの名前の入力を開始し、リストに表示されたらそれを選択します。\

      必須フィールドです。


      >[!NOTE]
      >
      >この統合に使用する予定のテンプレートにテンプレート所有者を指定している場合、それが新しいプロジェクトのプロジェクト所有者になります。新しいプロジェクトは、テンプレートに従って、新しいプロジェクトの所有者であるユーザーの[!UICONTROL 所有プロジェクト]リストの下に表示されます。

   1. （オプション）1 つの機会で販売される製品のタイプごとに新しいプロジェクトを作成する場合は、**[!UICONTROL 販売製品タイプごとに新しいプロジェクトを作成]フィールド**&#x200B;を選択します。
   1. （条件付き）「**[!UICONTROL 製品]**」ドロップダウンメニューで、「**[!UICONTROL 製品]**」を選択します。

      必須フィールドです。

   1. （条件付き）指定した製品が[!UICONTROL 機会]にある場合、新しい [!DNL Workfront] プロジェクトに関連付ける&#x200B;**[!UICONTROL テンプレート]**&#x200B;の名前の入力を開始します。名前がリストに表示されたら、選択します。

      必須フィールドです。

      新しい製品が [!DNL Salesforce] の機会に追加されるときに作成されるプロジェクトは、その機会に対して選択された同じポートフォリオまたはプログラムに配置されます。

      >[!IMPORTANT]
      >
      >プロジェクトは、[!UICONTROL 機会]でステージが更新された場合にのみ作成されます。製品が[!UICONTROL 機会]に追加されるときではなく、「ステージ」フィールドが更新されるときに、指定された製品ごとに一意のプロジェクトが作成されます。

1. （オプション）「**[!UICONTROL 新しいトリガー]**」をクリックします。
1. （オプション）「**[!UICONTROL [!DNL Salesforce]オブジェクト]**」ドロップダウンメニューから、「**アカウント
**」を選択します。

   必須フィールドです。
1. （条件付き）次の項目を指定します。

   1. 「**[!UICONTROL タイプ]**」ドロップダウンメニューから「**[!UICONTROL タイプ]**」を選択します。

      任意の「**アカウント
**」が、[!DNL Salesforce] で指定された&#x200B;**[!UICONTROL タイプ]**&#x200B;として指定されている場合、**[!UICONTROL プロジェクト]**&#x200B;が [!DNL Workfront] に作成されます。

      必須フィールドです。

   1. （オプション）「**[!UICONTROL ポートフォリオまたはプログラム]**」フィールドの [!DNL Workfront] にプロジェクトを配置する&#x200B;**[!UICONTROL ポートフォリオ]**&#x200B;または&#x200B;**[!UICONTROL プログラム]**&#x200B;の名前の入力を開始して、リストに表示されたら選択します。

      ポートフォリオまたはプログラムを指定しない場合、新しいプロジェクトが作成され、[!DNL Salesforce] から [!DNL Workfront] にログインしたユーザーの&#x200B;**[!UICONTROL 所有プロジェクト]**&#x200B;リストに追加されます。また、ユーザーは、新しいプロジェクトのプロジェクト所有者でもあります。

   1. 新しい [!DNL Workfront] プロジェクトに関連付ける&#x200B;**[!UICONTROL テンプレート]**&#x200B;の名前の入力を開始し、リストに表示されたらそれを選択します。

      必須フィールドです。

      >[!NOTE]
      >
      >この統合に使用する予定のテンプレートにテンプレート所有者を指定している場合、それが新しいプロジェクトのプロジェクト所有者になります。新しいプロジェクトは、テンプレートに従って、新しいプロジェクトの所有者であるユーザーの&#x200B;**[!UICONTROL 所有プロジェクト]**&#x200B;リストの下に表示されます。

   ![salesforce_トリガー_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   いずれかのトリガーが満たされるたびに、[!DNL Workfront] プロジェクトが生成されるようになりました。

### プロジェクト名について {#understanding-project-names}

どのトリガーがプロジェクトを生成したかに応じて、[!DNL Workfront] 内のプロジェクトの名前は次のいずれかのパターンに従います。

* プロジェクトが機会または取引先トリガーに基づいて作成された場合、プロジェクトの名前は次のようになります。*`<Salesforce object name>`：`<Project template name>`（[!DNL Salesforce] 経由）*。
* 新しい製品の追加も含まれる機会トリガーに基づいてプロジェクトが作成された場合、プロジェクトの名前は次のようになります：*`<Salesforce object name>`：`<Salesforce product name>`（[!DNL Salesforce] 経由）*。

## [!DNL Workfront] プロジェクトを表示する

[!DNL Workfront] 管理者が[!UICONTROL 機会]またはアカウント
ページレイアウトに「[!DNL Workfront]」セクションを追加した場合、このセクションの「[!UICONTROL プロジェクト]」タブで自動的に作成されたプロジェクトを確認できます。\
[!UICONTROL 機会]またはアカウント
のページレイアウトへの「[!DNL Workfront]」セクションの追加について詳しくは、[ [!DNL Salesforce]  ユーザーに「 [!DNL Adobe Workfront] 」セクションを設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

「[!UICONTROL プロジェクト]」タブを表示するには、[!DNL Workfront] アカウントを持ち、[!DNL Workfront] にログインしている必要があります。

[!UICONTROL 機会]またはアカウント
から作成されたプロジェクトを表示するには、以下の手順を実行します。

1. [!UICONTROL 機会]またはアカウント
に移動します。
1. 「**[!DNL Workfront]**」セクションに移動します。

   >[!NOTE]
   >
   >[!DNL Workfront] 管理者がこのセクションをどのように設定したかに応じて、別の名前が付けられる場合があります。

1. 「**[!UICONTROL プロジェクト]**」タブを選択します。

   定義済みのトリガーで作成されたすべてのプロジェクトがこのタブに表示されます。[!DNL Salesforce] のユーザーで、[!DNL Workfront] アカウントも持ち、[!DNL Workfront] でこれらのプロジェクトを表示する権限を持っている可能性があるユーザーは、それらを生成した[!UICONTROL 機会]またはアカウント
について [!DNL Salesforce] でもそれらを確認できます。

   統合で作成されたプロジェクトに関する次の情報を表示できます。

   * プロジェクト名
   * 参照番号
   * エントリ日
   * 所有者の名前
   * ステータス
   * 状況
   * 予定完了日
   * 完了率

     この情報が [!DNL Workfront] で更新されると、このリストで更新されたフィールドを確認できます。

1. （オプション）プロジェクトの名前をクリックして、Workfront で開きます。
1. （オプション）[!UICONTROL プロジェクト詳細]エリアまたはプロジェクトヘッダーの「[!UICONTROL **[!UICONTROL Salesforce に移動」]**]をクリックして、プロジェクトが開始された[!UICONTROL 機会]またはアカウント
にアクセスします。システム管理者またはグループ管理者は、プロジェクトヘッダーで「[!UICONTROL 統合]」フィールドを見つけるためにレイアウトテンプレートにそのフィールドを追加する必要があります。

   >[!NOTE]
   >
   >「[!UICONTROL Salesforce に移動]」リンクは、プロジェクトを表示できるすべての [!DNL Workfront] ユーザーに表示されます。プロジェクトが生成された [!DNL Salesforce] の機会またはアカウントに移動するには、[!DNL Salesforce] アカウントが必要です。
