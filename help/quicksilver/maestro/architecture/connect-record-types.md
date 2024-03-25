---
title: レコードタイプを接続
description: 個々のレコードの種類を相互に関連付ける方法を示すには、レコードの種類を接続します。 また、Adobe Workfront Planning のレコードタイプを他のアプリケーションのオブジェクトタイプと接続して、ユーザーのエクスペリエンスを向上させ、1 つのアプリケーションにフォーカスし続けることもできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 2%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Adobe Workfront planning record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# レコードタイプを接続

{{maestro-important-intro}}

Adobe Workfront Planning を使用して、組織で必要なレコードタイプを含む完全にカスタマイズ可能なワークスペースをデザインできます。 個々のレコードの種類を相互に関連付ける方法を示すには、レコードの種類を接続します。 また、Workfront Planning のレコードタイプを他のアプリケーションのオブジェクトタイプと接続して、ユーザーのエクスペリエンスを向上させ、1 つのアプリケーションにフォーカスし続けることもできます。

レコードの種類を相互に接続したり、他のアプリケーションのオブジェクトの種類を使用してレコードの種類を接続したりできます。

これにより、Workfront Planning レコードにリンクされたレコードまたはオブジェクトタイプのフィールドを表示できます。

この記事では、Workfront計画で 2 つのレコードタイプまたはレコードタイプを、別のアプリケーションのオブジェクトと接続する方法について説明します。

レコードまたはオブジェクトタイプ間の接続を確立した後、個々のレコードを相互に接続できます。

別のアプリケーションからWorkfront計画レコードをオブジェクトに接続する方法については、 [レコードを接続](../records/connect-records.md).

