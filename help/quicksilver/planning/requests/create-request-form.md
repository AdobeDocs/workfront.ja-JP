---
title: Adobe Workfront Planning でのリクエストフォームの作成と管理
description: Adobe Workfront計画エリアでレコードタイプを選択した後、リクエストフォームを作成し、そのレコードタイプに関連付けることができます。 その後、リンクを他の社内ユーザーや外部ユーザーと共有できます。 フォームへのリンクを持つユーザーは、フォームにフィールド値を入力でき、フォームを送信すると、フォームに関連付けられたレコードタイプに新しいレコードを追加できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 99e26d4249162e46da1a73301e68bdf30436a81d
workflow-type: tm+mt
source-wordcount: '2678'
ht-degree: 4%

---

# Adobe Workfront Planning でのリクエストフォームの作成と管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

リクエストフォームを作成し、Adobe Workfront Planning でレコードタイプに関連付けることができます。 その後、フォームを他のユーザーと共有し、他のユーザーがそのタイプのレコードを作成するリクエストを送信できます。

この記事では、ワークスペースマネージャーがレコードタイプに関連付けられたリクエストフォームを作成する方法について説明します。

レコードを作成するレコード・タイプにリクエストを発行する方法は、「レコードを作成するためのAdobe Workfront Planning リクエストの発行 [ を参照してください ](/help/quicksilver/planning/requests/submit-requests.md)。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfront パッケージと任意の Planning パッケージ</p>
または
<p>任意のワークフローパッケージと任意の Planning パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースまたはレコードタイプに対する権限の管理 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## リクエストフォームのフィールドと値の表示制限

リクエストを送信した後、リクエストフォームに表示されるフィールドとその値がレコードまたはリクエストの詳細ページに表示される方法には、制限があります。

