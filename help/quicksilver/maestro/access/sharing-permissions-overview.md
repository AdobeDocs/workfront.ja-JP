---
title: AdobeMaestro での共有権限の概要
description: 自分が作成したAdobeMaestro ワークスペースに対する権限を共有または削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: fda35538234593b66b01f9e0cc0dafd6a63a84dc
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 4%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!-- *********add to TOC****************-->

# AdobeMaestro での共有権限の概要

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro にアクセスするには、Ypu がWorkfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

自分が作成したAdobeMaestro ワークスペースに対する権限を共有または削除できます。

## AdobeMaestro で共有できるオブジェクト

Maestro では、以下のオブジェクトを共有できます。

* ワークスペース

  ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。 ビューは共有されません。

* ビュー

## Maestro でのオブジェクトの共有に関する考慮事項

* Maestro でワークスペースを作成するには、次のライセンスが必要です。

   * 新しい価格モデル：標準ライセンス
   * 現在の価格モデル：勤務先またはそれ以上のライセンス
* システム管理者は、他のユーザーが作成したワークスペースを管理および共有できます。
* システム管理者でない場合は、他のユーザーが作成したワークスペース（共有している場合）に投稿できます。
* ワークスペースを一括で共有することはできません。
* ワークスペースを次のエンティティと共有できます。
   * ユーザー
   * グループ
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。

## Maestro オブジェクトに対する権限の共有

次の表に、Maestro ワークスペースまたはビューを共有する際に選択できる権限のレベルを示します。

<table>
  <tr>


</td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td><p><b>新規：標準ライセンス</b></p> <p><b>現在：作業者以上のライセンス</b></p></strong>
   </td>
   <td><strong>権限の管理</strong>
   </td>
   <td><strong>Contribute の権限</strong>
   </td>
   <td><strong>権限を表示</strong>
   </td>
  </tr>
  <tr>
   <td><strong>作成</strong>
   </td>
   <td rowspan="5" ><strong>Workspace</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>削除</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>共有</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>編集</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>ビュー</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>作成/削除</strong>
   </td>
   <td rowspan="3" ><strong>レコードタイプ*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>編集</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>ビュー</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>作成/削除</strong>
   </td>
   <td rowspan="3" ><strong>レコード*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>編集</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>ビュー</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <tr>
   <td><strong>作成</strong>
   </td>
   <td rowspan="5" ><strong>ビュー</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>削除</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>共有</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>編集</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>ビュー</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>✓
   </td>
  </tr>

<tr>
   <td><strong>作成/削除</strong>
   </td>
   <td rowspan="3" ><strong>フィールド*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>編集</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>ビュー</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>



</table>

*レコードのタイプ、レコード、フィールドは、ワークスペースから権限を継承します。

Maestro でのアクセスに関する一般的な情報については、 [AdobeMaestro での共有権限の概要](../access/sharing-permissions-overview.md).

ワークスペースの共有について詳しくは、 [ワークスペースの共有](/help/quicksilver/maestro/access/share-workspaces.md).

ビューの共有について詳しくは、 [ビューの共有](/help/quicksilver/maestro/access/share-views.md)

