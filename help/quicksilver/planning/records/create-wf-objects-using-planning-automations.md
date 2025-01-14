---
title: Workfront計画レコードの自動作成を使用したAdobe Workfront オブジェクトの作成
description: Workfront Planning で自動化を構成し、アクティブ化するとWorkfrontにオブジェクトを作成できます。
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 10%

---

# Adobe Workfrontの計画レコードの自動作成を使用したオブジェクトの作成

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Adobe Workfront Planning でオートメーションを構成して、アクティブ化するとWorkfrontまたはWorkfront Planning にオブジェクトを作成できます。

レコードのページで自動処理を設定して有効化できます。 作成されたオブジェクトは、プランニング レコードに接続され、自動化で指定したフィールドに配置されます。

例えば、Workfront Planning キャンペーンを受け取り、Workfrontでプロジェクトを作成して、そのキャンペーンの進行状況を追跡する自動処理を作成できます。 プロジェクトは、Workfront Planning キャンペーンに接続されます。

接続されたレコードについて詳しくは、「[ 接続されたレコードの概要 ](/help/quicksilver/planning/records/connected-records-overview.md)」を参照してください。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

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
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
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
   <td> 標準
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>作成するオブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム）のWorkfrontでのアクセス権を編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードの追加先となるワークスペースに対する権限を管理します。 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 自動処理を使用したオブジェクトとレコードの作成に関する考慮事項

* 新しいオブジェクトまたはレコード名は、作成元のレコード名と同じです。
* オートメーションを使用するレコードで、新しいオブジェクトの追加先として選択したフィールドに、同じタイプのオブジェクトが既に接続されている場合、新しいオブジェクトは接続フィールドに追加され、既存のオブジェクトも接続されたままになります。

## Workfront Planning での自動処理の設定

Workfront Planning を使用してオブジェクトを作成する前に、自動処理を設定する必要があります。

{{step1-to-planning}}

1. レコードの種類カードをクリックし、レコードの名前をクリックします。

   レコードタイプのページが開きます。
1. レコードタイプ名の右 ![](assets/more-menu.png) にある **その他** メニューをクリックし、**自動化の管理** をクリックします。

   使用可能な自動化のリストが開きます。

1. 画面の右上隅にある「**新しいオートメーション**」をクリックします。 **新しい自動化** ボックスが開きます。
1. 次のフィールドを更新します。

   * **名称未設定のオートメーション** を、オートメーションボタンに表示するテキストに置き換えます。 自動処理を使用してWorkfront オブジェクトを作成する際に、このボタンをクリックします。
   * **説明**：説明を追加して、自動化の目的を特定します。

1. 自動処理の詳細ページの「**トリガー**」セクションで、次のフィールドを更新します。

   * **トリガー**：自動処理をトリガーにするアクションを選択します。 例えば、「**ボタンをクリック**」を選択します。<!--update this step with a list of all possible triggers; right not only Button click is available-->

1. 「**アクション**」セクションの次のフィールドを更新します。
   * **オブジェクトタイプ**：オートメーションで作成するオブジェクトを選択します。 必須フィールドです。

     Workfront計画レコードから次のオブジェクトを作成できます。

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * グループ
      * レコード
