---
title: AdobeMaestro での共有権限の概要
description: 自分が作成したAdobeMaestro ワークスペースに対する権限を共有または削除できます。 ワークスペースを作成および共有できるのは、Workfrontの管理者のみです。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 2%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://experienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!-- *********add to TOC****************-->

# AdobeMaestro での共有権限の概要

自分が作成したAdobeMaestro ワークスペースに対する権限を共有または削除できます。 ワークスペースを作成および共有できるのは、Workfrontの管理者のみです。

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro にアクセスするには、Ypu がWorkfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

## AdobeMaestro で共有できるオブジェクト

Maestro では、以下のオブジェクトを共有できます。

* ワークスペース

  ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。

## Maestro でのオブジェクトの共有に関する考慮事項

* Workfront管理者のみがワークスペースを共有できます。
* すべてのWorkfront管理者は、他のユーザーが作成したワークスペースにアクセスして共有できます。
* ワークスペースを一括で共有することはできません。
* ワークスペースを次のエンティティと共有できます。
   * ユーザー
   * グループ

## Maestro オブジェクトに対する権限の共有

次の表に、Maestro ワークスペースを共有する際に選択できる権限のレベルを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p><b>権限レベル</b></p></td> 
   <td> <p><b>実行できるアクション</b></p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>ビュー</p></td> 
   <td> 
    <ul> 
     <li>ワークスペースの表示</li> 
     <li>ワークスペース内のすべてのレコードの種類を表示する</li> 
     <li>レコードタイプ内のすべてのレコードを表示</li> 
     <li>レコードタイプのすべてのフィールドを表示する</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>参加</p></td> 
   <td>  
    <ul> 
     <li>表示権限に含まれるすべてのアクション</li> 
     <li>レコードを追加</li>
     <li>レコードを作成</li> 
     <li>レコードを削除</li>  
     <li>レコードを編集</li>
     <li>フィールド設定を編集</li>
     </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>管理</p></td> 
   <td> 
    <ul> 
     <li>表示および投稿権限に含まれるすべてのアクション</li> 
     <li>レコードタイプを編集</li> 
     <li>レコードタイプの作成</li> 
     <li>レコードタイプを削除</li> 
     <li>フィールドを追加</li> 
     <li>フィールドを削除</li> 
     <li>レコードタイプ間に新しい接続を追加する</li> 
     <li>ワークスペースをユーザーおよびグループと共有する</li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Workfront管理者</p></td> 
   <td> <p>これはマエストロの許可ではありません。</p>
   <p> すべてのWorkfront管理者は、次の操作を実行できます。 </p>
   <ul><li>ワークスペースの作成</li>
    <li> 既存のワークスペースを、自分で作成していない場合でも管理します。 </li> 
    <li>ワークスペース内のすべての情報（レコードの種類、レコード、フィールド）の管理
    </td> 
  </tr> 
 </tbody> 
</table>

<!-- the following sections are hidden in the links below - ensure they are visible-->

## ワークスペースの共有

Maestro ワークスペースの共有については、 [AdobeMaestro へのアクセスを許可](../access/grant-access.md).

## ワークスペースに対する権限の削除

Maestro ワークスペースの共有については、 [AdobeMaestro へのアクセスを許可](../access/grant-access.md).

<!--This is currently not possible: ## Request permissions to objects -->