レコードタイプを接続する例については、 [レコードタイプとレコードの接続例](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Adobe Workfront Planning のレコードタイプをExperience Manager Assetsに接続するには、Adobe Experience Manager Assetsライセンスが必要です。組織のWorkfrontインスタンスをAdobeビジネスプラットフォームまたはAdobe Admin Consoleにオンボーディングする必要があります。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Adobe Workfront Planning クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセスレベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースを含め、すべてのワークスペースに対する権限を持ちます。
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but planing is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## レコードタイプの接続に関する考慮事項

* Adobe Workfront Planning では、次のエンティティを接続できます。

   * 2 つのレコードタイプ

     レコードタイプは、同じワークスペースに属している必要があります。
   * 別のアプリケーションのレコードタイプとオブジェクトタイプ。

* 次のオブジェクト・タイプは、Workfront Planning レコード・タイプを使用して、次のアプリケーションから接続できます。

   * ADOBE WORKFRONT:

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * 会社
      * グループ

   * ADOBE EXPERIENCE MANAGER ASSETS:

      * 画像
      * フォルダー

     >[!IMPORTANT]
     >
     >Adobe Experience Manager Assetsライセンスが必要です。Workfront Planning レコードをAdobe Experience Manager Assetsに接続するには、組織のWorkfrontインスタンスをAdobeビジネスプラットフォームまたはAdobe Admin Consoleにオンボーディングする必要があります。
     >
     >Adobe Admin Consoleのオンボーディングについて質問がある場合は、 [AdobeUnified Experience に関する FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* レコードタイプの個々のレコードを作成した後、リンクされたレコードタイプのフィールドから接続先のレコードを選択できます。 詳しくは、 [レコードを接続](../records/connect-records.md).

* レコードタイプを別のレコードタイプに接続するか、別のアプリケーションのオブジェクトタイプに接続すると、次のシナリオが存在します。

   * **2 つのレコードタイプを接続する場合**：接続元のレコードタイプにリンクされたレコードフィールドが作成されます。 接続先のレコードタイプに、類似したリンクされたレコードフィールドが作成されます。

     例えば、「Campaign」レコードタイプを「Product」レコードタイプに接続すると、「Linked Product」という名前のリンクされたレコードフィールドが「Campaign」レコードタイプに作成され、「Campaign」という名前のリンクされたレコードタイプが「Product」レコードタイプに自動的に作成されます。

   * **別のアプリケーションのオブジェクトタイプにレコードタイプを接続する場合**：接続元のレコードタイプにリンクされたレコードフィールドが作成されます。 他のアプリケーションのオブジェクトタイプでは、リンクされたレコードフィールドは自動的に作成されません。

     新しいWorkfront Planning の読み取り専用レコードタイプは、実際のオブジェクトがWorkfront Planning レコードに接続されている場合にのみ、他のアプリケーションのオブジェクトに対して作成されます。

     詳しくは、 [レコードを接続](../records/connect-records.md).

   * **接続先のレコードまたはオブジェクトのルックアップフィールドを追加する場合**：他のアプリケーションのオブジェクトのフィールドをWorkfront Planning レコードタイプに接続できます。 これらは、リンクされたフィールドまたは参照フィールドです。 リンクされたフィールドは、レコードまたはオブジェクトを接続すると、接続されたレコードまたはオブジェクトの情報を自動的に表示します。 リンクされた参照フィールドは常に読み取り専用で、接続されたレコードまたはオブジェクトの値が自動的に設定されます。

     例えば、「Campaign」レコードタイプをWorkfrontプロジェクトに接続し、プロジェクトの「計画完了日」フィールドをWorkfront計画レコードに移行すると、「計画完了日（プロジェクトから） 」と呼ばれるリンクフィールドがキャンペーン用に自動的に作成されます。 このリンクされたフィールドは手動で編集できません。 「計画完了日」（「プロジェクトから」）フィールドには、リンクされたプロジェクトの計画完了日が表示されます。

     >[!IMPORTANT]
     >
     >    ワークスペースに対する表示権限以上の権限を持つユーザーは、リンクされたオブジェクトタイプのアプリケーションでの権限やアクセスレベルに関係なく、リンクされたフィールドの情報を表示できます。

* リンクされたレコードフィールドの前には関係アイコンが付きます ![](assets/relationship-field-icon.png).

  リンクされたフィールドの前には、フィールドタイプを識別するアイコンが付いています。 例えば、フィールドが数値、段落、日付であることを示すアイコンなどです。

## レコードタイプを接続

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを接続するワークスペースを選択します。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. 次をクリック： **+** アイコンをクリックし、 **新しい接続** タブをクリックします。

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. Adobe Analytics の **レコードタイプ** フィールド、レコードタイプを検索するか、次のいずれかを選択します。

   * 選択したワークスペースのセクションの別のレコードタイプ

     >[!TIP]
     >
     >選択したワークスペースのレコードタイプのみが接続できます。
     > 
     >選択したワークスペースに他のレコードタイプがない場合、ワークスペースセクションは表示されません。

   * A **プロジェクト、Portfolio、プログラム、会社**&#x200B;または **グループ化** から **Workfront Object Types** 」セクションに入力します。
   * **Experience Manager Assets** から **Adobeアプリ** 」セクションに入力します。

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. 次の情報を更新します。

   * **名前**：テーブル表示または元のレコードタイプの詳細ページに表示される、接続されたフィールドの名前。 これにより、元のレコードの種類のテーブルビューまたは元のレコードのリンクされたレコードフィールドに、リンクされたレコード列が作成されます。

   >[!TIP]
   >
   >リンク先のレコードの名前を、接続されたレコードフィールドの名前に含めて、新しいフィールドのレコードの種類を取り込むことをお勧めします。 リンクされたレコードの名前は、新しくリンクされたレコードフィールドまたはリンクされたフィールドには表示されません。

   * **説明**:「接続されたレコード」フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **複数のレコードを許可**：リンクされたレコードタイプのフィールドが元のレコードに表示される場合に、ユーザーが複数のレコードを追加できるようにするには、このオプションを選択します。 これはデフォルトで選択されています。
   * **参照フィールドを選択**：選択したレコードタイプからフィールドを追加するには、このオプションを選択します。 ルックアップフィールドは、リンク先のレコードまたはオブジェクトタイプに関連付けられたフィールドです。 リンクすると、目的のレコード上のレコードまたはオブジェクトの情報が表示されます。 これはデフォルトで選択されています。

1. （条件付きおよびオプション）Workfrontオブジェクトの接続を選択した場合、 **カスタムフォーム** から **これらの基準に一致するオブジェクトのみをリンク** 」セクションに入力します。 選択したカスタムフォームが添付されているオブジェクトのみ、選択したレコードタイプにリンクできます。 複数のフォームを選択できます。

   ![](assets/workfront-project-connection-selection.png)

   >[!NOTE]
   >
   > 選択したオブジェクトがこのリストに表示される前に、Workfrontでカスタムフォームを作成する必要があります。

1. （条件付き）Experience Manager Assetsへの接続を選択した場合、 **Experience Managerリポジトリ** ドロップダウンメニュー ( **次のリポジトリーからのアセットのリンク** 」セクションに入力します。 必須フィールドです。このフィールドには、Experience Manager Assetsでアクセス権のあるリポジトリのみが表示されます。

   ![](assets/aem-assets-connection-selection.png)

1. 「**作成**」をクリックします。

1. （条件付き） **参照フィールドを選択** 設定、 **参照フィールドを追加** ボックスが開きます。

   次をクリック： **+** アイコンをクリックして、 **未選択のフィールド** 領域。

   または

   次をクリック： **-** アイコンを使用して、次の場所からフィールドを削除します。 **選択したフィールド** 領域

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   レコードやオブジェクトをリンクした後、接続されたフィールドの値が自動的に入力されます。

   >[!IMPORTANT]
   >
   >    ワークスペースに対する表示権限以上の権限を持つユーザーは、リンクされたオブジェクトタイプのアプリケーションでの権限やアクセスレベルに関係なく、リンクされたフィールドの情報を表示できます。


1. （オプション）「 **スキップ** リンクされたレコードやオブジェクトからフィールドを追加しないでください。 The **名前** リンクされたレコードのフィールドは、元のレコードのテーブルビューに表示される唯一のフィールドです。

1. （オプションおよび条件付き）数値、通貨、割合または日付タイプのフィールドをリンクする場合は、集計値も選択します。 ユーザーがリンクされたレコードフィールドで複数のリンクされたレコードを選択する場合、リンクされたフィールドの値は、コンマで区切るか、選択した集計に従って集計値として表示されます。

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > レコードタイプをExperience Manager Assetsに接続する場合、集約は使用できません。

   次の中から選択します。

   * **なし**：複数のレコードから取得された値をコンマで区切って表示します。 これはデフォルトの選択です。
   * **MAX**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の最大値を表示します。
   * **最小**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の最小値を表示します。
   * **SUM**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の合計を表示します。
   * **AVG**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の平均を表示します。

   >[!NOTE]
   >
   >例えば、キャンペーンレコード（元のレコード）から製品レコード（リンクされたレコード）をリンクし、「製品フィールド」という名前を付けることができます。 また、キャンペーンレコードから製品レコードの「予算」フィールドをリンクし、「製品の予算」と呼ぶこともできます。 「製品」フィールドで複数のレコードを選択できる場合は、予算が$120,000 の製品 1 と、予算が$100,000 の製品 2 を選択できます。 選択した集約に応じて、元のレコードから、リンクされたフィールドに次の予算情報を表示できます。
   >
   >* **なし**:120,000 ドル、100,000 ドル
   >* **MAX**:120,000 ドル
   >* **最小**:100,000 ドル
   >* **SUM**:220,000 ドル
   >* **AVG**:110,000 ドル
   >

1. （オプション） **検索** アイコン ![](assets/search-icon.png) をクリックしてフィールドを検索します。

1. クリック **フィールドを追加** をクリックして変更を保存します。

   次の項目が追加されます。

   * リンク元のレコードタイプ上のリンクされたレコードフィールド。 リンクされたレコードフィールドは、手動で追加した後、リンクされたレコードタイプの個々のレコードを表示します。 レコードの追加について詳しくは、 [レコードを接続](/help/quicksilver/maestro/records/connect-records.md). リンクされたレコードフィールドの名前は、手順 6 で選択した名前です。 <!--accurate-->

   * リンクされたレコードフィールドに手動でレコードまたはオブジェクトを追加した後に、リンクされたレコードまたはオブジェクトタイプのフィールドの情報を表示する、リンクされたフィールド（複数可）。 リンクされたフィールドは、 **参照フィールドを選択** 接続を作成する際に設定が選択されます。 リンクされたフィールドは、次のパターンに従って自動的に名前が付けられます。

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例えば、Campaign のレコードタイプをプログラムのレコードタイプにリンクし、「プログラム情報」フィールドに「プログラム情報」という名前を付けた場合、リンクされたフィールドの名前は自動的に「キャンペーン」のテーブルビューに表示されます `Budget (from Program information)` キャンペーンのテーブル表示。

   * レコードの種類をリンクすると、リンク先のレコードの種類にリンクされたレコードフィールドも追加されます。 リンクされたレコードタイプのリンクされたレコードフィールドの名前は、リンク元のレコードタイプの名前です。

     例えば、「Campaign」レコードタイプから「Product」レコードタイプをリンクし、「Linked Product」キャンペーンの接続済みフィールドに名前を付けた場合、「Campaign」リンク済みレコードタイプに対して「Campaign」リンク済みレコードフィールドが作成されます。

     >[!TIP]
     >
     > 別のアプリケーションのオブジェクトから、Workfront計画でリンク元のレコードタイプにリンクするオブジェクトに対して、リンクされたレコードフィールドは作成されません。

1. （オプションおよび条件付き）元のレコードタイプまたはリンクされたレコードタイプのテーブルビューで、リンクされたレコードフィールドのヘッダーの下向き矢印をクリックし、次のいずれかをクリックします。

   * **フィールドを編集**：更新できるのは **名前** そして **説明** フィールドの情報。
   * **参照フィールドの編集**：リンクされているレコードのフィールドを追加または削除します。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   参照フィールドを追加または削除するには、上記の手順 10～14 の指示に従います。 <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > リンク元のレコードタイプに属する参照フィールドを別のアプリケーションのオブジェクトタイプに追加することはできません。
   >
   > 例えば、キャンペーンからリンク先のWorkfrontプロジェクトに「キャンペーンステータス」のルックアップフィールドを追加することはできません。

1. （オプション）リンク元のレコードタイプから、リンク先のレコードフィールドのヘッダーまたはルックアップフィールドのヘッダーの下向き矢印をクリックし、 **削除**.

   レコードフィールドまたはルックアップフィールドが削除されます。 レコードフィールドを削除すると、リンクされているレコードに関連付けられている参照フィールドも削除されます。