Workfront Planning 要求の発行の詳細は、[ レコードを作成するためのAdobe Workfront Planning 要求の発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

* リクエストフォーム、リクエストフォームで作成されたレコードまたはリクエストの詳細ページに表示されるフィールドには、以下のような制限があります。

   * リクエストフォームに次のタイプのフィールドを追加することはできません。

      * 作成者、最終変更者、承認者
      * 作成日、最終変更日、承認日
      * Workfront オブジェクトの参照フィールド
      * Workfront Planning 接続レコードの参照フィールド

* リクエストフォームビルダーでのフィールド形式の表示方法と、レコードまたはリクエスト詳細ページでのフィールド値の書式設定方法の違いを次に示します。

   * 通貨、数値、割合の各フィールドは、フォームビルダー内で 1 行のテキストフィールドタイプとして表示されます。

     ただし、フィールドの形式は保持され、リクエストの送信後に、レコードタイプとリクエストの詳細ページに通貨、数値、割合としてフィールド値が表示されます。

* 以下では、リクエストフォームとリクエストの詳細ページに表示されるフィールド値について説明します。

   * 「通貨」、「数値」、「パーセンテージ」の各フィールドの特殊な書式は保持されません。 例えば、これらの領域のこれらのフィールドの値に対して、小数点以下の精度は保持されません。
   * 人物フィールドの値は ID として表示されます。
   * 他のフィールドや計算を参照しない数式フィールドには、値は表示されません。 例えば、`STRING` 式を持つフィールドは「N/A」値を表示します。
   * 通貨フィールドを参照する数式フィールドは、為替レートを考慮せずに値を表示します。
   * 段落フィールドの値は、リクエストフォームに「N/A」値を表示し、リクエストの詳細ページに書式設定されたテキストの代わりに HTML タグを表示します。

## リクエストフォームの作成

リクエストフォームを作成するには、フォームの作成を開始し、フォームの詳細を設定してから、フォームを公開して共有する必要があります。

### リクエストフォームの作成を開始

リクエストフォームは、フォーム <!--span class="preview">, or from the Requests area of Workfront.</span>--> に関連付けられたレコードタイプから作成できます。

#### レコードタイプからのリクエストフォームの作成

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページ ヘッダーのレコードの種類名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、既にフォームがあり、追加のフォームを作成する場合は **リクエストフォームを作成** または **リクエストフォームを管理** をクリックします。
1. （条件付き）別のフォームを追加する場合は、「**新規リクエストフォーム**」をクリックします。

   「リクエストフォームを作成」ボックスが開きます。

1. 「リクエストフォームを作成」ボックスで、リクエストフォームの名前を更新します。 デフォルトでは、フォームの名前は **名称未設定フォーム** です。<!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. （オプション）リクエストフォームに **説明** を追加します。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 「**作成**」をクリックします。

   選択したレコードタイプのリクエストフォームが「フォーム」タブで開きます。
1. [ フォームの設定 ](#configure-the-form) を続行します。

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### 要求フォームの詳細を設定します

フォームの詳細はタブに分かれています。

* 「**フォーム**」タブを使用すると、フィールドとコンテンツ要素をフォームに追加できます
* 「**設定**」タブでは、フォームの承認プロセスを設定したり、リクエスト完了オプションを設定したりできます &lt;。
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### フォームの詳細の設定

1. [ リクエストフォームの作成の開始 ](#begin-creating-a-request-form) の節で説明されているように、リクエストフォームの作成または編集を開始します。

   または

   「リクエストフォーム」リストでリクエストフォームを見つけ、フォーム名の横のボックスをクリックし、画面下部の青いバーにある **フォームを編集** をクリックします。

   選択したレコードタイプのリクエストフォームが「フォーム」タブで開きます。

   ![ キャンペーンリクエストフォーム編集モード ](assets/campaigns-request-form-edit-mode.png)

   リクエストフォームには、デフォルトで次の情報が含まれています。

   * 選択したレコードタイプのテーブル表示で使用可能なレコードフィールド。<!--they are working on removing the limitation below-->

   * **デフォルトセクション**：これは、Workfrontがリクエストフォームに適用するデフォルトのセクション区切りです。 すべてのレコードフィールドが **デフォルトセクション** 領域に表示されます。
   * **件名** フィールド：Workfrontでリクエストを識別するフィールド。 「件名」フィールドの設定と値は編集できません。

     >[!NOTE]
     >
     >* **件名** フィールドは、リクエストフォームに表示される場合、値が必要です。 ただし、必要に応じて「**件名** フィールドを削除することができ、リクエスターがリクエストを送信してもフォームに表示されません。
     >* リクエストフォームに「件名」フィールドがなく、将来のレコードの名前に対する「名前」フィールドがある場合、リクエストの名前は、作成されたレコードと同じ名前に自動的に割り当てられます。
     >* リクエストフォームに「件名」フィールドと「名前」フィールドの両方がない場合、リクエストは、`< Record name > request form < Entry date of the request >` のパターンを使用して名前が付けられます。レコードの名前は **名称未設定** です。

   * レコードタイプに関連付けられているすべてのフィールド。

     リクエストフォームに含まれるフィールドは、このレコードタイプにリクエストを送信するすべてのユーザーに表示されます。

1. （オプション）削除するフォーム上のフィールドの上にマウスポインターを置き、「**x**」アイコンをクリックして削除します。 これらは、フォームの左側にある **フィールド** タブに追加されます。

1. （オプション）フォームから **デフォルトセクション** を削除するには、次の手順を実行します。

   1. デフォルトセクションからすべてのフィールドを削除します。
   1. **コンテンツ要素** をクリックし、新しいセクションを追加して、セクションの名前を追加します。
   1. 新しいセクションにフィールドを追加します。
   1. **x** アイコンをクリックして **デフォルトのセクション** を削除します。
1. 任意のフィールドをクリックし、フォームの右側のパネルにあるコントロールを使用して、フィールドのサイズまたは次の情報を定義します。

   * **ラベル**：リクエストフォームに表示されるフィールドの名前です。 レコードフィールドの名前は変更されません。
   * **手順**：フィールドに関する詳細情報を追加します。
   * **必須フィールドにする**：選択する場合、フィールドには値が必要です。 追加されていない場合、フォームを送信できません。
   * **ロジックの追加**：フィールドを表示または非表示にするには、どの条件を満たす必要があるかを定義します。

   >[!TIP]
   >
   >   フォームでフィールドを選択すると、各フィールドのフィールドタイプが右側のパネルの上部に表示されます。
   >     

1. （オプション）フォームの左側にある「**コンテンツ要素**」タブをクリックして、次の要素のいずれかを追加します。

   * **説明テキスト**
   * **セクション区切り**

   カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

1. （オプション） **プレビュー** をクリックして、他のユーザーが新しいレコードを送信する際にフォームを使用する際のフォームの表示方法を表示します。
1. フォームの詳細を設定する場合は、[ 設定の詳細を設定 ](#set-up-configuration-details) を続行するか、「[ リクエストフォームの作成を完了 ](#complete-request-form-creation)」に移動します。

#### 設定の詳細

「設定」タブでは、承認プロセスを設定し、このフォームから作成されたリクエストが完了としてマークされるタイミングを設定できます。

1. [ リクエストフォームの作成の開始 ](#begin-creating-a-request-form) の節で説明されているように、リクエストフォームの作成または編集を開始します。

   選択したレコードタイプのリクエストフォームが「フォーム」タブで開きます。
1. （オプション） [ フォーム詳細の設定 ](#set-up-form-details) の説明に従って、フォーム詳細を設定します。

1. （オプション）承認者を追加する場合は、「**設定**」タブをクリックし、「**承認者** フィールドに少なくとも 1 人のユーザーまたはチームを追加して、このレコードフォームの新しいリクエストを承認します。

   ![ 「設定」タブ ](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * リクエストフォームには、1 人または複数の承認者を追加できます。
   * 少なくとも 1 人の承認者が要求を拒否した場合、要求は拒否され、レコードは作成されません。 リクエストは、Workfrontの「リクエスト」領域にある「送信済み」セクションの「計画」タブに残ります。
   * 複数の承認者を追加し、「必要な決定が 1 つのみ」オプションが有効になっていない場合、リクエストが承認または却下される前に、すべての承認者が決定を行う必要があります。
   * チームが承認者として設定されている場合、チームからの決定は 1 つだけ必要です。

   リクエストフォームへの承認の追加について詳しくは、「[ リクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md)」を参照してください。

1. （条件付き）承認者の 1 人が承認した後にレコードを作成する場合は、「**決定は 1 つだけ必要**」チェックボックスをオンにします。

1. このフォームから作成された要求を、要求されたオブジェクトの作成時に完了とマークするか、または要求されたオブジェクトの完了時にマークするかを選択します。
1. （条件付き）リクエストされたオブジェクトが完了したときにリクエストが完了とマークされるようにを選択した場合は、オブジェクトが完了したときに示されるフィールドと値を選択します。 例えば、作成されたオブジェクトのステータスが「完了」に設定されている場合に、「ステータス」フィールドと値「完了」を選択してリクエストを完了できます。
1. <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[ リクエストフォームの作成を完了 ](#complete-request-form-creation) に進みます。

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### 完全なリクエストフォームの作成

1. [ リクエストフォームの作成の開始 ](#begin-creating-a-request-form) および [ リクエストフォームの詳細の設定 ](#set-up-details-for-the-request-form) の説明に従って、フォームを作成および設定します。
1. （オプション）ヘッダーのフォーム名の右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、「**編集**」をクリックしてフォーム名を更新します。

1. 「**公開**」をクリックしてフォームを公開し、フォームの一意のリンクを取得します。

   次のことが発生します。

   * **公開** ボタンは削除されました。
   * **非公開** ボタンがフォームに追加されます。 クリックすると、フォームにアクセスできなくなります。
   * 「**共有** ボタンがフォームに追加されます。
   * フォームは、Workfrontのメインメニューの「リクエスト」領域で使用できるようになります。

1. **共有** をクリックして、フォームを他のユーザーと共有します。

   リクエストフォームの共有について詳しくは、この記事の [ リクエストフォームの共有 ](#share-a-request-form) の節を参照してください
1. ヘッダーでフォーム名の左側にある左向き矢印をクリックして、フォームを閉じます。

   **リクエストフォーム** テーブル表示が開き、フォームが追加されます。

## 既存の要求フォームの管理


1. リクエストフォームを管理するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、**リクエストフォームの管理** をクリックします。

   レコードタイプに関連付けられたすべてのリクエストフォームがテーブル表示に表示されます。

1. （オプション）テーブル表示でリクエストフォームの名前の上にマウスポインターを置き、フォーム名の右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックして、次のいずれかをクリックします。

   * **フォームを編集**：フォームの情報をさらに編集するには、これをクリックします。
   * **非公開**：このボタンをクリックしてフォームを非公開にすると、Workfrontのリクエスト領域から削除されます。
   * **共有**: フォームへのアクセス権を持つユーザーを変更するには、これをクリックします。
   * **リンクをコピー**：フォームを開かずにリクエストフォームのリンクをすばやくコピーする場合は、これをクリックします。
   * **削除**：フォームを削除するには、これをクリックします。 フォームを使用して追加されたリクエストとレコードはすべて削除されません。 フォームを復元できません。

   ![ リクエストフォームリストからのリクエストフォームの「詳細」メニュー ](assets/more-menu-on-request-form-from-request-forms-list.png)

1. ヘッダーにある **リクエストフォーム** の左側の左向き矢印をクリックして、リクエストフォームテーブルを閉じます。

   レコードタイプのページが開きます。
1. （オプションおよび条件付き）ヘッダーのレコードタイプ名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、次のいずれかの操作を行います。

   1. 「**リクエストフォームを更新**」をクリックしてリクエストフォームに変更を加え、リクエストフォームをクリックして開いて編集します。
   1. **リクエストフォームにリンクをコピー** をクリックして、フォームへのリンクを他のユーザーと共有します。

1. （オプション）Workfrontの **リクエスト** エリアに移動して、リクエストを送信する共有フォームを見つけます。 詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。

## リクエストフォームの共有

1. この記事の [ レコードタイプのリクエストフォームを作成する ](#create-a-request-form-for-a-record-type) の節の説明に従ってリクエストフォームを作成します。
1. レコードタイプのページでリクエストフォームの名前の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックします。
1. **共有** をクリックして、フォームを他のユーザーと共有します。

1. フォームを内部的に共有するには、「**内部共有**」タブを選択し、「**このフォームを送信するためのアクセス権を付与**」フィールドでユーザー、チーム、担当業務、グループまたは会社の名前を検索して、リストに表示されたら選択します。 **送信** 権限は、各エンティティに対してデフォルトで選択されています。

   ![ リクエストフォームの共有ボックス ](assets/share-box-for-request-form.png)

1. （オプション）エンティティ名の後のドロップダウンメニューをクリックして「**削除**」をクリックすると、リストから削除されてフォームの共有が停止されます。

   >[!NOTE]
   >
   >チーム、グループ、会社、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。 Workfrontのみのユーザーを追加することはできません。 詳しくは、[Adobe Admin Consoleでのユーザーの管理 ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。

1. 「**このフォームを通じてリクエストを送信できるユーザー**」セクションで、このフォームにアクセスできるユーザーのタイプを次のオプションから選択します。

   * 招待されたユーザーのみがアクセス可能
   * ワークスペースに対する表示またはそれ以上のアクセス権を持つすべてのユーザー
   * ワークスペースに対する参加またはそれ以上のアクセス権を持つすべてのユーザー
1. （オプション）「**リンクをコピー**」をクリックして、アクセス権を持つユーザーとフォームへのリンクを共有します。 リンクがクリップボードにコピーされます。
1. フォームを公開で共有するには、「**公開共有**」タブを選択し、「**公開リンクを作成** 設定を有効にします。

   ![ 請求書類の公開 ](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* **公開リンクを作成** 設定を有効にすると、組織外のユーザーであっても、誰でもフォームにアクセスして、新しいレコードを送信できます。Workfront アカウントがない場合も同様です。
   >
   >* 次のフィールドタイプを含むフォームは、パブリックに共有できません。
   >
   >     * WorkfrontまたはAEM Assetsの接続
   >     * ユーザー
   >

1. **リンクの有効期限** を選択します。

   現在の日付から 180 日以内の将来の日付を選択できます。

   >[!TIP]
   >
   >共有日が終了すると、Workfrontの「リクエスト」領域でリクエストフォームが使用できなくなり、他のユーザーと共有されていたリンクにもアクセスできなくなります。

   リンクの有効期限が切れた後、ユーザーはエラーを受け取ります。ユーザーがフォームに再度アクセスできるようにするには、リンクの日付を更新し、新しいリンクを生成して共有する必要があります。


1. （オプションおよび条件付き） **保存** をクリックして、フォームの共有の詳細を保存します。
1. （条件付き）フォームが以前に保存されている場合は、「**リンクをコピー**」をクリックします。

   フォーム共有オプションが保存され、リンクがクリップボードにコピーされます。 他のユーザーと共有できるようになりました。

   リクエストフォームへのリンクを使用してレコードを作成する方法については、「[Adobe Workfront Planning リクエストの送信 ](/help/quicksilver/planning/requests/submit-requests.md)」を参照してください。

1. **フォーム** タブの右下隅にある「**保存**」をクリックしてフォームを保存します。
