---
title: Adobe Workfront Planning でのリクエストフォームの作成と管理
description: Adobe Workfront計画エリアでレコードタイプを選択した後、リクエストフォームを作成し、そのレコードタイプに関連付けることができます。 その後、リンクを他の社内ユーザーや外部ユーザーと共有できます。 フォームへのリンクを持つユーザーは、フォームにフィールド値を入力でき、フォームを送信すると、フォームに関連付けられたレコードタイプに新しいレコードを追加できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 12%

---

# Adobe Workfront Planning でのリクエストフォームの作成と管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

リクエストフォームを作成し、Adobe Workfront Planning でレコードタイプに関連付けることができます。 その後、リンクを他の社内ユーザーや外部ユーザーと共有できます。

フォームへのリンクを持つユーザーは、そのフォームにフィールド値を更新し、フォームを送信して新しいレコードを追加できます。

この記事では、ワークスペースマネージャーがレコードタイプに関連付けられたリクエストフォームを作成する方法について説明します。

レコードを作成するレコード・タイプにリクエストを発行する方法は、「レコードを作成するためのAdobe Workfront Planning リクエストの発行 [ を参照してください ](/help/quicksilver/planning/requests/submit-requests.md)。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfrontの計画<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
<p>次のいずれかのWorkfront プラン：</p>
<ul><li>選択</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td>
   <td>
<p>任意 </p>  
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <ul>
   <li><p>ワークスペースに対する権限の管理</p></li>
    <li><p>システム管理者は、自分が作成していないワークスペースを管理できます。 </p></li>
    </ul>
   <p>Workfront Planning オブジェクトの共有権限について詳しくは、
<a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a>を参照してください。 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードタイプ用のリクエストフォームの作成

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側 ![](assets/more-menu.png) ある **詳細** メニューをクリックし、「**リクエストフォームを作成**」をクリックします。
1. リクエストフォームの名前を更新します。 デフォルトでは、フォームの名前は **名称未設定フォーム** です。<!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. （オプション）リクエストフォームに **説明** を追加します。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 「**作成**」をクリックします。選択したレコードタイプのリクエストフォームが「フォーム」タブで開きます。

   ![](assets/campaigns-request-form-edit-mode.png)

   リクエストフォームには、デフォルトで次の情報が含まれています。

   * 選択したレコードタイプのテーブル表示で使用可能なレコードフィールド。<!--they are working on removing the limitation below-->

   <!-- when we go to prod, the Preview batch below will become the only batch-->

   >[!IMPORTANT]
   >
   >次のタイプのフィールドは、リクエストフォームに表示されません。
   >
   >* 作成者と最終変更者
   >* 作成日と最終変更日
   >* 式
   >* Workfront オブジェクトの参照フィールド
   >* Workfront Planning 接続レコードの参照フィールド
   >

   <!--before release to prod: 
    > Depending on what environment you use to create a request form, the following scenarios exist:
   >
   >* Fields of the following types do not display in the request form in the Production environment: 
   >
   >    * Created by and Last modified by
   >    * Created date and Last modified date
   >    * Formula
   >    * People 
   >    * Workfront connected fields
   >    * Workfront objects' lookup fields
   >    * Workfront Planning records' connected fields
   >    * Workfront Planning connected records' lookup fields
   >    * AEM Assets connection fields-->

   * **デフォルトセクション**：これは、Workfrontがリクエストフォームに適用するデフォルトのセクション区切りです。 既定のセクションの名前を変更したり、削除することはできません。
   * **件名** フィールド：Workfrontでリクエストを識別するフィールド。 「件名」フィールドの設定と値は編集できません。

     >[!TIP]
     >
     >**件名** フィールドは、リクエストフォームに表示される場合、値が必要です。 ただし、必要に応じて「**件名** フィールドを削除することができ、リクエスターがリクエストを送信してもフォームに表示されません。

   * レコードタイプに関連付けられているすべてのフィールド。

     リクエストフォームに含まれるフィールドは、このレコードタイプにリクエストを送信するすべてのユーザーに表示されます。

1. （オプション）削除するフォーム上のフィールドの上にマウスポインターを置き、「**x**」アイコンをクリックして削除します。 これらは、フォームの左側にある **フィールド** タブに追加されます。

   例えば、「**件名** フィールドはWorkfront Planning には表示されないので、これを削除します。<!--remove this step when we connect intake with the Requests area in Workfront-->
