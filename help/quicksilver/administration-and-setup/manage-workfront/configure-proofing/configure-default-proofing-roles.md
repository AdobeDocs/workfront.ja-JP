---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 既定の校正の役割を設定する
description: Adobe Workfrontの管理者は、Workfrontで作成した配達確認にアクセスするユーザーおよびゲストユーザーに対して、デフォルトの校正の役割を設定できます。 配達確認にユーザーを追加するユーザーは、そのユーザーの役割を調整できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 既定の校正の役割を設定する

Adobe Workfrontの管理者は、Workfrontで作成した配達確認にアクセスするユーザーおよびゲストユーザーに対して、デフォルトの校正の役割を設定できます。 配達確認にユーザーを追加するユーザーは、そのユーザーの役割を調整できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront管理者である。 Workfront管理者について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 既定の校正の役割を設定する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. クリック **レビューと承認** 左側に表示されるリストの下部付近にあります。
1. 内 **ドキュメント配達確認の指定受信者の役割** 「 」セクションで、配達確認のワークフローに追加されるユーザーとゲストユーザーのデフォルトの役割を選択します。

   詳しくは、 [校正ロールに関連付けられた権限](#rights-associated-with-proofing-roles) 以下に、各校正の役割と関連付けられている権限の一覧を示します。

   >[!NOTE]
   >
   >* この設定は、役割の設定後にWorkfrontシステムで作成されたユーザーにのみ適用されます。既存のユーザーには割り当てられません。
   >* 配達確認にユーザーを追加するユーザーは、この役割を調整できます。詳しくは、 [配達確認にユーザーを追加](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Adobe Workfront内での配達確認の共有](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. 内 **ドキュメント配達確認を開く非受信者の役割** 「 」セクションで、配達確認にアクセスできるが配達確認のワークフローに追加されていないユーザーとゲストユーザーに対するデフォルトの役割を選択します。

   この状況は、配達確認が作成されたドキュメントにユーザーとゲストがアクセスできる場合に発生します。配達確認のワークフローに追加されていなくても、配達確認を開くことができます。

   **例：** この設定の使用方法の例を次に示します。

   * 次を選択します。 **読み取り専用** ：コメントの追加や、コメントの実行を求められたユーザーに対する決定など、すべての配達確認アクティビティを制限する場合。
   * 次を選択します。 **レビュー担当者** チームの任意のメンバーが、配達確認にマークアップやコメントを追加できるようにしたいからです。

1. 「**保存**」をクリックします。

## 校正ロールに関連付けられた権限 {#rights-associated-with-proofing-roles}

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
   <th> <p><strong>配達確認を表示</strong> </p> </th> 
   <th> <p><strong>マークアップを追加</strong> </p> </th> 
   <th> <p><strong>コメントを追加</strong> </p> </th> 
   <th> <p><strong>返信がない場合は自分のコメントを編集</strong> </p> </th> 
   <th> <p><strong>決定を下す</strong> </p> </th> 
   <th> <p><strong>他のユーザーが行ったコメントを削除</strong> </p> </th> 
   <th>コメントを解決</th> 
   <th>コメントにアクションを適用</th> 
   <th> <p><strong>配達確認を編集</strong> </p> </th> 
   <th>他のユーザーと配達確認を共有</th> 
   <th>新しいバージョンを作成</th> 
   <th> <p><strong>ホーム領域での承認リクエストの表示</strong> </p> </th> 
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
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>承認者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レビュアーと承認者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>調整者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
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
>新しいWorkfrontプランのユーザーは、システム内の任意のユーザーに作成者またはモデレーターの役割を付与できます。 レガシープランのユーザーは、システム内の配達確認ライセンスを持つすべてのユーザーに、作成者またはモデレーターの役割を付与できます。
