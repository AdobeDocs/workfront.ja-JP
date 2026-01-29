---
title: 接続されたレコードタイプの概要
description: 個々のレコードタイプが互いにどのように関連しているかは、レコードタイプを連結するとよくわかります。また、Workfront Planning のレコードタイプを他のアプリケーションのオブジェクトタイプに接続して、ユーザーのエクスペリエンスを向上させ、ユーザーが 1 つのアプリケーションに集中できるようにすることもできます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: 29579097cd3aa75ab0478743b84dcb9bc3217489
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 9%

---


<!--keep the 30 limit verbiage in yellow til Jan 2026-->

# 接続されたレコードタイプの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   -->

個々のレコードタイプを相互に関連付けたり、他のアプリケーションのオブジェクトに接続して関連付けることができます。

この記事では、レコードタイプ接続の概要を説明し、レコードタイプとオブジェクトタイプの間で確立できる接続のタイプについて説明します。

レコードタイプの接続について詳しくは、[&#x200B; レコードタイプの接続 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md) を参照してください。

## レコードタイプの連結に関する考慮事項

* 個々のレコードまたはオブジェクトを相互に接続するには、まずレコード タイプをオブジェクト タイプに接続する必要があります。

  レコードタイプとオブジェクトタイプは、次の方法で相互に接続できます。

   * 手動
   * 自動

  >[!NOTE]
  >
  >Workfront Planning には、1 つのレコードタイプに対して最大 30 個の接続されたフィールドを持つことができます。


* レコードタイプとオブジェクトタイプの接続については、次の点を考慮してください。

   * レコードタイプから手動で「新規接続」フィールドを追加して、Workfront Planning 内の次のエンティティを接続できます。

      * 2 つのレコードタイプ

        デフォルトでは、同じワークスペースから 2 つのレコードタイプを接続できます。 上位のWorkfrontまたは Planning パッケージを購入した場合は、他のワークスペースのレコードタイプと連携するようにレコードタイプを設定することもできます。 詳しくは、[&#x200B; レコードタイプの編集 &#x200B;](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。
      * 1 つのレコードタイプと、別のアプリケーションの 1 つのオブジェクトタイプ

     レコードタイプとオブジェクトタイプを接続する方法については、[&#x200B; レコードタイプの接続 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md) を参照してください。

     レコードの種類を他のレコードまたはオブジェクトの種類に手動で接続した後、個々のレコードおよびオブジェクトを接続できます。

     詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

   * エンティティ間の接続は、次のシナリオで自動的に確立されます。

      * 自動化を使用してレコードタイプのページからレコードを作成する場合。

        オートメーションが接続されたレコードまたはオブジェクトを作成すると、レコードの種類またはレコードの種類と他のアプリケーションのオブジェクトの種類との間の接続が自動的に作成されます。

        詳しくは、[Adobe Workfront Planning の自動設定の構成 &#x200B;](/help/quicksilver/planning/records/configure-automations-to-create-records.md) を参照してください。

      * レコードタイプのリクエストフォームを設定してレコードまたはオブジェクトを作成する場合。

        レコード・タイプと要求オブジェクト・タイプ間の接続は、レコードを作成する Planning 要求を発行および承認すると自動的に作成されます。

        詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの発行 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

        元のリクエストは、Workfront<!--, <span class="preview">or in the Original Request connection field in Workfront Planning.</span>--> の「リクエスト」領域で確認できます。

   * Workfrontの計画レコードタイプを次のアプリケーションの次のオブジェクトタイプと結び付けることができます。

      * Adobe Workfront:

         * プロジェクト
         * ポートフォリオ
         * プログラム
         * 会社
         * グループ

      * Adobe Experience Manager Assets：

         * 画像
         * フォルダー

      * Adobe GenStudio for Performance Marketing

         * ブランド

        >[!IMPORTANT]
        >
        >Adobe Experience Manager AssetsおよびGenStudio Brands に接続するには、以下が必要です。
        >* Adobe Experience Manager Assets ライセンス
        >* Adobe GenStudio for Performance Marketing ライセンス
        >* Workfront Planning レコードをWorkfrontに接続するには、組織のAdobe Experience Manager Assets インスタンスをAdobe Business Platform またはAdobe Admin Consoleにオンボーディングする必要があります。
        >Adobe Admin Consoleについて詳しくは、[Adobe統合エクスペリエンス FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md) を参照してください。

* 別のアプリケーションから 2 つのレコードタイプまたはレコードタイプとオブジェクトタイプが接続されている場合、次のシナリオが発生します。

   * **2 つの Planning レコードタイプを接続する場合**：リンクされたレコードフィールドは、接続元のレコードタイプで作成されます。 同様のリンクされたレコードフィールドは、接続先のレコードタイプで作成されます。「新しい接続」タブの「リンクされたレコードタイプに対応するフィールドを作成」設定を有効にした場合にのみ作成されます。

     例えば、「キャンペーン」レコードタイプを「製品」レコードタイプに接続すると、「リンクされた製品」という名前のリンクされたレコードフィールド（接続フィールド）がキャンペーンレコードタイプに作成されます。 製品レコードタイプに、「キャンペーン」という名前のリンクされたレコードタイプが自動的に作成されます。

     例えば、次のようなシナリオが存在します。

      * 「リンクされたレコードタイプに対応するフィールドを作成」設定を有効にし、「キャンペーン」レコードタイプを「製品」レコードタイプに接続すると、「リンクされた製品」と名前が付いたリンクされたレコードフィールド（接続フィールド）がキャンペーンレコードタイプに作成されます。 製品レコードタイプに、「キャンペーン」という名前のリンクされたレコードタイプが自動的に作成されます。
      * 「リンクされたレコードタイプに対応するフィールドを作成」設定を無効にして、「キャンペーン」レコードタイプを「製品」レコードタイプに接続すると、「リンクされた製品」と名前が付いたリンクレコードフィールド（接続フィールド）がキャンペーンレコードタイプに作成されます。 製品レコードタイプに「キャンペーン」という名前のリンクされたレコードタイプが自動的に作成されません。

     詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

   * **レコードタイプを別のアプリケーションのオブジェクトタイプに接続する場合**

      * リンクされたレコードフィールドは、接続元のレコードタイプで作成されます。 他のアプリケーションのオブジェクトタイプには、リンクされたレコードフィールドが自動的に作成されません。
      * 計画レコードフィールドには、Workfront オブジェクトからアクセスできません。
      * 計画レコードは、Workfront オブジェクトの計画セクションに表示されます。 詳しくは、[Workfront オブジェクトからのレコード接続の管理 &#x200B;](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。
      * Planning 接続のカスタムフィールドを作成して、Workfront オブジェクトのカスタムフォームに添付できます。 詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。
      * WorkfrontとExperience Managerの統合を通じてWorkfront管理者がメタデータマッピングを設定すると、Adobe Experience Manager Assets Assets から計画レコードフィールドにアクセスできます。 詳しくは、[Adobe WorkfrontとExperience Manager Assets間のアセットメタデータのマッピングの設定 &#x200B;](https://experienceleague.adobe.com/ja/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) を参照してください。
      * 計画レコードフィールドは、GenStudio for Performance Marketingのブランドからアクセスできません。

   * **接続先のレコードまたはオブジェクトからルックアップ フィールドを追加する場合**: リンクされたレコード フィールドを作成する以外に、ルックアップ フィールドと呼ばれる接続されたレコードまたはオブジェクト タイプのフィールドにも接続できます。 接続先のレコードの情報とリンクされた（またはルックアップ フィールド）が、接続先のレコードに表示されます。

     他のレコードタイプまたは別のアプリケーションのオブジェクトのフィールドを、Workfront Planning レコードタイプに関連付けることができます。

     リンクされたフィールドは読み取り専用で、接続されたレコードの情報が自動的に表示されます。

     式、フィルター、またはグループ化で、他のレコードまたはオブジェクト タイプのルックアップ フィールドを参照できます。

     例えば、「キャンペーン」レコードタイプを Workfront プロジェクトに接続し、プロジェクトの「予定完了日」フィールドを Workfront Planning レコードに取り込むと、キャンペーンに対して（プロジェクトからの）「予定完了日」という名前のリンクされたフィールドが自動的に作成されます。このリンクされたフィールドを手動で編集することはできません。（プロジェクトからの）「予定完了日」フィールドには、リンクされたプロジェクトの予定完了日が表示されます。

     >[!IMPORTANT]
     >
     >ワークスペースに対する表示以上のアクセス権を持つすべてのユーザーは、リンク オブジェクトの種類のアプリケーションでのアクセス権またはアクセス レベル、または他のワークスペースでのアクセス権に関係なく、ルックアップ フィールドの情報を表示することができます。

     リンクされたレコードフィールドの前には、関係アイコン ![&#x200B; 関係フィールドアイコン &#x200B;](assets/relationship-field-icon.png) が付きます。

     リンクされたフィールドの前には、フィールドタイプを識別するアイコンが付きます。例えば、リンクされた（または参照）フィールドの前には、フィールドが数値、段落、または日付であることを示すアイコンが付きます。

     >[!TIP]
     >
     >Workfront オブジェクトの日付フィールドの情報は、Workfront Planning では、Workfrontでの表示方法に関係なく、24 時間形式で表示されます。
     >
     >例えば、プロジェクトの予定開始日がWorkfrontで午後 3:00 と表示された場合、Workfront Planning の読み込まれた参照フィールドでは 15:00 と表示されます。

   * Workfront Planning で階層を作成するには、レコード・タイプを関連付ける必要があります。 レコードタイプの接続が存在しない場合は、階層の作成時に自動的に作成されます。 詳しくは、[&#x200B; ワークスペース階層の作成 &#x200B;](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) を参照してください。


## 接続タイプ

2 つのレコードタイプ間、または別のアプリケーションのレコードとオブジェクトタイプ間の接続を確立した後、接続されたレコードフィールドにレコードを追加できます。

>[!WARNING]
>
>この節で説明するオプションは、次の接続では使用できません。
>
>* 異なるワークスペースの 2 つのレコード
>
>* レコードタイプとExperience Manager アセット
>
>* レコードタイプとAdobe GenStudio ブランド

一度に 1 つのレコードを複数のレコードに接続するか、一度に 1 つのレコードを相互に接続するかを選択できます。

レコードタイプを接続する際に選択できる接続タイプは次のとおりです。

* **リンクされたレコードタイプに対応するフィールドを作成** 設定が無効になっている場合は、次から選択できます。

   * [複数選択](#multi-select-connection-type)
   * [単一選択](#single-select-connection-type)

* **リンクされたレコードタイプに対応するフィールドを作成** 設定が有効になっている場合は、次から選択できます。

   * [多対多](#many-to-many-connection-type)
   * [1 対多](#one-to-many-connection-type)
   * [多対 1](#many-to-one-connection-type)
   * [1 対 1](#many-to-one-connection-type)

### 接続タイプを複数選択

![&#x200B; 複数選択の接続タイプ &#x200B;](assets/multi-select-connection-picker.png)

レコードタイプ間に複数選択接続を作成すると、元のレコードタイプから接続フィールドで複数の接続レコードを選択できます。

例えば、キャンペーンとプロジェクトの間に複数選択接続を作成した場合、1 つのキャンペーンに対して複数のプロジェクトを選択できます。 プロジェクト オブジェクト タイプに対して、キャンペーンに接続されたレコード タイプが作成されません。

この接続の種類を選択した後は、次のいずれかの種類に保存すると、接続の種類を変更できなくなります。

* 単一選択
* 1 対多
* 多対 1
* 1 対 1

### 単一選択の接続タイプ

![&#x200B; 単一選択接続タイプ &#x200B;](assets/single-select-connection-picker.png)

レコードタイプ間に単一選択の接続を作成すると、元のレコードタイプから接続フィールドの 1 つのレコードを選択できます。

例えば、キャンペーンと会社の間に単一選択の接続を作成する場合、1 つのキャンペーンに対して 1 つの会社を選択できます。 会社オブジェクトタイプに対して、キャンペーンに接続されたレコードタイプが作成されません。

この接続の種類を選択した後で、次のいずれかに保存すると、接続の種類を変更できなくなります。

* 1 対多
* 1 対 1

<!--
* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)
-->

### 多対多接続タイプ

![&#x200B; 多対多の接続ピッカー &#x200B;](assets/many-to-many-connection-picker.png)

レコードタイプ間に多対多の接続を作成すると、両方のレコードタイプの接続フィールドで複数のレコードを選択できます。

例えば、キャンペーンとプロジェクトの間に多対多の接続を作成する場合、キャンペーンごとに複数のプロジェクトを選択し、プロジェクトごとに複数のキャンペーンを選択できます。

多対多の関係タイプの実際の例は、映画と俳優の関係です。 各映画は複数の俳優を持つことができ、各俳優は複数の映画で再生できます。

この接続の種類を選択すると、保存した後で接続の種類を変更することはできません。

### 1 対多接続タイプ

![1 対多接続ピッカー &#x200B;](assets/one-to-many-connection-picker.png)


レコードタイプ間に 1 対多の接続を作成すると、現在のレコードタイプの「接続」フィールドで複数のレコードを選択できますが、接続先のレコードタイプの対応する「接続」フィールドでは、1 つのレコードしか選択できません。 2 番目のレコードタイプで自動的に作成される接続済みレコードフィールドは、自動的に多対 1 の関係タイプに設定されます。

例えば、キャンペーンとプロジェクトの間に 1 対多の接続を作成した場合、キャンペーンごとに複数のプロジェクトを選択できますが、各プロジェクトを接続できるキャンペーンは 1 つだけです。

一対多の関係タイプの実際の例は、ライブラリとブックの関係です。ライブラリにはインベントリ内に多数のブックがありますが、特定のブックは特定の時点で 1 つのライブラリにのみ存在できます。

この接続タイプを選択した場合は、後で多対多の接続タイプにのみ変更できます。

### 多対 1 接続タイプ

![&#x200B; 多対 1 の接続ピッカー &#x200B;](assets/many-to-one-connection-picker.png)


レコードタイプ間に多対 1 の接続を作成すると、現在のレコードタイプの各レコードを、接続されたレコードタイプの 1 つのレコードのみで接続できます。 2 番目のレコードタイプで自動的に作成される接続済みレコードフィールドは、1 対多の関係タイプに自動的に設定されます。

例えば、キャンペーンをプロジェクトと結び付け、このタイプの接続を選択した場合、キャンペーンに追加できるプロジェクトは 1 つだけです。 ただし、複数のキャンペーンを 1 つのプロジェクトに追加できます。

多対一の関係タイプの実際の例は、多数の映画と 1 人の俳優の関係です。1 人の俳優は多数の映画に出演できますが、各映画はキャストに特定の俳優を出演させるのは 1 回だけです。

この接続タイプを選択した場合は、後で多対多の接続タイプにのみ変更できます。

### 1 対 1 の接続タイプ

![1 対 1 の接続ピッカー &#x200B;](assets/one-to-one-connection-picker.png)

レコードタイプ間で 1 対 1 の接続を作成する場合、両方のレコードタイプで、各レコードを他のレコードタイプの 1 つのレコードにのみ接続できます。

例えば、キャンペーンとプロジェクトを接続してこのタイプの接続を選択した場合、1 つのキャンペーンを 1 つのプロジェクトに接続できます。 1 つのプロジェクトを 1 つのキャンペーンにのみ接続できます。

1 対 1 の関係の実際の例としては、ある人物とその国の一意の ID （社会保障番号、パスポート ID、地域の ID ID など）の間に存在する関係が挙げられます。各人物は 1 つの国に 1 つの一意の ID しか持たず、各一意の ID は 1 人の人物にのみリンクできます。

この接続の種類を選択すると、後で他の接続の種類に変更できます。