1. （条件付き）作成するオブジェクトのタイプに応じて、次のフィールドを更新します。

   * **プロジェクト**:
      * **オブジェクトが作成される「接続」フィールド**：新しいプロジェクトが表示される「接続」フィールドです。 これは必須フィールドです
      * **プロジェクトを作成するテンプレート**:Workfrontでプロジェクトの作成に使用するプロジェクトテンプレートを選択します。
   * **Portfolio**:
      * **オブジェクトが作成される接続フィールド**：新しいポートフォリオが表示される接続フィールドです。 必須フィールドです。
      * **新しいポートフォリオに添付するカスタムフォーム**：新しいポートフォリオに添付するカスタムフォームを選択します。 ポートフォリオのカスタム フォームを作成してから選択する必要があります。
   * **プログラム**:
      * **オブジェクトが作成される接続フィールド**：新しいプログラムが表示される接続フィールドです。 必須フィールドです。
      * **プログラムポートフォリオ**：新しいプログラムが追加されるポートフォリオを選択します。 必須フィールドです。
      * 
         * **新しいプログラムに添付するカスタムフォーム**：新しいプログラムに添付するカスタムフォームを選択します。 選択する前に、プログラムカスタムフォームを作成する必要があります。
   * **グループ**:
      * **オブジェクトが作成される接続フィールド**：新しいグループが表示される接続フィールドです。 必須フィールドです。
      * **新規グループに添付するカスタムフォーム**：新しいプログラムに添付するカスタムフォームを選択します。 選択する前に、プログラムカスタムフォームを作成する必要があります。
   * **レコード**:
      * **接続されたレコードタイプ**：作成するレコードタイプを選択します。
      * **レコードが作成される接続されたフィールド**：これは、新しいレコードが表示される接続されたフィールドです。 必須フィールドです。
      * **フィールドをマッピング**：オートメーションが作成されるレコードタイプからフィールドを選択して、接続されたレコードタイプのフィールドにマッピングします。
      * **接続されたレコードフィールドに対して**：自動処理を作成するレコードタイプのフィールドに対応するフィールドを、接続されたレコードから選択します。
1. （オプションおよび条件付き）Workfront オブジェクトタイプの接続フィールドがない場合は、「**接続フィールドを作成**」アイコンをクリックしてフィールドを追加し ![](assets/create-a-connection-field-icon.png) す。
1. （オプションおよび条件付き）レコードの追加を選択した場合は、「**フィールドのマッピング****フィールドのマッピング** 領域で「追加」をクリックして追加フィールドを追加し、**転送元** フィールドと **転送先** フィールドを選択して、最初に選択したレコードのどのフィールドを、接続されたレコードのフィールドに表示するかを指定します。
1. **保存**&#x200B;をクリックします。

   自動処理は自動処理のリストに表示され、レコードで使用できます。
1. （オプション）オートメーションを編集、無効化、または削除するには、以下の手順を実行します。

   自動処理のリストで、保存済みの自動処理の名前にポインタを合わせて **詳細** メニュー ![](assets/more-menu.png) ージをクリックし、次のいずれかのオプションを選択します。

   * **編集**：自動処理に関する情報を更新し、フィールドを設定します。
   * **無効**：自動処理は、レコードのテーブルビューのツールバーにオプションとして表示されず、ユーザーはレコードやオブジェクトの作成に使用できなくなります。 再び使用できるようにするには、**その他** メニュー ![](assets/more-menu.png) ージをもう一度クリックしてから、**アクティブ化** をクリックします。
   * **削除**：自動処理は削除され、復元できません。 自動処理を使用して作成されたレコードは、最初に選択されたレコードに接続されたままになります。

## Workfront Planning 自動処理を使用したオブジェクトの作成

1. Workfront Planning で、Workfrontオブジェクトの作成に使用するレコードを含む「レコード・タイプ」ページを開きます。
1. テーブル表示を開きます。
1. 1 つ以上のレコードを選択します。

   テーブルの下部に青いバーが表示され、オートメーションボタンなどの追加ボタンも表示されます。
1. 画面の右下隅付近にあるオートメーションボタンをクリックします。

   ![ オートメーションボタン ](assets/automation-custom-button.png)

   新しいオブジェクトは、オートメーションボタンの設定で指定した接続フィールドに表示されます。

   >[!NOTE]
   >
   >オブジェクトが作成され、期待どおりに接続されたことを確認することをお勧めします。

1. （オプション）接続フィールドで新しいオブジェクトをクリックします。 オブジェクトページが開き、新しいオブジェクトに追加の変更を加えることができます。

<!--you might need to add something about notifications and emails?!-->
