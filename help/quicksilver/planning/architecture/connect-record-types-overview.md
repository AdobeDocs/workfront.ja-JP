---
title: レコードタイプの接続：概要
description: 個々のレコードタイプが互いにどのように関連しているかは、レコードタイプを連結するとよくわかります。また、Workfront Planning のレコードタイプを他のアプリケーションのオブジェクトタイプに接続して、ユーザーのエクスペリエンスを向上させ、ユーザーが 1 つのアプリケーションに集中できるようにすることもできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 36%

---


<!--update metadata at GA-->
<!--add to TOC and mini TOC when live-->

# レコードタイプの接続：概要

個々のレコードタイプを相互に関連付けたり、他のアプリケーションのオブジェクトに接続して関連付けることができます。

この記事では、レコードタイプの接続方法の概要と、レコードタイプとオブジェクトタイプの間で確立できる接続のタイプについて説明します。

レコードタイプの接続について詳しくは、[ レコードタイプの接続 ](/help/quicksilver/planning/architecture/connect-record-types.md) を参照してください。

## レコードタイプの連結に関する考慮事項

* Workfront Planning では、次のエンティティを接続できます。

   * 2 つのレコードタイプ

     レコードタイプは、同じワークスペースに属している必要があります。
   * 1 つのレコードタイプと、別のアプリケーションの 1 つのオブジェクトタイプ

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

     >[!IMPORTANT]
     >
     >Adobe Experience Manager Assets ライセンスが必要です。Workfront Planning レコードを Adobe Experience Manager Assets に接続するには、組織の Workfront インスタンスを Adobe Business Platform または Adobe Admin Console にオンボーディングする必要があります。
     >
     >Adobe Admin Console のオンボーディングについて質問がある場合は、[Adobe Unified Experience の FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md) を参照してください。

* レコードタイプの個々のレコードを作成した後、リンクされたレコードタイプのフィールドから接続先のレコードを選択できます。詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

* レコードタイプを別のレコードタイプに接続するか、別のアプリケーションのオブジェクトタイプに接続すると、次のシナリオが存在します。

   * **2 つのレコードタイプを接続する場合**：接続元のレコードタイプに、リンクされたレコードフィールドが作成されます。接続先のレコードタイプに、同様のリンクされたレコードフィールドが作成されます。

     例えば、「キャンペーン」レコードタイプを「製品」レコードタイプに関連付けると、「リンクされた製品」という名前のリンクされたレコードフィールドがキャンペーンレコードタイプに作成されます。 製品レコードタイプに、「キャンペーン」という名前のリンクされたレコードタイプが自動的に作成されます。

   * **レコードタイプを別のアプリケーションのオブジェクトタイプに接続する場合**

      * リンクされたレコードフィールドは、接続元のレコードタイプで作成されます。 他のアプリケーションのオブジェクトタイプには、リンクされたレコードフィールドが自動的に作成されません。

      * 計画レコードフィールドには、Workfront オブジェクトからアクセスできません。
      * Workfront管理者がWorkfrontとAdobe Experience Manager Assetsの統合を通じてメタデータマッピングを設定すると、Experience Managerのアセットから計画レコードフィールドにアクセスできます。 詳しくは、[Adobe WorkfrontとExperience Manager Assets間のアセットメタデータのマッピングの設定 ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=ja) を参照してください。

   * **接続先のレコードまたはオブジェクトからリンクされた（またはルックアップ）フィールドを追加する場合**：接続先のレコードの情報を含むリンクされた（またはルックアップ フィールド）が、接続先のレコードに表示されます。

     他のレコードタイプまたは別のアプリケーションのオブジェクトのフィールドを、Workfront Planning レコードタイプに関連付けることができます。

     リンクされたフィールドは読み取り専用で、レコードまたはオブジェクトを接続すると、接続されたレコードまたはオブジェクトの情報が自動的に表示されます。

     例えば、「キャンペーン」レコードタイプを Workfront プロジェクトに接続し、プロジェクトの「予定完了日」フィールドを Workfront Planning レコードに取り込むと、キャンペーンに対して（プロジェクトからの）「予定完了日」という名前のリンクされたフィールドが自動的に作成されます。このリンクされたフィールドを手動で編集することはできません。（プロジェクトからの）「予定完了日」フィールドには、リンクされたプロジェクトの予定完了日が表示されます。

     >[!IMPORTANT]
     >
     >ワークスペースに対する表示権限以上の権限を持つユーザーは、リンクされたオブジェクトタイプのアプリケーションでの権限やアクセスレベルに関係なく、リンクされたフィールドの情報を表示できます。

* リンクされたレコードフィールドの前には関係アイコン ![](assets/relationship-field-icon.png) が付きます。

  リンクされたフィールドの前には、フィールドタイプを識別するアイコンが付きます。例えば、リンクされた（または参照）フィールドの前には、フィールドが数値、段落、または日付であることを示すアイコンが付きます。

* 参照フィールドの前には、フィールドに表示される情報のタイプを示すアイコンが付きます。

## 接続タイプ

2 つのレコードタイプ間、または別のアプリケーションのレコードとオブジェクトタイプ間の接続を確立した後、接続されたレコードフィールドにレコードを追加できます。

接続に追加できるレコードの数に応じて、レコードタイプを接続するときに選択できる接続タイプは次のとおりです。

* [1 対多](#one-to-many-connection-type)
* [1 対 1](#many-to-one-connection-type)
* [多対 1](#many-to-one-connection-type)
* [多対多](#many-to-many-connection-type)

<!-- add screen shots for each type of connection below-->

### 1 対多接続タイプ

レコードタイプ間で 1 対多の接続タイプを選択した場合、後で 1 つのレコードを複数の接続先レコードに接続できます。

例えば、キャンペーンをプロジェクトと接続する場合は、1 つのキャンペーンを複数のプロジェクトと接続できます。 ただし、1 つのプロジェクトを 1 つのキャンペーンにのみ接続できます。

この接続タイプを選択した場合は、後で多対多の接続タイプにのみ変更できます。

### 1 対 1 の接続タイプ

レコードタイプ間で 1 対 1 の接続タイプを選択した場合、後で 1 つのレコードを接続先の他の 1 つのレコードに接続できます。

例えば、キャンペーンをプロジェクトと結び付ける場合、1 つのキャンペーンを 1 つのプロジェクトと結び付けることができます。 1 つのプロジェクトを 1 つのキャンペーンにのみ接続できます。

この接続の種類を選択すると、後で他の接続の種類に変更できます。

### 多対 1 接続タイプ

レコードタイプ間で多対 1 の接続タイプを選択した場合、後で接続先のレコードが 1 つだけの多数のレコードを接続できます。

例えば、キャンペーンをプロジェクトに接続する場合、複数のキャンペーンを 1 つのプロジェクトに接続できます。 1 つのプロジェクトを複数のキャンペーンに接続できます。

この接続タイプを選択した場合は、後で多対多の接続タイプにのみ変更できます。

### 多対多接続タイプ

レコードタイプ間で多対多の接続タイプを選択した場合、後で、接続先の複数のレコードを持つ多くのレコードを接続できます。

例えば、キャンペーンをプロジェクトに接続する場合、複数のキャンペーンを複数のプロジェクトに接続できます。 また、複数のプロジェクトを複数のキャンペーンに接続することもできます。

この接続の種類を選択すると、保存した後で接続の種類を変更することはできません。