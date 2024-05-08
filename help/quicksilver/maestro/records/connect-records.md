---
title: レコードを接続
description: レコードタイプ間の接続を作成した後、個別のレコードを相互に接続できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '2356'
ht-degree: 67%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# レコードを接続

{{maestro-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。

まず、2 つのレコードタイプを相互に接続するか、レコードタイプを別のアプリケーションのオブジェクトタイプに接続する必要があります。これにより、リンクされたレコードフィールドが作成されます。その後、リンクされたレコードフィールドを使用して、レコードを相互に接続したり、他のアプリケーションの他のオブジェクトに接続したりできます。

レコードの接続は、レコードを別のアプリケーションのオブジェクトに接続することと似ています。

レコードタイプの相互の接続や、レコードタイプの他のアプリケーションのオブジェクトタイプへの接続について詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

レコードタイプの接続例について詳しくは、[レコードタイプとレコードの接続例](../architecture/example-connect-record-types-and-records.md)を参照してください。

接続できるのは次のとおりです。

* Adobe Workfront計画レコード
* 他のアプリケーションからのオブジェクトを含むAdobe Workfront Planning レコード。

  以下に示すタイプのオブジェクトには、次のアプリケーションからレコードを接続できます。

   * Adobe Workfront

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * 会社
      * グループ

   * Adobe Experience Manager Assets

      * 画像ファイル
      * フォルダー

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
<td>製品</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Adobe Workfront Planning レコードをExperience Manager Assetsに接続するには、Adobe Experience Manager Assets ライセンスが必要で、組織のWorkfront インスタンスがAdobeの Unified Experience にオンボーディングされている必要があります。 詳しくは、を参照してください <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">WorkfrontのAdobe統合エクスペリエンス</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning クローズドベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Workfront Planning には、アクセス レベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>レコードを接続するワークスペースへの権限を管理 </p>  
   <p>他のアプリケーションでのアクセス権に関係なく、他のアプリケーションからのオブジェクトおよびフィールドへのすべての接続を表示するには、ワークスペースに対する表示以上の権限が必要です。 </p>
   <p>システム管理者は、自分が作成したものでないものも含めて、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## レコードを接続

### レコードの接続に関する考慮事項

* レコードタイプを接続すると、接続されたレコードタイプは、リンクされたレコードタイプのテーブルのリンクレコードフィールドとして、およびレコードのページに表示されます。
* リンクされたレコードフィールドから、リンクされたレコードのレコードとオブジェクト、およびオブジェクトタイプを参照して追加できます。
* リンクされたレコードタイプのフィールドを、リンク元のレコードタイプのテーブルに追加できます。
* リンク元のレコードのリンクされたフィールドの値を、手動では更新できません。

  リンクされたレコードのリンクされたフィールドの値は、元のレコードまたはオブジェクトから自動的にリンクしようとしているWorkfront Planning レコードに入力されます。

* ワークスペースに対するWorkfront Planning and View 以上のアクセス権を持つすべてのユーザーは、レコード間またはレコードと他のアプリケーションのオブジェクト間で確立された関連付けを確認できます。 そのようなユーザーは、接続先のアプリケーションの権限に関係なく、接続されたレコードとオブジェクトを表示できます。
* 接続されているレコードが存在するワークスペースに対する管理権限を持っている場合は、他のすべてのユーザーの接続を表示および編集できます。
* 1 つのレコードを別のアプリケーションの 1 つまたは複数のオブジェクトに接続できます。
* レコードを他のレコードまたはオブジェクトとリンクするには、次の条件を満たす必要があります。

   * 少なくとも 1 つのワークスペース、レコードタイプおよびレコード。

     詳しくは、次の記事を参照してください。

      * [ワークスペースを作成](../architecture/create-workspaces.md)
      * [レコードタイプの作成](../architecture/create-record-types.md)
      * [レコードの作成](../records/create-records.md)

   * レコードタイプ間の接続、またはレコードタイプと他のアプリケーションのオブジェクト間の接続。詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

### Adobe Workfrontの計画レコードの接続

{{step1-to-maestro}}

最後にアクセスしたワークスペースが、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードを接続するワークスペースを選択します。
1. レコードタイプのカードをクリックして、レコードタイプページを開きます。
1. レコードタイプページの右上隅にある&#x200B;**ビュー**&#x200B;ドロップダウンメニューから&#x200B;**テーブル**&#x200B;ビューを選択します。
1. （オプション）テーブルに新しい行を追加することにより選択したレコードタイプに、レコードを追加します。詳しくは、[レコードの作成](../../maestro/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプを別のレコードタイプに接続した後、リンクされたレコード列に移動し、他のレコードとリンクするレコードに対応するセルをダブルクリックします。

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 次のいずれかの操作を行います。

   * リストから接続されているレコードの名前をクリックして、選択したレコードに追加します。レコードは自動的に追加されます。
   * レコードの名前の入力を開始し、リストに名前が表示されたら選択します。レコードは自動的に追加されます。
   * 「**すべて表示**」をクリックし、すべてのレコードを表示します。

1. （条件付き）前の手順で「**すべて選択**」をクリックした場合、「**オブジェクトを接続**」ボックスが表示されます。

   ![](assets/connected-objects-table-for-records.png)

1. 検索ボックスにレコードの名前の入力を開始し、リストに名前が表示されたら選択します。

   または

   ボックス内で 1 つまたは複数のレコードの名前を選択し、「オブジェクトを接続」ボックスの右上隅にある「**オブジェクトを接続**」をクリックします。

   >[!TIP]
   >
   >    レコードのページを開き、リンクされたレコードフィールドを見つけて、 **レコードを接続** フィールドで、接続されたレコードまたはオブジェクトタイプからレコードを追加します。
   >
   >![](assets/connect-records-from-record-page-field.png)

   次のものが追加されます。

   * リンクされたレコードは、手順 6 で選択したレコードのリンクされたレコードフィールドに表示されます。<!--accurate?-->
   * レコードタイプを接続したときにリンクされたルックアップフィールドを追加した場合、リンクされたフィールドには、リンクされたレコードからの情報が入力されます。

   リンクされたレコードを更新すると、リンク元のレコードのリンクされたフィールドも自動的に更新されます。リンクされたフィールドは手動で編集できません。

   >[!TIP]
   >
   >* 「リンクされたフィールド」と「ルックアップフィールド」を互換的に使用します。
   >
   >* レコードタイプを接続する際に「**複数のレコードを許可**」設定を有効にした場合、選択した複数のオブジェクトのフィールドの値がカンマで区切られて表示されるか、選択したアグリゲータに従って集計されます。

1. （オプション） レコードタイプ ページを閉じ、選択したワークスペースに移動します。
1. リンク先のレコードタイプのカードをクリックします。

   例えば、**キャンペーン**&#x200B;レコードを製品レコードに接続した場合は、**製品**&#x200B;カードをクリックします。

   レコードタイプカードがテーブルビューで開くはずです。開かない場合は、テーブルビューを選択します。

   **キャンペーン**&#x200B;にリンクされたレコードフィールドには、製品レコードタイプページの製品にリンクしたキャンペーンの名前が表示されることに注意してください。キャンペーン情報を更新すると、製品レコードタイプのキャンペーンにリンクされたレコードフィールドが自動的に更新されます。

### Adobe Workfront Planning レコードのWorkfront オブジェクトへの接続

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

レコードタイプとWorkfront オブジェクトタイプの関連付けを作成したら、個々のレコードをWorkfrontのオブジェクトに関連付けることができます。 接続したWorkfront フィールドは、オブジェクトのリンク元のレコードに自動入力されます。

>[!NOTE]
>
>Workfront オブジェクトをWorkfrontのWorkfront Planning レコードに関連付けることはできません。


{{step1-to-maestro}}

最後にアクセスしたワークスペースが、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードを接続するワークスペースを選択します。
1. レコードタイプのカードをクリックして、レコードタイプページを開きます。
1. **ビュー**&#x200B;ドロップダウンメニューから&#x200B;**テーブル**&#x200B;ビューを選択します。

1. 「**新規レコード**」をクリックして、選択したレコードタイプに個別のレコードを追加します。詳しくは、[レコードの作成](../../maestro/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプを Workfront オブジェクトタイプに接続した後、リンクされたオブジェクト列に移動し、Workfront のオブジェクトにリンクするレコードに対応するセルをダブルクリックします。

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 次のいずれかの操作を行います。

   * リストからオブジェクトをクリックして、選択したレコードに追加します。オブジェクトはアルファベット順にリストされます。オブジェクトは自動的に追加されます。
   * オブジェクトの名前の入力を開始し、リストに名前が表示されたらクリックします。オブジェクトは自動的に追加されます。
   * 「**すべて表示**」をクリックすると、少なくとも表示権限を持つすべてのオブジェクトが表示されます。

1. （条件付き）前の手順で「**すべて表示**」をクリックした場合、「**オブジェクトを接続**」ボックスが表示されます。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 検索ボックスに Workfront オブジェクトの名前の入力を開始し、リストに名前が表示されたら選択します。

   または

   ボックス内の 1 つまたは複数のオブジェクトの名前を選択し、「オブジェクトを接続」ボックスの右上隅にある「**オブジェクトを接続**」をクリックします。

   >[!IMPORTANT]
   >
   >* 表示のアクセス権限のある Workfront オブジェクトのみを追加できます。
   >
   >* Workfront オブジェクトを追加すると、ワークスペースに対する表示権限以上の権限を持つすべてのユーザーは、Workfront での権限やアクセス権に関係なく、Workfront オブジェクトとそのフィールド情報を表示できるようになります。

   次のものが追加されます。

   * 選択した Workfront オブジェクトが、リンクされたレコードフィールドに追加されます。
   * レコードタイプを Workfront に接続するときにこれらを追加した場合、Workfront オブジェクトのリンクされたフィールド（またはルックアップフィールド）には、Workfront からの情報が自動的に入力されます。

   >[!TIP]
   >
   >レコードのページを開き、リンクされたレコードフィールドを見つけて、 **+** アイコンをクリックして、接続されたオブジェクトタイプからオブジェクトを追加します。

   レコードタイプと別のアプリケーションのオブジェクトの接続について詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

1. （オプション）テーブルビューのリンクされたフィールド、またはレコードページのリンクされたフィールドのいずれかから、Workfront Planning レコードに接続されたWorkfront オブジェクトの名前をクリックします。

   これにより、リンクされたWorkfront オブジェクトの読み取り専用Workfront Planning レコードページが開きます。 レコードタイプをWorkfront オブジェクトに接続したときにルックアップフィールドとして選択したフィールドが、Workfront計画レコードページに表示されます。

   >[!TIP]
   >
   >* 「複数のレコードを許可」する設定を有効にすると、ルックアップフィールドの値がカンマで区切られて表示されるか、選択したアグリゲータに従って集計されます。
   >
   >* Workfront のリンクされた Workfront オブジェクトに対して、リンクされたレコードフィールドは作成されません。

1. （オプション）リンクされたWorkfront オブジェクトをWorkfrontで開くには、 **ソースに移動** をWorkfront オブジェクトのレコードページの右上隅に追加します。

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   少なくともオブジェクトを表示する表示権限がある場合は、これにより Workfront オブジェクトページが開きます。編集権限がある場合は、Workfront オブジェクトに関する情報を編集できます。

1. （オプション）レコードタイプのテーブル表示で、リンクされたWorkfront オブジェクトの列見出しにカーソルを置いてドロップダウンメニューをクリックし、「」をクリックします **参照フィールドを編集**.

1. **選択されていないフィールド**&#x200B;エリアから Workfront オブジェクトフィールドを追加します。

   または

   **選択されたフィールド**&#x200B;エリアから、Workfront オブジェクトフィールドを削除します。

   これにより、Workfront Planning レコードにリンクされたフィールドが追加または削除されます。 削除されたフィールドに関連付けられた情報は Workfront に残ります。


### Workfront Planning レコードのAdobe Experience Manager オブジェクトへの接続

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>Workfront Planning レコードをAdobe Experience Manager Assetsに接続するには、Workfrontのライセンスが必要で、組織のAdobe Experience Manager Assets インスタンスがAdobeビジネスプラットフォームまたはAdobe Admin Consoleにオンボーディングされている必要があります。
>
>Adobe Admin Console のオンボーディングについて質問がある場合は、[Adobe Unified Experience の FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md) を参照してください。

レコードタイプとAdobe Experience Manager Assetsの間の関連付けを作成したら、個々のレコードをExperience Managerアセットに関連付けることができます。 接続を作成したときにExperience Manager Assetsから接続したアセットフィールドは、リンク元のレコードタイプに自動入力されます。

{{step1-to-maestro}}

最後にアクセスしたワークスペースが、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードを接続するワークスペースを選択します。
1. レコードタイプのカードをクリックして、レコードタイプページを開きます。
1. レコードタイプページの右上隅にある&#x200B;**ビュー**&#x200B;ドロップダウンメニューから、**テーブル**&#x200B;ビューを選択します。

1. （オプション）「**新規レコード**」をクリックして、選択したレコードタイプに新規レコードを追加します。詳しくは、[レコードの作成](../../maestro/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプを Experience Manager Assets に接続した後、リンクされたオブジェクト列に移動し、Experience Manager の他のオブジェクトとリンクするレコードに対応するセルにポインタを合わせて、**+** アイコンをクリックします。

   >[!TIP]
   >
   >  「」をクリックすると、 **+** アイコンをクリックし、「レコード」ページの「リンクされたオブジェクト」フィールドからアセットをレコードに接続します。

   「**アセットを選択**」ボックスが表示されます。<!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 次のタイプのアセットのいくつかをクリックして選択します。

   * 画像
   * フォルダー

   複数のアセットを選択できます。

   >[!IMPORTANT]
   >
   > Experience Manager で表示するアクセス権のあるアセットのみを接続できます。接続すると、すべてのWorkfront Planning ユーザーは、Experience Manager Assetsでのアクセス権に関係なく、Workfront Planning でアセットを表示できます。

1. 「**選択**」をクリックします。<!-- we might change this to Connect-->

   次のものが追加されます。

   * 選択した Experience Manager Assets が、リンクされたレコードフィールドに追加されます。
   * リンクされたフィールド（またはルックアップフィールド）には、Experience Manager に接続されたアセットからの情報が入力されます。

     Experience Manager Assets のフィールドからのすべての既存の情報は、リンクされたフィールドまたはルックアップフィールドに自動的に表示されます。

     >[!TIP]
     >
     >* 「複数のレコードを許可」する設定を有効にした場合、複数のオブジェクトの値がカンマで区切られて表示されるか、選択したアグリゲータに従って集計されて表示されます。
     >
     >* Experience Manager Assets アプリケーション内のリンクされたExperience Managerアセットに対して、Workfront Planning のリンクされたレコードへのリンクされたレコードフィールドが作成されません。

1. （オプション）Experience Manager Assets にリンクしたレコードタイプに移動し、リンクされたレコードフィールドでアセットの名前をクリックします。アセットの Experience Manager の詳細がポップアップウィンドウに表示されます。<!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   画像ファイルには、次のフィールドが表示されます。

   * 画像のサムネイル
   * 画像ファイル名
   * 寸法
   * サイズ
   * 説明
   * Experience Manager のファイルパス
   * アセットタイプ
   * 作成日
   * 変更日時

1. （オプション）Experience ManagerアセットレコードページをExperience Managerで開くには、リンク元のレコードのレコードタイプページに移動し、「リンクされたレコード」フィールドでアセットの名前をクリックしてポップアップウィンドウを開き、 **開く** アイコン ![](assets/open-asset-icon.png) をクリックしてアセットを開きます。

   これにより、Adobe Experience Manager Assets で Experience Manager のアセットが開きます。

1. （オプション）レコードタイプのテーブル表示で、リンクされたExperience Managerアセットの列見出しにカーソルを置いてドロップダウンメニューをクリックし、「」をクリックします **参照フィールドを編集**.

1. **選択されていないフィールド**&#x200B;エリアから、Experience Manager Assets オブジェクトフィールドを追加します。

   または

   **選択されたフィールド**&#x200B;エリアから、Workfront オブジェクトフィールドを削除します。

   リンクされたフィールドをレコードに追加したり、レコードから削除したりします。 削除されたフィールドに関連付けられた情報は、Adobe Experience Assets に残ります。
