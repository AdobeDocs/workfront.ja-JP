---
title: Adobe Workfront計画リクエストの発行
description: Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 3942ba8d626a854344624bc5b7ea3ad01e8ad7fb
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 5%

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
* 新規レコードを追加または要求する場合は、「レコードタイプ」ページから。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

ここでは、Workfrontの「リクエスト」エリアまたは共有リンクからレコードタイプに新しいレコードを追加するリクエストを送信する方法について説明します。


Workfront ユーザーと外部ユーザーは、Planning レコードタイプに対してリクエストを送信し、レコードを作成できます。<!--double check on the external users-->

ワークスペースマネージャーがリクエストフォームを作成し、レコードタイプに関連付ける方法について詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p>
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
   <p>Workfront ユーザーの場合は、ワークスペースおよびレコードタイプに対する以上の権限を表示します。</p> 
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

     詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

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

  詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

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

<!--Production-->

1. 実稼動環境で、「**新規リクエスト**」をクリックします。

   <!--![New request box with unified Workfront and Planning cards](assets/new-request-box-with-unified-workfront-and-planning-cards.png-->

   **新規リクエスト** ボックスが開き、次の情報が表示されます。

   * 最近アクセスした 6 つのWorkfront リクエストキューおよび Planning リクエストフォームが「最近」セクションに表示されます。
   * 50 個の追加のWorkfront リクエストキューおよび Planning のリクエストフォームが、「すべてのリクエストフォーム **セクションにアルファベット順に表示され** す。 デフォルトで表示されないリクエストキューを検索できます。

1. 実稼動環境で、次のいずれかの操作を行います。

   * 「最近」または「すべて」の要求フォーム・セクションで、計画の要求フォームを選択します
   * 検索ボックスに Planning 要求フォームの名前の入力を開始し、リストに表示されたらカードをクリックします。

   リクエストフォームが開きます。

<!-- Put preview section here-->
1. <span class="preview"> プレビュー環境で、最近アクセスしたリクエストフォーム領域からリクエストフォームまたはキューを選択するか、リストにフォームまたはキュー名を入力してから、表示されたら選択します。

1. リクエストフォームで使用可能なフィールドを更新します。 赤いアスタリスクが付いているフィールドは必須です。
1. 「**送信**」をクリックします。

   リクエストフォームが閉じ、「**リクエスト** エリアに戻ります。

   フォームが送信され、次の処理が行われます。

   * リクエストフォームが承認に関連付けられていない場合、リクエストは「Workfront リクエスト」エリアの「送信済み」セクションの「計画」タブに追加され、新しいレコードがフォームに関連付けられたレコードタイプに追加されます。

   * リクエストフォームが承認に関連付けられている場合、リクエストは「Workfront リクエスト」エリアの「送信済み」セクションの「計画」タブに追加されます。 新しいレコードは、すべての承認者が承認した後にのみ、レコードタイプページに追加されます。

     詳しくは、[&#x200B; リクエストフォームへの承認の追加 &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

     ![&#x200B; 「統合ワークフロー計画」タブの切替スイッチが付いたリクエスト領域 &#x200B;](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

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

1. （任意）「**リクエスト**」エリアの「**計画**」タブをクリックして、リクエストを表示します。
Planning 要求フォームに送信された表示アクセス権を持つすべての要求がリストに表示されます。
1. （オプション）次のいずれかの操作を行います。

   * 「**フィルター**」をクリックして、「計画」タブに表示するリクエストの条件の追加を開始します。

     ![&#x200B; 「計画要求」タブでのフィルターの編集 &#x200B;](assets/filters-editing-box-in-requests-planning-tab.png)

     次のフィールドでフィルタリングできます。

      * **Workspace**: リクエストフォームが関連付けられているワークスペース。
      * **レコードタイプ**：リクエストフォームが関連付けられているレコードタイプ。
      * **エントリ日**：リクエストが送信された日付。
      * **リクエストフォーム**：リクエストの送信に使用されるリクエストフォームの名前。
      * **ステータス**：リクエストのステータス。
      * **入力者**：リクエストを追加したユーザーの名前。 Workfront以外のユーザーがリクエストを追加した場合は、「入力者 **フィールドに** が表示さ `N/A` ます。

        複数のフィルターを **And** または **Or** で結合できます。
フィルター条件を追加すると、リクエストリストが自動的にフィルタリングされます。

   * **列** をクリックし、リクエストリストの列の非表示、表示、並べ替えを行います。

     >[!TIP]
     >
     >これ以上列を追加することはできません。
     >
     >「**件名** フィールドを表示することはできません。

     ![](assets/columns-editing-box-in-requests-planning-tab.png)


1. リスト内のリクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![&#x200B; リクエストの詳細ページ &#x200B;](assets/request-details-page.png)

   <div class="preview">
      プレビュー：

   ![&#x200B; コメント付きのリクエストページ &#x200B;](assets/new-request-page-with-comment.png)

   </div>

1. <span class="preview"> （オプション）「コメント」領域にコメントを入力します。
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

     詳しくは、[&#x200B; リクエストフォームへの承認の追加 &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

     ![&#x200B; リクエストの「計画」タブ &#x200B;](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >1 つ以上のワークスペースにアクセスできるすべてのユーザーは、リクエスト エリアの「計画」タブを表示できます。 表示可能な少なくとも権限を持つ、自分または他のユーザーがワークスペースに送信したリクエストのみを表示できます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。<!--ensure this is correct; asking team in slack-->

   * アプリ内と、リクエストが正常に送信されたかレビュー用に送信された旨のメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者は、リクエストをレビューして承認するためのアプリ内通知とメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experience にオンボードされている場合にのみ表示されます。

   * <span class="preview"> 要求が承認され、レコードが作成された後、「承認者」および「承認日」フィールドに、承認に関する情報がレコードに表示されます。</span>

1. （任意）「**リクエストを表示**」をクリックして、Workfrontでリクエストを開きます。

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. （オプション） **メインメニュー**/**リクエスト**/**計画** タブをクリックしてリクエストを表示し、リクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![&#x200B; リクエストの詳細ページ &#x200B;](assets/request-details-page.png)

   <div class="preview">
   プレビュー：

   ![&#x200B; コメント付きのリクエストページ &#x200B;](assets/new-request-page-with-comment.png)

   </div>

1. <span class="preview"> （オプション）「コメント」領域にコメントを入力します。
1. （条件付き）リクエストフォームが承認と関連付けられていない場合、またはリクエストが承認されている場合は、リクエストの名前をクリックし、「**レコード**」フィールドのレコードの名前をクリックします。

   Workfront Planning でレコードのページが開きます。

   >[!TIP]
   >
   >* レコード名がリクエストフォームに追加されなかった場合、リクエストのレコードフィールドのレコード名は **名称未設定** と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合、リクエストページからレコードにアクセスするには、承認を付与する必要があります。

1. （オプション） **レコードタイプ** の名前をクリックします。

   Workfront Planning に「レコードタイプ」ページが開きます。




