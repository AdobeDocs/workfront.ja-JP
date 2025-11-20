---
title: レコードの共有
description: 「共有」ボタンを使用してレコードを共有すると、Adobe Workfront Planning でのコラボレーションを強化できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 10%

---


<!--update metadata with real information at release-->

# レコードの共有

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

レコードタイプ内の個々のレコードに対するユーザーの権限を調整できます。 O

次の方法で Adobe Workfront Planning レコードを共有できます。

* レコードへのリンクの共有。

  詳しくは、「[&#x200B; リンクを使用してレコードを共有する &#x200B;](/help/quicksilver/planning/records/share-records.md)」を参照してください。

* ワークスペースとレコードタイプを共有することで、ワークスペース内のすべてのレコードを他のユーザーと共有します。

  詳しくは、次の記事を参照してください。

   * [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

   * [レコードタイプの共有](/help/quicksilver/planning/access/share-record-types.md)

* 「**共有** オプションを使用してレコードを共有します。

  この記事では、「**共有** オプションを使用して他のユーザーとレコードを共有する方法について説明します。

>[!IMPORTANT]
>
>ワークスペースへのアクセス権を持つユーザーには、ワークスペース内のすべてのレコードに対する少なくとも表示権限が自動的に付与されます。
>ビューを共有しても、レコードに対する権限はユーザーに付与されません。 共有ワークスペースのみが、レコードタイプとレコードに対する権限をユーザーに付与できます。
>
>Adobe Workfront Planning でのオブジェクトの共有の一般的な情報については、[Workfront Planning での共有権限の概要 &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md) も参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>任意のWorkfrontおよび Planning パッケージ</p> 
または
<p>任意のワークフローおよび計画パッケージ</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
   <p><b>メモ</b></p>
   <p>標準ライセンスを持つユーザーのみが、レコードに対する管理権限を付与できます。 その他のライセンスは、表示権限のみを持つことができ、管理オプションは淡色表示されます。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペース、レコードタイプおよびレコードに対する権限の管理</p>  
   <p><b>重要</b></p>
   <p>ワークスペースに対する管理権限を持つユーザーのみがレコードを共有できます</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## レコードを共有する際の考慮事項

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* 人物、グループ、チーム、会社、担当業務のエンティティとレコードを共有できます。
* ワークスペースをユーザーと共有すると、デフォルトでは、ユーザーはワークスペース内のレコードに対しても同じ権限を受け取ります。
* ワークスペースからエンティティを削除すると、すべての共有権限がレコードタイプとその中のすべてのレコードから削除されます。
* レコードに対するユーザーのアクセスは、次の 3 つの設定を組み合わせて決定されます。

   * レコードタイプおよびワークスペースから継承された権限
   * レコード共有ダイアログで個別に追加された権限
   * 次の権限：

      * **ワークスペース内の全員が表示できます**：これにより、ワークスペース内の全員がレコードを表示できるように <!-- is this OK to say "workspace? should it be "record"??--> ります
      * **招待されたユーザーのみがアクセスできます**：これはデフォルトで選択されており、レコードへのアクセスを特定のユーザーに制限できます。

* レコードに付与できる権限レベルは次のとおりです。

   * 表示
   * 管理

* ユーザーとレコードを共有すると、デフォルトでは、レコードタイプに対する権限と同じ権限で追加されます。

  例：

   * レコードタイプに対する表示権限を持っている場合、レコードに対する表示権限を取得します
   * レコードタイプに対する投稿権限または管理権限を持っている場合、レコードに対する管理権限を取得します

* ワークスペースマネージャーは、ワークスペースに属していないユーザーとレコードを共有できます。 この場合、追加されたエンティティの横に、ワークスペースへのアクセス権がないことを知らせる警告が表示されます。 ユーザーを承認してレコードとワークスペースの両方に追加するか、ワークスペースへの追加を拒否してレコードから削除することもできます。

* ワークスペースに対する管理権限を持つユーザーとレコードを共有すると、デフォルトでは、そのレコードに対する管理権限も取得されます。 表示権限は淡色表示されます。

* ワークスペースにユーザーを追加する権限がない場合は、既にワークスペースに追加されているユーザー、チーム、グループ、役割および会社のみが表示および追加されます。 ワークスペースにまだ含まれていない他のエンティティは追加できません。

* 単一のレコードに対して継承された権限を無効にすることができます。この場合、権限を個別に付与することも、「ワークスペース内の全員」オプションに属している場合は権限を取得することもできます。<!-- is this OK to say "workspace? should it be "record"??-->

* 同じユーザーに対して複数の共有権限が適用される場合、それらの権限のうち最も高い権限を受け取ります。

  例えば、レコードが表示権限を持つユーザーと共有され、そのレコードのグループが管理アクセス権を持つ場合、そのレコードに対する管理権限を取得します。

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 連結レコードの数式フィールドまたはルックアップ フィールドが、アクセス権のないレコードのフィールドに基づいている場合、そのレコードがアクセスできない要因となっている正しい計算が表示されます。

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## レコードの共有権限

