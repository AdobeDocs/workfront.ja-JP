---
title: Adobe Workfront計画リクエストの発行
description: Adobe Workfront Planning の「レコードタイプ」ページでユーザーがリクエストフォームへのリンクを共有すると、リクエストを追加して、リクエストフォームに関連付けられた「レコードタイプ」のレコードを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '2176'
ht-degree: 3%

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

Workfront ユーザーと外部ユーザーは、Planning レコード タイプに対して要求を送信できます。 リクエストは、リクエストフォームに関連付けられたレコードタイプのレコードを作成します。<!--double check on the external users-->

ワークスペースマネージャーがリクエストフォームを作成し、レコードタイプに関連付ける方法について詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

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
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>Workfront ユーザーの場合は、ワークスペースおよびレコードタイプに対する以上の権限を表示します。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 前提条件

Workfront Planning 要求フォームに要求を送信するには、次の手順を実行する必要があります。

* Workfront Planning には、次のものが存在する必要があります。

   * ワークスペース
   * レコードタイプ
   * レコードタイプに関連付けられたリクエストフォーム。

     詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

* リクエストフォームは、アクセス可能な方法で共有する必要があります。 次のシナリオが存在します。

   * 内部的には、フォームは、ワークスペースに対する表示以上の権限を持つユーザーと共有する必要があります。

     Workfront ユーザーは、リンクからフォームにアクセスするか、Workfrontの「リクエスト」エリアでリクエストフォームを見つけることができます。

   * 外部的に使用する場合、Workfront アカウントを持たない外部のユーザーとレコードフォームへのリンクを共有します。

     また、Workfront ユーザーは、外部のユーザーと共有されているリンクにアクセスすることもできます。

* リンクと共有する場合、フォームへのリンクの有効期限を切ってはいけません。

## Workfront Planning への要求の送信に関する考慮事項

* Workfrontでリクエストを送信した後に編集することはできません。
* 送信された各リクエストでは、使用するフォームに関連付けられたレコードタイプのレコードが作成されます。フォームが承認に関連付けられていない場合や、すべての承認者によって承認が付与された場合は、送信されます。
* リクエストフォームを送信して作成されたレコードは、Workfront Planning で他の方法を使用して追加されたレコードと同一です。

  詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* リクエストフォームを送信することで作成されたレコードは、元のリクエストに接続されます。 この接続は削除できません。
* 次の領域で、作成されたレコードとリクエストの両方を表示できます。
   * Workfrontのリクエスト エリア

  <div class="preview">

   * 「元のリクエスト接続」フィールドの任意のレコードタイプページのレコード
   * 「元のリクエスト接続」フィールドのレコードの「詳細プレビュー」ボックス

  </div>
* 送信されたリクエストは、Workfrontの「リクエスト」領域に表示されます。
* 送信された Planning 要求は、新しい要求エクスペリエンスでのみ表示されます。 従来のリクエストエクスペリエンスでは、Planning リクエストを表示できません。
詳しくは、[ リクエストの作成と送信 ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) を参照してください。
* フォーム送信後のリクエストフォームまたはリクエストの詳細ページでの特定のフィールドタイプの表示方法には制限があります。

  詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Workfrontの「リクエスト」領域で、Workfront Planning にリクエストを送信します。

{{step1-to-requests}}

1. 画面の右上隅にある「**新しいエクスペリエンスに切り替え** 設定を有効にします。
この設定を有効にすると、Workfrontの計画リクエストフォームがWorkfrontの **リクエスト** エリアで使用できるようになります。

   >[!TIP]
   >
   >この設定は、Workfront インスタンスがAdobe統合エクスペリエンスにオンボードされている場合にのみ使用できます。
   >
   >このエリアでWorkfront計画リクエストを発行するには、次の条件を満たす必要があります。
   >
   >* Workfront Planning ライセンスを購入しました。
   >
   >* 1 つ以上のワークスペースを表示するアクセス権があります。

1. **送信するリクエスト** バーをクリックして、リクエストフォームのリストを開きます。
1. リストからリクエストフォームを選択するか、リクエストフォーム名の入力を開始し、リストに表示されたら選択します。

   ウィンドウが開き、上部にリクエストフォーム名が表示されます。
