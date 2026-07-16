---
title: レコードのデフォルト権限の設定
description: レコードの種類またはワークスペース設定を変更する際に、レコードのデフォルトの権限を設定できます。 レコードタイプに追加されるすべてのレコードに対して、オープン権限または制限付き権限を付与できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 9ef64f5a39c94426b2158c6504b913c8cb749c8e
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 5%

---


# レコードのデフォルト権限の設定

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}


レコードの種類またはワークスペース設定を変更する際に、レコードのデフォルトの権限を設定できます。

レコードタイプに追加されるすべてのレコードに対して、オープン権限または制限付き権限を付与できます。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p> 
または
<p>スタンドアロンの製品パッケージとしてのWorkfront Planningは</p>

</tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
   <p><b>メモ</b></p>
   <p>レコードに対する管理権限を付与できるのは、標準ライセンスを持つユーザーのみです。 他のすべてのライセンスには表示権限しかなく、「管理」オプションはグレー表示されます。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペースとレコードタイプに対する権限の管理</p>  
   <p><b>重要</b></p>
   <p>ワークスペースへの管理権限を持つユーザーのみがレコードを共有できます</p></td> 
  </tr>
</tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## デフォルトのレコード権限の設定に関する考慮事項

デフォルトのレコード権限を設定する際は、次の点を考慮してください。

* 一度にレコードタイプごとにアクティブにできるデフォルトの権限ルールは1つだけです。
* ルールの変更は、変更後に作成されたレコードにのみ影響します。 既存のレコードは、現在の権限を保持します。
* システム管理者とワークスペースマネージャーは、ルールに関係なく、すべてのレコードへのアクセスを常に管理できます。
* レコードを作成すると、デフォルトのルールに影響を与えることなく、共有ダイアログで権限を個別に変更できます。
* グローバルレコードタイプの場合、各ワークスペース（プライマリおよびセカンダリ）は独自のデフォルトルールを設定でき、新しいレコードは作成されるワークスペースのルールを引き受けます。

## ワークスペースのデフォルトのレコード権限の設定

1. ワークスペース > **詳細** メニュー![詳細メニュー](assets/more-menu.png) > **設定** > **レコードタイプ**&#x200B;に移動します。

   ![Workspace レコードタイプの設定領域](assets/workspace-record-types-settings-area.png)

1. （オプション） **レコードタイプ**&#x200B;のセル内をクリックして、レコードタイプ名を編集します。

1. **新規レコード権限のデフォルト**&#x200B;列で、権限を更新するレコードタイプのセルをクリックします。

1. 次のオプションから選択します。

   * **開く**：すべてのワークスペースのコントリビューターは、新しく作成したレコードを管理できます。 これは、既存および新規のすべてのレコードタイプの現在のデフォルト動作です。
   * **制限付き**：新しく作成されたレコードを編集できるのは、レコード作成者と明示的に追加したユーザーのみです。 他の人は表示のみのアクセスとなります。

1. （条件付き）デフォルトの権限を&#x200B;**制限付き**&#x200B;から&#x200B;**オープン**&#x200B;に変更する場合は、「**オープンに切り替え**」ボックスの「**切り替え**」をクリックして、選択を確定します。
1. （条件付き）制限付き&#x200B;**を選択した場合は、** レコードを編集できるユーザー&#x200B;**列に追加の編集者を追加します。**&#x200B;ユーザー、グループ、チーム、役割、または会社を追加できます。

   >[!NOTE]
   >
   >* レコード作成者は常に含まれ、削除できません。
   >* 既にレコードタイプに対するContributeまたはManage権限を持つエンティティのみを選択できます。

   変更は自動的に保存されます。 保存すると、ルールはすぐに有効になり、そのレコードタイプ用に作成されたすべてのレコードに自動的に適用されます。

## レコードタイプのデフォルトのレコード権限の設定

1. レコードタイプ > **詳細** メニュー![詳細メニュー](assets/more-menu.png) > **設定** > **レコード設定**&#x200B;に移動します。

   ![ レコードタイプ設定エリアの「レコード設定」タブ ](assets/record-settings-tab-in-record-type-settings-area.png)

1. **レコード権限タイプ** フィールドで、次のいずれかのオプションをクリックします。

   * **開く**：すべてのワークスペースのコントリビューターは、新しく作成したレコードを管理できます。 これは、既存および新規のすべてのレコードタイプの現在のデフォルト動作です。
   * **制限付き**：新しく作成されたレコードを編集できるのは、レコード作成者と明示的に追加したユーザーのみです。 他の人は表示のみのアクセスとなります。
1. （条件付き）デフォルトの権限を&#x200B;**制限付き**&#x200B;から&#x200B;**オープン**&#x200B;に変更する場合は、「**オープンに切り替え**」ボックスの「**切り替え**」をクリックして、選択を確定します。
1. （条件付き）制限付き&#x200B;**を選択した場合は、** レコードを編集できるユーザー&#x200B;**フィールドに追加の編集者を追加します。**&#x200B;ユーザー、グループ、チーム、役割、または会社を追加できます。

   >[!NOTE]
   >
   >* レコード作成者は常に含まれ、削除できません。
   >* 既にレコードタイプに対するContributeまたはManage権限を持つエンティティのみを選択できます。

   変更は自動的に保存されます。 保存すると、ルールはすぐに有効になり、そのレコードタイプ用に作成されたすべてのレコードに自動的に適用されます。