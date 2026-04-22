---
title: Adobe Workfront計画リクエストの送信
description: Adobe Workfront Planningのレコードタイプページから誰かがリクエストフォームへのリンクを共有した後、リクエストを追加して、リクエストフォームに関連付けられたレコードタイプのレコードを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 3%

---

# Adobe Workfront Planning リクエストを送信して、レコードを作成

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Workspace ManagerがAdobe Workfront Planningでレコードタイプのリクエストフォームを作成した後、そのフォームを使用して、そのフォームに関連付けられたレコードタイプのレコードを作成するリクエストを送信できます。

次の領域からWorkfront Planning リクエストを送信できます。

* Workfrontのリクエストエリアまたはホームのマイリクエストウィジェットから。
* 共有されたリクエストフォームへの直接リンクから。
* レコードタイプページから、リクエストを送信して新しいレコードを追加する場合。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

この記事では、Workfrontのリクエスト領域または共有リンクから、レコードタイプに新しいレコードを追加するリクエストを送信する方法について説明します。

Workspace管理者は、リクエストフォームを作成できます。このフォームをユーザーまたは外部ユーザーとして使用して、Planning レコードタイプにリクエストを送信できます。 リクエストは、リクエストフォームに関連付けられたレコードタイプのレコードを作成します。

Workspace Managerがリクエストフォームを作成し、レコードタイプに関連付ける方法について詳しくは、[Adobe Workfront Planningでのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)を参照してください。

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
<p>任意のWorkfrontまたはWorkflow パッケージ</p>
<p>任意のWorkfront計画パッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。</p>
   </td> </tr>
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>Workfront ユーザーの場合は、ワークスペースおよびレコードタイプに対する表示以上の権限</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## 前提条件

Workfront Planning リクエストフォームにリクエストを送信するには、次の手順を実行する必要があります。

* Workfront Planningには、次の情報が必要です。

   * ワークスペース
   * レコードタイプ
   * レコードタイプに関連付けられたリクエストフォーム。

     詳しくは、[Adobe Workfront Planningでのリクエストフォームの作成](/help/quicksilver/planning/requests/create-request-form.md)を参照してください。

* リクエストフォームは、アクセスできる方法で共有する必要があります。 次のシナリオが存在します。

   * 内部的には、ワークスペースに対する表示権限またはそれ以上の権限を持つユーザーとフォームを共有する必要があります。

     Workfront ユーザーは、リンクからフォームにアクセスするか、Workfrontのリクエスト領域でリクエストフォームを見つけることができます。

   * 外部では、Workfront アカウントを持たない外部のユーザーとレコードフォームへのリンクを共有します。

     Workfront ユーザーは、外部のユーザーと共有されたリンクにアクセスすることもできます。

* リンクで共有する場合、フォームへのリンクは期限切れにしないでください。

## Workfront Planningへのリクエストの送信に関する考慮事項

* Workfrontでリクエストを送信した後は、リクエストを編集することはできません。
* 送信された各要求は、使用するフォームに関連付けられたレコードタイプ、フォームが承認に関連付けられていない場合、またはすべての承認者によって承認が付与された場合のレコードを作成します。
* リクエストフォームの送信によって作成されたレコードは、Workfront Planningの他のメソッドで追加されたレコードと同じです。

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* リクエストフォームの送信によって作成されたレコードは、元のリクエストに接続されます。 この接続は削除できません。
* 作成されたレコードと、作成に使用されたリクエストの両方を次の領域で表示できます。
   * Workfrontのリクエスト領域。
   * リクエストを接続されたレコードとして追加すると、Workfront Planningのレコードタイプページの接続フィールドに。
   * リクエストを接続されたレコードとして追加すると、Workfront Planningのレコードの「詳細」領域の接続フィールドに。

  >[!TIP]
  >
  >リクエストの名前は、Workfrontの「リクエスト」エリアの「件名」フィールドまたはWorkfront Planningの「元のリクエスト接続」フィールドで確認できます。