1. 任意のフィールドをクリックし、フォームの右側のパネルにあるコントロールを使用して、フィールドのサイズまたは次の情報を定義します。

   * **ラベル**：リクエストフォームに表示されるフィールドの名前です。 レコードフィールドの名前は変更されません。
   * **手順**：フィールドに関する詳細情報を追加します。
   * **必須フィールドにする**：選択する場合、フィールドには値が必要です。 追加されていない場合、フォームを送信できません。
   * **ロジックの追加**：フィールドを表示または非表示にするには、どの条件を満たす必要があるかを定義します。

   >[!NOTE]
   >
   >   フォームでフィールドを選択すると、各フィールドのフィールドタイプが右側のパネルの上部に表示されます。
   >   
   >
   >   「通貨」、「数値」、「パーセント」の各フィールドは、1 行のテキスト・フィールド・タイプとして表示されます。 ただし、フィールドの形式は保持され、これらのフィールド内の値は、通貨、数値、パーセント値として表示されます。

1. （オプション）フォームの左側にある「**コンテンツ要素**」タブをクリックして、次の要素のいずれかを追加します。

   * **説明テキスト**
   * **セクション区切り**

   カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

1. （オプション） **プレビュー** をクリックして、他のユーザーが新しいレコードを送信する際にフォームを使用する際のフォームの表示方法を表示します。

1. （オプション）「**設定**」タブをクリックし、「**承認者**」フィールドに少なくとも 1 人のユーザーを追加して、このレコードフォームの新しいリクエストを承認します。

   ![](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * リクエストフォームを承認者に関連付ける場合、新しいリクエストは、新しいレコードを生成する前に、最初にすべての承認者の承認を受ける必要があります。
   * リクエストフォームには、1 人または複数の承認者を追加できます。
   * 少なくとも 1 人の承認者が要求を拒否した場合、要求は拒否され、レコードは作成されません。
   * すべての承認者は、リクエストが承認または却下される前に決定を行う必要があります。

     リクエストフォームへの承認の追加について詳しくは、「[ リクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md)」を参照してください。

1. （オプション）ヘッダーのフォーム名の右 ![](assets/more-menu.png) にある **詳細** メニューをクリックしてから、**編集** をクリックしてフォームの名前を更新します。
1. **Publish** をクリックしてフォームを公開し、フォームの一意のリンクを取得します。

   次のことが発生します。

   * 「**Publish**」ボタンが削除されました。
   * **非公開** ボタンがフォームに追加されます。 クリックすると、フォームにアクセスできなくなります。
   * 「**共有** ボタンがフォームに追加されます。

1. **共有** をクリックして、フォームを他のユーザーと共有します。

   ![](assets/share-box-for-request-form.png)

1. このフォームにアクセスできるユーザーのタイプを指定するには、次のオプションから選択します。

   * ワークスペースへの表示またはそれ以上のアクセス権を持つすべてのユーザー
   * ワークスペースへの参加またはそれ以上のアクセス権を持つすべてのユーザー
   * リンクを知っているすべてのユーザー

   >[!WARNING]
   >
   >* **リンクを持つすべてのユーザー** を選択すると、組織外のユーザーであっても、Workfront アカウントを持たないユーザーであっても、誰でもフォームにアクセスして、新しいレコードを送信できます。
   >
   > * 次のフィールドタイプを含むフォームは、パブリックに共有できません。
   >
   >     * WorkfrontまたはAEM Assetsの接続
   >     * ユーザー
   >

1. （条件付き）前の手順で「**リンクを持つすべてのユーザー**」を選択した場合は、使用可能なカレンダーから **有効期限をリンク** を選択します。 リンクの有効期限が切れた後、ユーザーはエラーを受け取ります。ユーザーがフォームに再度アクセスできるようにするには、リンクの日付を更新し、新しいリンクを生成して共有する必要があります。

   現在の日付から 180 日以内の将来の日付を選択できます。

1. **リンクを保存してコピー** をクリックして、フォームの共有の詳細を保存します。 フォームが以前に保存されている場合は、「**リンクをコピー**」をクリックします。

   フォーム共有オプションが保存され、リンクがクリップボードにコピーされます。 他のユーザーと共有できるようになりました。

   リクエストフォームへのリンクを使用してレコードを作成する方法については、「[Adobe Workfront Planning リクエストの送信 ](/help/quicksilver/planning/requests/submit-requests.md)」を参照してください。

1. **フォーム** タブの右下隅にある「**保存**」をクリックしてフォームを保存します。
1. ヘッダーでフォーム名の左側にある左向き矢印をクリックして、フォームを閉じます。

   レコードタイプのページが開きます。
1. （オプション）ヘッダーのレコードタイプ名の右側に ![](assets/more-menu.png) る **詳細** メニューをクリックして、次のいずれかの操作を行います。
   * 「**リクエストフォームを更新**」をクリックして、リクエストフォームに変更を加えます。
   * **リクエストフォームにリンクをコピー** をクリックして、フォームへのリンクを他のユーザーと共有します。

   >[!TIP]
   >
   >その場合には、リンクが公開されている表示があります。
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
