---
title: Adobe Workfront計画リクエストの発行
description: Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '1914'
ht-degree: 6%

---

# レコードを作成するためのAdobe Workfront Planning 要求の発行

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Workspace Manager がAdobe Workfront Planning でレコードタイプのリクエストフォームを作成したら、そのフォームを使用してリクエストを送信できます。これにより、フォームに関連付けられたレコードタイプのレコードが作成されます。

次の領域からWorkfront計画リクエストを発行できます。

* Workfrontの「リクエスト」エリアから。
* 直接リンクから共有されたリクエストフォームへ。

  ここでは、Workfrontの「リクエスト」エリアまたは共有リンクからレコードタイプに新しいレコードを追加するリクエストを送信する方法について説明します。
* 新規レコードを追加または要求する場合は、「レコードタイプ」ページから。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

Workfront ユーザーと外部ユーザーは、Planning レコードタイプに対してリクエストを送信し、レコードを作成できます。<!--double check on the external users-->

ワークスペースマネージャーがリクエストフォームを作成し、レコードタイプに関連付ける方法について詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <p>外部、コントリビューター、ライト、または標準のライセンス</p>
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
   <p>Workfront ユーザーの場合は、ワークスペース <span class="preview"> およびレコードタイプ </span> に対する表示以上の権限</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontのプランニング エリアにアクセスするには、次のレイアウトテンプレート設定が必要です。 </p>
<ul>
<li><p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p></li>
<li><div class="preview">
<p> プレビュー環境では、ライトまたはコントリビューターライセンスを持つユーザーには、Planning を含むレイアウトテンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>

<p> ただし、Workfront Planning にリクエストを送信するために Planning エリアにアクセスする必要はありません。 </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 前提条件

Workfront Planning 要求フォームに要求を送信するには、次の手順を実行する必要があります。

* Workfront Planning には、次のものが存在する必要があります。

   * ワークスペース
   * レコードタイプ。
   * レコードタイプに関連付けられたリクエストフォーム。

     詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

* リクエストフォームは、アクセス可能な方法で共有する必要があります。 次のシナリオが存在します。

   * 内部的には、フォームは、ワークスペースに対する表示以上の権限を持つユーザーと共有する必要があります。

     Workfront ユーザーは、リンクからフォームにアクセスするか、Workfrontの「リクエスト」エリアでリクエストフォームを見つけることができます。

   * Workfront アカウントをお持ちでない場合、フォームへのリンクが外部のユーザーと共有されています。

     また、Workfront ユーザーは、外部のユーザーと共有されているリンクにアクセスすることもできます。

* フォームへのリンクは期限切れにできません。

## Workfront Planning への要求の送信に関する考慮事項

* Workfrontでリクエストを送信した後に編集することはできません。
* 送信された各リクエストでは、使用するフォームに関連付けられたレコードタイプのレコードが作成されます。フォームが承認に関連付けられていない場合や、すべての承認者によって承認が付与された場合は、送信されます。
* リクエストフォームを送信して作成されたレコードを、Workfront Planning で他の方法を使用して追加されたレコードと区別することはできません。

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* 送信されたリクエストは、Workfrontの「リクエスト」領域の「送信済み」セクションの「計画」タブに表示されます。
* フォーム送信後のリクエストフォームまたはリクエストの詳細ページでの特定のフィールドタイプの表示方法には制限があります。

  詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Workfrontの「リクエスト」領域で、Workfront Planning にリクエストを送信します。

{{step1-to-requests}}

1. 画面の右上隅にある「**新しいエクスペリエンスに切り替え** 設定を有効にします。
この設定を有効にすると、Workfrontの計画リクエストフォームがWorkfrontの **リクエスト** エリアで使用できるようになります。

   >[!TIP]
   >
   >この設定は、次の環境が整っている場合にのみ使用できます。
   >
   >* 貴社はWorkfrontプランニングのパッケージを購入されました。
   >* お使いのWorkfront インスタンスは、Adobe Unified Experience にオンボードされます。
   >* 1 つ以上のワークスペースを表示するアクセス権があります。
   >