* 送信された計画リクエストは、新しいリクエストエクスペリエンスでのみ表示されます。 従来のリクエストエクスペリエンスでは、プランニングリクエストを表示できません。

  詳しくは、[&#x200B; リクエストの作成と送信](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)を参照してください。
* 特定のフィールドタイプをリクエストフォームに表示する方法や、フォームの送信後にリクエストの詳細ページを表示する方法には制限があります。

  詳しくは、[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)でのリクエストフォームの作成と管理を参照してください。

<!--
Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.
-->


## Workfrontのリクエスト領域で、Workfront Planningにリクエストを送信します

{{step1-to-requests}}

1. 画面の右上隅にある「**新しいエクスペリエンスを使用**」設定をオンにします。
この設定をオンにすると、Workfront Planning リクエストフォームがWorkfrontの&#x200B;**リクエスト**&#x200B;領域で使用できるようになります。

   >[!TIP]
   >
   >この設定は、Workfront インスタンスがAdobe Unified Experienceにオンボーディングされている場合にのみ使用できます。
   >
   >この領域でWorkfront計画リクエストを送信するには、次の条件を満たす必要があります。
   >
   >* お客様の会社がWorkfront プランニングライセンスを購入しました。
   >
   >* 少なくとも1つのワークスペースを表示するアクセス権があります。

1. **どのリクエストを送信しますか？リクエストフォームのリストを開くための** バー。
1. リストからリクエストフォームを選択するか、リクエストフォーム名の入力を開始してから、リストに表示されたらリクエストフォームを選択します。

   ウィンドウが開き、上部にリクエストフォーム名が表示されます。

   >[!TIP]
   >
   >Workfront リクエストキューには、リクエストのリストに含まれるキューの名前とフォームの名前が含まれます。 プランニングリクエストフォームは、リクエストのリストにフォーム名のみを表示します。

1. **件名** フィールドを更新します。 これはリクエスト名です。 必須フィールドです。
1. **名前** フィールドを更新します。 これは将来のレコードの名前です。

   >[!TIP]
   >
   >**名前** フィールドは組織に固有であり、Workfront インスタンスに別のラベルが表示される場合があります。 フィールドはレコードのプライマリフィールドです。

1. リクエストフォームの残りのフィールドを更新します。 赤いアスタリスクのフィールドは必須です。
1. （条件付き）組織がAIによる&#x200B;**フォーム入力**&#x200B;を許可している場合、プロンプトとしてドキュメントをアップロードできます。 AIはこれらのドキュメントを使用してフォームに入力します。リクエストを送信する前に、AIの提案を承認または却下できます。


   手順については、[AIを活用したフォーム入力を使用して、プロンプトまたはドキュメントを使用してリクエストを入力する](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)を参照してください。
1. 「**送信**」をクリックします。

   リクエストフォームが閉じ、**リクエスト**&#x200B;領域に戻ります。

   フォームが送信され、次のことが発生します。

   * リクエストフォームが承認に関連付けられていない場合、リクエストはWorkfront リクエスト領域のリクエストリストとホームのマイリクエストウィジェットに追加され、フォームに関連付けられたレコードタイプに新しいレコードが追加されます。

     次のフィールドは、「リクエスト」エリアにリクエスト情報とレコード情報を表示し、「ホーム」にマイリクエストウィジェットを表示します。

      * **件名**: リクエスト領域に追加された元のリクエストの名前。 リクエストリストから&#x200B;**件名** フィールドを非表示または削除することはできません。 名前には、Planningでリクエストページを開くリンクがあります。
      * **作成済みオブジェクト**:Planningに表示されるリクエストから作成されたレコードの名前。 作成済みオブジェクト名には、リクエストから作成したレコードを開くリンクがあります。
      * **オブジェクトタイプ**:Planningのリクエストからレコードが作成されたワークスペースとレコードタイプの名前。
      * **ステータス**: リクエストオブジェクトのステータス。
      * **リクエストフォーム**:Planningのレコードタイプに関連付けられたリクエストフォームの名前。
      * **作成済みオブジェクトの状態**：作成されたレコードの状態。

   * リクエストフォームが承認に関連付けられている場合、リクエストはWorkfront リクエスト領域のリクエストリストに追加され、ステータスは&#x200B;**レビュー待ち**&#x200B;です。 新しいレコードは、承認者が承認した後にのみレコードタイプページに追加されます。

     詳しくは、[&#x200B; リクエストフォームへの承認の追加](/help/quicksilver/planning/requests/add-approval-to-request-form.md)を参照してください。

   * レコードを作成した元のリクエストの名前を表示するには、Planningのレコードタイプに「**元のリクエスト**」接続フィールドを追加できます。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   * リクエストは、所有者、承認者、および少なくともワークスペースに対する表示権限を持つユーザーにのみ表示されます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。
   * リクエストが正常に送信されたか、レビュー用に送信されたことを示すアプリ内およびメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者はアプリ内メッセージと、リクエストをレビューして承認するためのメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experienceにオンボーディングされている場合にのみ表示されます。
     >
     >メールの確認または承認通知に、リクエストへのリンクがあります。

1. （オプション）確認メッセージで「**リクエストを表示**」をクリックしてリクエストを開くか、**X** アイコンをクリックして確認を閉じます。
1. （オプション）情報がリクエストリストに表示される方法を管理するには、リストの次のビュー要素を更新します。

   * 表示
   * フィルター
   * 列
   * グループ化
   * セルを書式設定
   * 行の高さ

   詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。

   <!-- 
   Removing this as this is covered at a higher level in the Use enhanced lists article: 
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. リスト内のリクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![&#x200B; コメント付きのリクエストページ &#x200B;](assets/new-request-page-with-comment.png)

1. （オプション）「**コメント**」領域にコメントを入力します。
1. （条件付き）要求フォームが承認に関連付けられていない場合、または要求が承認されている場合は、要求の名前をクリックし、**作成済みオブジェクト** フィールドのレコード名をクリックします。

   レコードのページがWorkfront Planningで開きます。

   >[!TIP]
   >
   >* レコードのプライマリフィールドがリクエストフォームで更新されていない場合、リクエストの「レコード」フィールドのレコードの名前は&#x200B;**名称未設定**&#x200B;と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合は、リクエストページからレコードにアクセスする前に、承認を付与する必要があります。 レコードは、承認が付与されるまで作成されません。

1. （オプション） **レコードタイプ**&#x200B;の名前をクリックします。

   Workfront Planningでレコードタイプページが開きます。

## 共有リンクからリクエストフォームにリクエストをWorkfront Planningに送信する

このセクションの情報は、共有リンクからリクエストを送信し、Workfront アカウントを持っていない可能性があるユーザーにのみ適用されます。

**リクエスト**&#x200B;や&#x200B;**ホーム**&#x200B;など、Workfrontの内部領域に外部ユーザーがアクセスできません。

1. Workfront Planningのレコードタイプから共有されたリンクに移動します。

1. フォームで使用可能なフィールドを更新します。 アスタリスク付きのフィールドは必須です。

   >[!TIP]
   >
   >   **件名** フィールドが使用可能な場合、リクエストの送信後、Workfront Planningに表示されません。
   >
   >Workfront Planningのレコードタイプに新しいレコードを追加する際に、新しいレコードを識別可能にするために、リクエスト内のフィールドをできるだけ更新することをお勧めします。

1. 「**送信**」をクリックします。

   フォームが送信され、確認メールが届きます。

   フォームが承認に関連付けられている場合は、レコードを作成する前に承認する必要があります。

1. （オプション）「**別のリクエストを送信**」をクリックして、同じ共有リンクを使用して別のリクエストを追加します。

   * リクエストフォームが承認に関連付けられていない場合、リクエストはWorkfront リクエスト領域のリクエストリストとホームのマイリクエストウィジェットに追加され、フォームに関連付けられたレコードタイプに新しいレコードが追加されます。 これは、Workfrontにログインしている場合にのみ使用できます。

   * リクエストフォームが承認に関連付けられている場合、リクエストはWorkfront リクエスト領域のリクエストリストに追加され、マイリクエストウィジェットのステータスは「レビュー待ち」になります。 すべての承認者がレコードを承認した後にのみ、新しいレコードがレコードタイプページに追加されます。 これは、Workfrontにログインしている場合にのみ使用できます。

     詳しくは、[&#x200B; リクエストフォームへの承認の追加](/help/quicksilver/planning/requests/add-approval-to-request-form.md)を参照してください。

     >[!IMPORTANT]
     >
     >少なくとも表示権限を持つワークスペースに対して、自分または他のユーザーが送信したリクエストのみを表示できます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。

   * リクエストが正常に送信されたか、レビュー用に送信されたことを示すアプリ内およびメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者はアプリ内メッセージと、リクエストをレビューして承認するためのメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experienceにオンボーディングされている場合にのみ表示されます。

     リクエストが承認され、レコードが作成された後、「承認者」および「承認日」フィールドには、レコードに対する承認に関する情報が表示されます。

1. （オプション）「**リクエストを表示**」をクリックして、Workfrontでリクエストを開きます。

または

「[別のリクエストを送信](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request)」をクリックしてリクエストフォームを開き、新しいリクエストを追加します。

リクエストの詳細ページが開きます。

![&#x200B; コメント付きのリクエストページ &#x200B;](assets/new-request-page-with-comment.png)

1. （オプション）「**コメント**」領域にコメントを入力します。
1. （条件付き）要求フォームが承認に関連付けられていない場合、または要求が承認されている場合は、要求の名前をクリックし、**作成済みオブジェクト** フィールドのレコード名をクリックします。

   レコードのページがWorkfront Planningで開きます。

   >[!TIP]
   >
   >* レコード名がリクエストフォームに追加されていない場合、リクエストの「レコード」フィールドのレコード名は&#x200B;**名称未設定**&#x200B;と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合は、リクエストページからレコードにアクセスする前に、承認を付与する必要があります。

1. （オプション） **オブジェクトタイプ**&#x200B;の名前をクリックします。

   Workfront Planningでレコードタイプページが開きます。

## 既存のリクエストをコピーしてリクエストを作成する

Workfrontのリクエストリストでリクエストをコピーし、その詳細を編集して新しいリクエストとして送信できます。

これは、新しいリクエストエクスペリエンスでのみ使用できます。

既存のPlanning リクエストをコピーし、新しいリクエストとして送信することは、既存のWorkfront リクエストをコピーすることと同じです。

詳しくは、[リクエストをコピーして送信](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)を参照してください。

## 既存のドラフトからのドラフトとリクエストの作成

リクエストのドラフトを作成してからドラフトに戻り、後でリクエストとして送信できます。

これは、新しいリクエストエクスペリエンスでのみ使用できます。 Workfront Planningで既存のドラフトからドラフトとリクエストを作成することは、Adobe Workfrontからドラフトを作成することと同じです。

詳しくは、[ドラフトからリクエストを作成](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md)を参照してください。

## ドラフトまたは送信されたリクエストの削除

新しいリクエストエクスペリエンスを使用すると、送信されたリクエストまたはそのドラフトを削除できます。

Planning リクエストを削除すると、次のことが発生します。

* リクエストを復元できません。
* リクエストから作成されたレコードは削除されません。
* 削除されたドラフトは復元できません。 下書きに関連付けられたレコードはありません。

プランニングリクエストの削除は、Workfront リクエストの削除と同様です。

詳しくは、[送信されたリクエストの削除またはドラフトのリクエスト &#x200B;](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md)を参照してください。







