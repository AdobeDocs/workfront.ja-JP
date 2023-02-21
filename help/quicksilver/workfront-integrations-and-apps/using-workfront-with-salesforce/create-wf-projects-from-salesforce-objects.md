---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: 作成 [!DNL Adobe Workfront] プロジェクトから [!DNL Salesforce] オブジェクト
description: インストール後 [!DNL Adobe Workfront] Salesforce の場合は、 [!DNL Workfront] プロジェクト [!DNL Salesforce] 商談とアカウント。
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1506'
ht-degree: 3%

---

# 作成 [!DNL Adobe Workfront] プロジェクトから [!DNL Salesforce] オブジェクト

インストール後 [!DNL Adobe Workfront] Salesforce の場合は、 [!DNL Workfront] プロジェクト [!DNL Salesforce] [!UICONTROL 商談] および [!UICONTROL アカウント].

## アクセス要件

この記事で説明する機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

次の手順で [!DNL Workfront] からのリクエスト [!DNL Salesforce] [!UICONTROL 商談] またはアカウントを使用して、環境に次の設定があることを確認します。

* お使いの [!DNL Workfront] 管理者がインストール済み [!DNL Workfront for Salesforce].\
   インストールの詳細 [!DNL Workfront for Salesforce]を参照してください。 [インストール [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* お使いの [!DNL Workfront] 管理者が [!DNL Workfront] セクションで [!UICONTROL 商談] およびアカウントページレイアウト\
   詳しくは、 [!DNL Workfront] セクションをページレイアウトに追加する場合は、 [の設定 [!DNL Adobe Workfront] セクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 次の条件を満たしている： [!DNL Workfront] アカウントを使用し、 [!DNL Workfront] セクションを [!UICONTROL 商談] またはアカウント。

## 作成の設定 [!DNL Workfront] プロジェクト元 [!DNL Salesforce]

* [プロジェクトの自動作成について](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [設定トリガー](#configuring-triggers-configuring-triggers)
* [プロジェクト名について](#understanding-project-names-understanding-project-names)

### プロジェクトの自動作成について {#understanding-the-automatic-creation-of-projects}

を [!DNL Salesforce] システム管理者は、でプロジェクトを自動的に作成できるトリガーを定義できます。 [!DNL Workfront] で次のことが起こった場合 [!DNL Salesforce]:

* この [!UICONTROL ステージ] の [!UICONTROL 商談] が更新されました。
* この [!UICONTROL タイプ] の数が更新されました。

トリガーは、 [!DNL Workfront for Salesforce].  \
インストールに関する情報 [!DNL Workfront for Salesforce]を参照してください。 [インストール [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

自動的に作成するトリガーを設定する際は、次の点を考慮してください [!DNL Workfront] 次の場合にプロジェクト [!DNL Salesforce] 項目が作成または更新されました：

* 次の条件を満たす必要があります。 [!DNL Salesforce] および [!DNL Workfront] システム管理者：トリガーを設定します。
* 設定後、すべてのトリガーが [!UICONTROL ステージ] の [!UICONTROL 商談] または [!UICONTROL タイプ] アカウントのトリガーに、 [!DNL Workfront] プロジェクト。 これには以下が含まれます。 [!DNL Salesforce] ユーザーの [!DNL Workfront] アカウント
* 使用できるトリガー数に制限はありません。
* 同じ条件に基づいて複数のトリガーを作成することはできません。 トリガーは、デフォルトで一意です。
* プロジェクトを作成すると、そのプロジェクトは自動的にオポチュニティまたは生成されたアカウントにリンクされます。 一旦確立すると、このリンクは切断できません。
* 1 つのオポチュニティまたはアカウントを [!DNL Workfront] トリガーされた条件が、オポチュニティまたはアカウントの存続期間中に複数回満たされた場合。

   例えば、複数の [!UICONTROL ステージ] の [!UICONTROL 商談] プロジェクトをトリガーするには、オポチュニティが到達する定義済みのステージごとに、そのオポチュニティの存続期間中にプロジェクトが作成されます。 また、 [!UICONTROL ステージ] の [!UICONTROL 商談] 定義されたステージから別のステージに移動し、定義されたステージに戻ると、2 回目に更新したときに 2 つ目のプロジェクトが作成されます。 [!UICONTROL ステージ] フィールドを同じ定義済みステージに追加します。

* の 1 つのプロジェクト [!DNL Workfront] は、 [!DNL Salesforce] いつでも同時にではなく、両方に対して同時にではありません。

### 設定トリガー {#configuring-triggers}

設定が完了すると、トリガーの作成プロセスが [!DNL Workfront] 両方に対してプロジェクトが有効です [!UICONTROL Salesforce Classic] または [!DNL Lightning Experience] フレームワーク

でトリガーを設定するには [!UICONTROL Salesforce]:

1. にログインします。 [!DNL Salesforce] をシステム管理者として設定します。
1. （条件付き）で [!DNL Salesforce Classic]をクリックし、 **[!UICONTROL 設定]**、および **[!UICONTROL ビルド]** セクション、展開 **[!UICONTROL 稲妻]**.

   または

   In [!DNL Salesforce] Lightning Experience で、 **[!UICONTROL 設定] アイコン**&#x200B;を、 **[!UICONTROL 設定]**&#x200B;および **[!UICONTROL PLATFORM ツール]** 展開 **[!UICONTROL アプリ]**.

1. クリック **[!UICONTROL インストール済みパッケージ]**.

   この **[!DNL Workfront]** パッケージがインストールされました。

1. クリック **[!UICONTROL 設定]** 次の **[!DNL Workfront]**.

1. にログインします。 [!DNL Workfront] をシステム管理者として設定します。

   この **[!UICONTROL トリガー]** ページが表示されます。

   ![salesforce_トリガー_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. クリック **[!UICONTROL 新規トリガー]**.
1. 次の **[!UICONTROL [!DNL Salesforce]オブジェクト]** ドロップダウンメニューで、「 **[!UICONTROL 商談]**.

   必須フィールドです。

1. （条件付き）次の項目を指定します。

   1. 次の **[!UICONTROL ステージ]** ドロップダウンメニューで、 **[!UICONTROL ステージ]**.\

      商談が [!UICONTROL ステージ] ここで指定した場合、 [!DNL Workfront]. 必須フィールドです。

   1. 内 **[!UICONTROL Portfolioまたはプログラム]** フィールドに、プロジェクトを配置するPortfolioまたはプログラムの名前を入力します [!DNL Workfront]」をクリックし、リストに表示されたら選択します。\

      Portfolioまたはプログラムを指定しない場合、新しいプロジェクトが作成され、 [!UICONTROL 自分が所有するプロジェクト] 次にログインしたユーザーのリスト： [!DNL Workfront] トリガー このユーザーは、新しいプロジェクトのプロジェクト所有者でもあります。

   1. 新しいテンプレートに関連付けるテンプレートの名前の入力を開始します [!DNL Workfront] プロジェクトを選択し、リストに表示されたら選択します。\

      必須フィールドです。


      >[!NOTE]
      >
      >この統合で使用するテンプレートに対してテンプレート所有者を指定した場合、その所有者が新しいプロジェクトのプロジェクト所有者になります。 新しいプロジェクトが [!UICONTROL 自分が所有するプロジェクト] テンプレートに従った、新しいプロジェクトの所有者であるユーザーのリスト。

   1. （オプション） **[!UICONTROL 販売した各製品タイプに対して新しいプロジェクトを作成] フィールド**&#x200B;任意の 1 つのオポチュニティで販売されるすべてのタイプの製品の新しいプロジェクトを作成する場合。
   1. （条件付き） **[!UICONTROL 製品]** 内 **[!UICONTROL 製品]** ドロップダウンメニュー。

      必須フィールドです。

   1. （条件付き）名前の入力を開始する **[!UICONTROL テンプレート]** 新しい [!DNL Workfront] 指定した製品が [!UICONTROL 商談]. リストに表示される場合に選択します。

      必須フィールドです。

      新しい製品をに追加したときに作成されるプロジェクト [!DNL Salesforce] 商談が、商談に対して選択された同じPortfolioまたはプログラムに配置されています。

      >[!IMPORTANT]
      >
      >プロジェクトは、 [!UICONTROL 商談]. 製品がに追加されるのではなく、「ステージ」フィールドの更新時に指定された製品ごとに一意のプロジェクトが作成されます。 [!UICONTROL 商談].

1. （オプション）「 **[!UICONTROL 新規トリガー]**.
1. （オプション） **[!UICONTROL [!DNL Salesforce]オブジェクト]** ドロップダウンメニューから「**アカウント**」を選択します。

   必須フィールドです。
1. （条件付き）次の項目を指定します。

   1. を選択します。 **[!UICONTROL タイプ]** から **[!UICONTROL タイプ]** ドロップダウンメニュー。

      **アカウント**が **[!UICONTROL タイプ]** ここで指定 [!DNL Salesforce], a **[!UICONTROL プロジェクト]** 次で作成： [!DNL Workfront].

      必須フィールドです。

   1. （オプション）名前の入力を開始する **[!UICONTROL Portfolio]** または **[!UICONTROL プログラム]** プロジェクトを配置する場所 [!DNL Workfront] 内 **[!UICONTROL Portfolioまたはプログラム]** フィールドに値を入力し、リストに表示されるときに選択します。

      Portfolioまたはプログラムを指定しない場合、新しいプロジェクトが作成され、 **[!UICONTROL 自分が所有するプロジェクト]** 次にログインしたユーザーのリスト： [!DNL Workfront] から [!DNL Salesforce]. また、ユーザーは、新しいプロジェクトのプロジェクト所有者でもあります。

   1. 名前の入力を開始 **[!UICONTROL テンプレート]** 新しい [!DNL Workfront] プロジェクトを選択し、リストに表示されたら選択します。

      必須フィールドです。

      >[!NOTE]
      >
      >この統合で使用するテンプレートに対してテンプレート所有者を指定した場合、その所有者が新しいプロジェクトのプロジェクト所有者になります。 新しいプロジェクトが **[!UICONTROL 自分が所有するプロジェクト]** テンプレートに従った、新しいプロジェクトの所有者であるユーザーのリスト。
   ![salesforce_トリガー_page_with_cleaned_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   [!DNL Workfront] プロジェクトは、どのトリガーも満たすたびに生成されます。

### プロジェクト名について {#understanding-project-names}

プロジェクトを生成したトリガーに応じて、 [!DNL Workfront] は、次のいずれかのパターンに従うことができます。

* オポチュニティまたはアカウントトリガーに基づいてプロジェクトを作成した場合、プロジェクトの名前は次のようになります。 *`<Salesforce object name>`: `<Project template name>` ( [!DNL Salesforce])*.
* 新しい製品の追加も含む商談トリガーに基づいてプロジェクトが作成される場合、プロジェクトの名前は次のようになります。 *`<Salesforce object name>`: `<Salesforce product name>` ( [!DNL Salesforce])*.

## 表示 [!DNL Workfront] プロジェクト

次に、 [!DNL Workfront] 管理者が [!DNL Workfront] セクションで [!UICONTROL 商談] またはアカウントページレイアウトを使用すると、 [!UICONTROL プロジェクト] 」タブをクリックします。\
詳しくは、 [!DNL Workfront] セクションを [!UICONTROL 商談] またはアカウントについては、 [の設定 [!DNL Adobe Workfront] セクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

次をお持ちの場合は、 [!DNL Workfront] アカウントにログインし、 [!DNL Workfront] 表示する [!UICONTROL プロジェクト] タブをクリックします。

から作成されたプロジェクトを表示するには [!UICONTROL 商談] またはアカウント：

1. 次に移動： [!UICONTROL 商談] またはアカウント。
1. 次に移動： **[!DNL Workfront]** 」セクションに入力します。

   >[!NOTE]
   >
   >使用する [!DNL Workfront] 管理者がこのセクションを設定しました。別の名前を使用している可能性があります。

1. を選択します。 **[!UICONTROL プロジェクト]** タブをクリックします。

   定義済みのプロジェクトで作成されたすべてのトリガーがこのタブに表示されます。 の任意のユーザー [!DNL Salesforce] 同じく [!DNL Workfront] アカウントと、これらのプロジェクトをで表示する権限を持つユーザー [!DNL Workfront] また、 [!DNL Salesforce] の [!UICONTROL 商談] または生成したアカウント。

   統合で作成されたプロジェクトに関する次の情報を表示できます。

   * プロジェクト名
   * 参照番号
   * エントリ日
   * 所有者の名前
   * ステータス
   * 状況
   * 予定完了日
   * 完了率

      この情報が [!DNL Workfront]をクリックすると、このリストで更新されたフィールドを確認できます。

1. （オプション）プロジェクトの名前をクリックして、Workfrontで開きます。
1. （オプション）「 [!UICONTROL **[!UICONTROL Salesforce に移動]**] 内 [!UICONTROL プロジェクトの詳細] 領域、または [!UICONTROL 商談] またはプロジェクトが開始されたアカウント システム管理者またはグループ管理者が [!UICONTROL 統合] フィールドをレイアウトテンプレートに追加して、プロジェクトのヘッダーに表示します。

   >[!NOTE]
   >
   >この [!UICONTROL Salesforce に移動] リンクはすべてのに対して表示されます [!DNL Workfront] プロジェクトを表示できるユーザー。 次をお持ちの場合は、 [!DNL Salesforce] 次にアクセスできるアカウント [!DNL Salesforce] プロジェクトが生成された商談またはアカウント。