1. **新規リクエスト** をクリックします。

   ![Workfrontと Planning の統合カードを含む新しいリクエストボックス ](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   **新規リクエスト** ボックスが開き、次の情報が表示されます。

   * 最近アクセスした 6 つのWorkfront リクエストキューおよび Planning リクエストフォームが「最近」セクションに表示されます。
   * 50 個の追加のWorkfront リクエストキューおよび Planning のリクエストフォームが、「すべてのリクエストフォーム **セクションにアルファベット順に表示され** す。 デフォルトで表示されないリクエストキューを検索できます。

1. 次のいずれかの操作を行います。

   * 「最近」または「すべてのリクエストフォーム」セクションで、Planning リクエストフォームのいずれかのカードをクリックします
   * 検索ボックスに Planning 要求フォームの名前の入力を開始し、リストに表示されたらカードをクリックします。

   リクエストフォームが開きます。

1. リクエストフォームで使用可能なフィールドを更新します。 赤いアスタリスクが付いているフィールドは必須です。
1. 「**送信**」をクリックします。

   リクエストフォームが閉じ、「**リクエスト** エリアに戻ります。

   フォームが送信され、次の処理が行われます。

   * リクエストフォームが承認に関連付けられていない場合、リクエストは「Workfront リクエスト」エリアの「送信済み」セクションの「計画」タブに追加され、新しいレコードがフォームに関連付けられたレコードタイプに追加されます。

   * リクエストフォームが承認に関連付けられている場合、リクエストは「Workfront リクエスト」エリアの「送信済み」セクションの「計画」タブに追加されます。 新しいレコードは、すべての承認者が承認した後にのみ、レコードタイプページに追加されます。

     詳しくは、[ リクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

     ![ 「統合ワークフロー計画」タブの切替スイッチが付いたリクエスト領域 ](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >1 つ以上のワークスペースにアクセスできるすべてのユーザーは、リクエスト エリアの「計画」タブを表示できます。 表示可能な少なくとも権限を持つ、自分または他のユーザーがワークスペースに送信したリクエストのみを表示できます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。

   * リクエストは、所有者、承認者、および少なくともワークスペースに対する表示権限を持つ人物にのみ表示されます。

   * アプリ内と、リクエストが正常に送信されたかレビュー用に送信された旨のメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者は、リクエストをレビューして承認するためのアプリ内通知とメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experience にオンボードされている場合にのみ表示されます。
     >
     >メールの確認または承認通知にリクエストへのリンクがあります。

1. （任意）確認メッセージで「**リクエストを表示**」をクリックしてリクエストを開くか、「**X**」アイコンをクリックして確認を閉じます。

1. （オプション） **リクエスト** エリアの「**計画**」タブをクリックしてリクエストを表示し、リクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![ リクエストの詳細ページ ](assets/request-details-page.png)

   <!--replace the step directly above with this when we release filters and columns: 
      1. (Optional) Click the **Planning** tab in the **Requests** area to view your requests. 
         All the requests you have access to view that were submitted to a Planning request form display in a list. 
      1. (Optional) Do any of the following:
         <div class="preview">
         * Click **Filters** and start adding conditions for what requests you want to view in the Planning tab. 
                     ![Editing filters in the Planning requests tab](assets/filters-editing-box-in-requests-planning-tab.png)
            You can filter by any of the following fields:  
            * **Workspace**: The workspace the request form is associated with.
            * **Record type**: The record type the request form is associated with.
            * **Entry date**: The date when the request was submitted.
            * **Request form**: The name of the request form used to submit the request.
            * **Status**: The status of the request.
            * **Entered by**: The name of the user who added the request. If the request was added with someone outside of Workfront, the **Entered by** field shows `N/A`.
            You can have multiple filters joined by either And or Or.  
            The request list is filtered automatically, as you add the filter conditions. 
         * Click **Columns** and hide, show, or rearrange the columns in the request list. 
            >[!TIP]
            >
            >You cannot add any more columns. 
            >
            >You cannot display the **Subject** field.
                     ![](assets/columns-editing-box-in-requests-planning-tab.png)

      1. Click the name of a request in the list. 
   The request details page opens. 
   ![Request details page](assets/request-details-page.png)             
      </div>
      -->


1. （条件付き）リクエストフォームが承認と関連付けられていない場合、またはリクエストが承認されている場合は、リクエストの名前をクリックし、「**レコード**」フィールドのレコードの名前をクリックします。

   Workfront Planning でレコードのページが開きます。

   >[!TIP]
   >
   >* レコードのプライマリフィールドがリクエストフォームで更新されなかった場合、リクエストのレコードフィールドのレコードの名前は **名称未設定** と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合、リクエストページからレコードにアクセスするには、承認を付与する必要があります。

1. （オプション） **レコードタイプ** の名前をクリックします。

   Workfront Planning に「レコードタイプ」ページが開きます。

## リクエストフォームへの共有リンクからWorkfront Planning にリクエストを送信する

1. Workfront Planning レコードタイプから共有されたリンクに移動します。

1. フォームで使用可能なフィールドを更新します。 アスタリスクの付いたフィールドは必須です。

   >[!TIP]
   >
   >   **件名** フィールドが使用可能な場合、リクエストの送信後に、Workfront Planning に表示されません。
   >
   >新しいレコードがWorkfront Planning のレコードタイプに追加された際に識別可能になるように、リクエストのできるだけ多くのフィールドを更新することをお勧めします。

1. 「**送信**」をクリックします。

   フォームが送信され、次の処理が行われます。

   * リクエストフォームが承認に関連付けられていない場合、リクエストは「Workfront リクエスト」エリアの「送信済み」セクションの「計画」タブに追加され、新しいレコードがフォームに関連付けられたレコードタイプに追加されます。

   * リクエストフォームが承認に関連付けられている場合、リクエストは「Workfront リクエスト」エリアの「送信済み」セクションの「計画」タブに追加されます。 新しいレコードは、すべての承認者が承認した後にのみ、レコードタイプページに追加されます。

     詳しくは、[ リクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

     ![ リクエストの「計画」タブ ](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >1 つ以上のワークスペースにアクセスできるすべてのユーザーは、リクエスト エリアの「計画」タブを表示できます。 表示可能な少なくとも権限を持つ、自分または他のユーザーがワークスペースに送信したリクエストのみを表示できます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。<!--ensure this is correct; asking team in slack-->

   * アプリ内と、リクエストが正常に送信されたかレビュー用に送信された旨のメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者は、リクエストをレビューして承認するためのアプリ内通知とメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experience にオンボードされている場合にのみ表示されます。

1. （任意）「**リクエストを表示**」をクリックして、Workfrontでリクエストを開きます。

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. （オプション） **メインメニュー**/**リクエスト**/**計画** タブをクリックしてリクエストを表示し、リクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![ リクエストの詳細ページ ](assets/request-details-page.png)

1. （条件付き）リクエストフォームが承認と関連付けられていない場合、またはリクエストが承認されている場合は、リクエストの名前をクリックし、「**レコード**」フィールドのレコードの名前をクリックします。

   Workfront Planning でレコードのページが開きます。

   >[!TIP]
   >
   >* レコード名がリクエストフォームに追加されなかった場合、リクエストのレコードフィールドのレコード名は **名称未設定** と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合、リクエストページからレコードにアクセスするには、承認を付与する必要があります。

1. （オプション） **レコードタイプ** の名前をクリックします。

   Workfront Planning に「レコードタイプ」ページが開きます。