1. リクエストフォームで使用可能なフィールドを更新します。 赤いアスタリスクが付いているフィールドは必須です。
1. 「**送信**」をクリックします。

   リクエストフォームが閉じ、「**リクエスト** エリアに戻ります。

   フォームが送信され、次の処理が行われます。

   * リクエストフォームが承認と関連付けられていない場合、リクエストはWorkfrontの「リクエスト」エリアの「リクエスト」リストとホームの「マイリクエスト」ウィジェットに追加され、新しいレコードがフォームに関連付けられたレコードタイプに追加されます。

     次のフィールドは、ホームのリクエスト エリアとマイリクエストウィジェットにリクエストとレコードの情報を表示します。

      * **件名**:「リクエスト」領域に追加された元のリクエストの名前。 リクエストリストから **件名** フィールドを非表示または削除することはできません。
      * **作成されたオブジェクト**：リクエストから作成され、Planning に表示されるレコードの名前。
      * **オブジェクトタイプ**：ワークスペースの名前と、Planning のリクエストからレコードが作成されたレコードタイプ。
      * **ステータス**：リクエストオブジェクトのステータス。
      * **リクエストフォーム**:Planning のレコードタイプに関連付けられたリクエストフォームの名前。

   * リクエストフォームが承認に関連付けられている場合、リクエストは、Workfront リクエスト エリアとマイリクエストウィジェットのリクエストリストに、レビュー保留中のステータスで追加されます。 新しいレコードは、承認者が承認した後にのみ、レコードタイプページに追加されます。

     詳しくは、[ リクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

   * <span class="preview"> 「元の要求」接続フィールドは、元の要求の名前を表示する Planning のレコード・タイプに追加できます。 詳しくは、[ レコードタイプの接続 ](/help/quicksilver/planning/architecture/connect-record-types.md) を参照してください。</span>
   * リクエストは、所有者、承認者、および少なくともワークスペースに対する表示権限を持つ人物にのみ表示されます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。

   * アプリ内と、リクエストが正常に送信されたかレビュー用に送信された旨のメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者は、リクエストをレビューして承認するためのアプリ内通知とメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experience にオンボードされている場合にのみ表示されます。
     >
     >メールの確認または承認通知にリクエストへのリンクがあります。

1. （任意）確認メッセージで「**リクエストを表示**」をクリックしてリクエストを開くか、「**X**」アイコンをクリックして確認を閉じます。
1. （オプション）リクエスト リストから、次のいずれかの操作を行います。

   * 「**フィルター**」をクリックして、「リクエスト」リストに表示するリクエストの条件の追加を開始します。

     ![ リクエスト エリアでのフィルターの編集 ](assets/filters-editing-box-in-requests-planning-tab.png)

     次のフィールドでフィルタリングできます。

      * **Workspace**: リクエストフォームが関連付けられているワークスペース。
      * **レコードタイプ**：リクエストフォームが関連付けられているレコードタイプ。
      * **エントリ日**：リクエストが送信された日付。
      * **リクエストフォーム**：リクエストの送信に使用されるリクエストフォームの名前。
      * **ステータス**：リクエストのステータス。
      * **入力者**：リクエストを追加したユーザーの名前。 Workfront以外のユーザーがリクエストを追加した場合は、「入力者 **フィールドに** が表示さ `N/A` ます。
      * **作成されたオブジェクトステータス**：作成されたレコードのステータス。

     複数のフィルターを **And** または **Or** で結合できます。
フィルター条件を追加すると、リクエストリストが自動的にフィルタリングされます。

   * **列** をクリックして **フィールドの表示と順序** ボックスを開き、リクエストリストの列を非表示、表示、再配置します。

     >[!TIP]
     >
     >これ以上列を追加することはできません。

     ![ リクエスト領域の列編集ボックス ](assets/columns-editing-box-in-requests-planning-tab.png)
   * リクエストリストの右上隅にある「**+**」アイコンをクリックして **列マネージャー** を開き、リクエストリストの列を追加または削除します。

1. リスト内のリクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![ コメント付きのリクエストページ ](assets/new-request-page-with-comment.png)

1. （オプション）「コメント **領域にコメントを入力し** す。
1. （条件付き）リクエストフォームが承認と関連付けられていない場合、またはリクエストが承認されている場合は、リクエストの名前をクリックし、「作成されたオブジェクト **フィールドのレコードの名前をクリック** ます。

   Workfront Planning でレコードのページが開きます。

   >[!TIP]
   >
   >* レコードのプライマリフィールドがリクエストフォームで更新されなかった場合、リクエストのレコードフィールドのレコードの名前は **名称未設定** と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合、リクエストページからレコードにアクセスするには、承認を付与する必要があります。

1. （オプション） **レコードタイプ** の名前をクリックします。

   Workfront Planning に「レコードタイプ」ページが開きます。

## リクエストフォームへの共有リンクからWorkfront Planning にリクエストを送信する

この節の情報は、共有リンクからリクエストを送信するWorkfront ユーザーにのみ適用されます。 外部のユーザーは、リクエストやホームなど、Workfrontの内部領域にアクセスできません。

1. Workfront Planning レコードタイプから共有されたリンクに移動します。

1. フォームで使用可能なフィールドを更新します。 アスタリスクの付いたフィールドは必須です。

   >[!TIP]
   >
   >   **件名** フィールドが使用可能な場合、リクエストの送信後に、Workfront Planning に表示されません。
   >
   >新しいレコードがWorkfront Planning のレコードタイプに追加された際に識別可能になるように、リクエストのできるだけ多くのフィールドを更新することをお勧めします。

1. 「**送信**」をクリックします。

   フォームが送信され、次の処理が行われます。

   * リクエストフォームが承認と関連付けられていない場合、リクエストはWorkfrontの「リクエスト」エリアの「リクエスト」リストとホームの「マイリクエスト」ウィジェットに追加され、新しいレコードがフォームに関連付けられたレコードタイプに追加されます。

   * リクエストフォームが承認に関連付けられている場合、リクエストはWorkfrontの「リクエスト」エリアとマイリクエストウィジェットの「リクエスト」リストに追加されます。 新しいレコードは、すべての承認者が承認した後にのみ、レコードタイプページに追加されます。

     詳しくは、[ リクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

     >[!IMPORTANT]
     >
     >表示可能な少なくとも権限を持つ、自分または他のユーザーがワークスペースに送信したリクエストのみを表示できます。 Workfront管理者は、システム内の任意のワークスペースに送信されたすべてのリクエストを表示できます。<!--ensure this is correct; asking team in slack-->

   * アプリ内と、リクエストが正常に送信されたかレビュー用に送信された旨のメール通知が届きます。
   * リクエストフォームが承認に関連付けられている場合、承認者は、リクエストをレビューして承認するためのアプリ内通知とメール通知を受け取ります。

     >[!NOTE]
     >
     >メールおよびアプリ内通知は、組織のWorkfront インスタンスがAdobe Unified Experience にオンボードされている場合にのみ表示されます。

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. （任意）「**リクエストを表示**」をクリックして、Workfrontでリクエストを開きます。

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. （オプション） **メインメニュー**/**リクエスト** をクリックしてリクエストを表示し、リクエストの名前をクリックします。

   リクエストの詳細ページが開きます。

   ![ コメント付きのリクエストページ ](assets/new-request-page-with-comment.png)

1. （オプション）「コメント」領域にコメントを入力します。
1. （条件付き）リクエストフォームが承認と関連付けられていない場合、またはリクエストが承認されている場合は、リクエストの名前をクリックし、「作成されたオブジェクト **フィールドのレコードの名前をクリック** ます。

   Workfront Planning でレコードのページが開きます。

   >[!TIP]
   >
   >* レコード名がリクエストフォームに追加されなかった場合、リクエストのレコードフィールドのレコード名は **名称未設定** と表示されます。
   >
   >* リクエストフォームが承認に関連付けられている場合、リクエストページからレコードにアクセスするには、承認を付与する必要があります。

1. （オプション） **オブジェクトタイプ** の名前をクリックします。

   Workfront Planning に「レコードタイプ」ページが開きます。

## 既存のリクエストをコピーしてリクエストを作成

Workfrontのリクエストリストでリクエストをコピーし、詳細を編集して新しいリクエストとして送信できます。

これは、新しいリクエスト側エクスペリエンスでのみ使用できます。

手順については、[ リクエストのコピーと送信 ](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md) を参照してください。

## 既存のドラフトからのドラフトとリクエストの作成

リクエストのドラフトを作成したあとドラフトに戻り、後でリクエストとして送信できます。

これは、新しいリクエスト側エクスペリエンスでのみ使用できます。

手順については、[ ドラフトからのリクエストの作成 ](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md) を参照してください。



