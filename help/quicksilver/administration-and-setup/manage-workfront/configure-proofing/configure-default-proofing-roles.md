---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: デフォルトのプルーフの役割の設定
description: Adobe Workfront の管理者は、Workfront で作成したプルーフにアクセスするユーザーおよびゲストユーザーに対して、デフォルトのプルーフの役割を設定できます。プルーフにユーザーを追加するどんな担当者でも、そのユーザーのこれらの役割を調整できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '508'
ht-degree: 100%

---

# デフォルトのプルーフの役割の設定

Adobe Workfront の管理者は、Workfront で作成したプルーフにアクセスするユーザーおよびゲストユーザーに対して、デフォルトのプルーフの役割を設定できます。プルーフにユーザーを追加するどんな担当者でも、そのユーザーのこれらの役割を調整できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront 管理者である必要があります。Workfront 管理者について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## デフォルトのプルーフの役割の設定

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 左側に表示されるリストの下部付近にある&#x200B;**レビューと承認**&#x200B;をクリックします。
1. **ドキュメント プルーフ受信指定者の役割**&#x200B;セクションで、プルーフのワークフローに追加されるユーザーとゲストユーザーのデフォルトの役割を選択します。

   各プルーフの役割とそれに関連付けられている権限の一覧について詳しくは、以下の[プルーフの役割に関連付けられた権限](#rights-associated-with-proofing-roles)を参照してください。

   >[!NOTE]
   >
   >* この設定は、役割の設定後に Workfront システムで作成されたユーザーにのみ適用され、既存のユーザーには適用されません。
   >* [Adobe Workfront 内でのプルーフの共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)内の[プルーフにユーザーを追加](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)で説明したように、プルーフにユーザーを追加する担当者は、この役割を調整できます。

1. **ドキュメントプルーフを開く受信者以外のユーザーの役割**&#x200B;セクションで、プルーフにアクセスできるがプルーフのワークフローに追加されていないユーザーとゲストユーザーのデフォルトの役割を選択します。

   この状況は、プルーフが作成されたドキュメントにユーザーとゲストがアクセスできる場合に発生します。プルーフのワークフローに追加されていなくても、プルーフを開くことができます。

   **例：**&#x200B;この設定の使用方法の例を次に示します。

   * コメントの追加や、それを求められたユーザーの決定など、すべてのプルーフアクティビティを制限するには、「**読み取り専用**」を選択します。
   * チームの任意のメンバーがプルーフにマークアップやコメントを追加できるようにしたいので、**レビュアー**&#x200B;を選択します。

1. 「**保存**」をクリックします。

## プルーフの役割に関連付けられた権限 {#rights-associated-with-proofing-roles}

次の表に、各役割とそれに関連する権限を示します。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>プルーフを表示</strong> </p> </th> 
   <th> <p><strong>マークアップを追加</strong> </p> </th> 
   <th> <p><strong>コメントを追加</strong> </p> </th> 
   <th> <p><strong>返信がない場合は自分のコメントを編集</strong> </p> </th> 
   <th> <p><strong>決定を下す</strong> </p> </th> 
   <th> <p><strong>他のユーザーが残したコメントを削除</strong> </p> </th> 
   <th>コメントを解決</th> 
   <th>コメントにアクションを適用</th> 
   <th> <p><strong>プルーフを編集</strong> </p> </th> 
   <th>他のユーザーとプルーフを共有</th> 
   <th>新しいバージョンを作成</th> 
   <th> <p><strong>ホームエリアでの承認リクエストの表示</strong> </p> </th> 
   <th>新しいレビュー担当者を追加</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>読み取り専用</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レビュアー</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>承認者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レビュアーと承認者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>調整者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>新しい Workfront プランのユーザーは、システム内の任意のユーザーに作成者またはモデレーターの役割を付与できます。従来のプランのユーザーは、システム内のプルーフライセンスを持つユーザーに作成者またはモデレーターの役割を付与できます。
