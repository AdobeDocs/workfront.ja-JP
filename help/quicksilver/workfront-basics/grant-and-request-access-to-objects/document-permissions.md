---
title: ドキュメントの共有
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront管理者は、ドキュメントへのアクセス権の付与で説明されているように、アクセスレベルを割り当てる際に、ドキュメントの表示または編集のためのアクセス権をユーザーに付与します。
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# ドキュメントの共有

Adobe Workfront管理者は、アクセスレベルを割り当てる際に、ユーザーにドキュメントの表示や編集のアクセス権を付与します。詳しくは、 [ドキュメントへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Workfront管理者がユーザーに付与するアクセスレベルでは、ユーザーはドキュメントの表示または編集を行うことができます。 これに加えて、他のユーザーも、自分でアップロードした特定のドキュメントを表示または管理する権限や、自分が共有するアクセス権を持つ他のユーザーに付与することができます。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。 オブジェクトの権限について詳しくは、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

デフォルトでは、Workfrontにドキュメントをアップロードするユーザーには、そのドキュメントに対する管理権限が付与されています。

ドキュメントフォルダー全体の共有について詳しくは、 [ドキュメントフォルダーの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## ドキュメントの共有に関する考慮事項

以下の考慮事項に加えて、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理者は、システム内のすべてのユーザーに対して、それらの項目の所有者にならずに、システム内の項目に対する権限を追加または削除できます。

* ドキュメントの共有は、Workfrontでの他のオブジェクトの共有と似ています。 Workfrontでドキュメントを共有する方法について詳しくは、 [オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* ドキュメントには次の権限を付与できます。

   * ビュー
   * 管理

* ドキュメントを公開またはシステム全体で共有することもできます。

   >[!CAUTION]
   >
   >機密情報を含むオブジェクトを外部のユーザーと共有する場合は、慎重におこなうことをお勧めします。 これにより、Workfrontのユーザーや組織の一員でなくても、ユーザーは情報を表示できます。

* 「ドキュメントへのアクセスを許可」フィールドに電子メールアドレスを追加することで、Workfrontアカウントを持たないユーザーとドキュメントを共有できます。
* ドキュメントを共有すると、ユーザーはすべてのドキュメントバージョンとすべてのドキュメント配達確認に同じアクセス権を持ちます。\
   Workfrontでの校正について詳しくは、 [校正](../../review-and-approve-work/proofing/proofing.md) 」セクションに入力します。

* ドキュメントに対する権限は、ドキュメントに関連付けられているオブジェクトから継承できます。 Workfront管理者は、アクセスレベルでドキュメントの権限の継承を制限できます。

   ドキュメントに対する継承された権限の制限について詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   ドキュメントの継承された権限は手動で削除できます。 詳しくは、 [オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* 添付されたドキュメントは、添付されたオブジェクトからのみ権限を継承します。 オブジェクト上にフォルダーを作成し、ドキュメントをフォルダーに移動すると、そのフォルダーの権限が継承されます。 ただし、親オブジェクトまたは親オブジェクト上にフォルダを作成し、ドキュメントをそのフォルダに移動した場合、そのフォルダの権限は継承されません。

## ドキュメント権限

次の表に、ユーザーがドキュメントの表示や管理を許可する際に付与できる権限を示します。

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>アクション</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>ビュー</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">作成</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">ドキュメントの詳細を編集</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">削除*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">ダウンロード</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">チェックアウト</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">承認者を追加</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">ドキュメントを承認</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">カスタムフォームを添付</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">カスタムフィールドの編集</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移動先（オブジェクト）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">送信先（統合）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更新/コメント</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">新しいバージョンをアップロード</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">バージョンを削除</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">ドキュメントを表示</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">プレビュー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proof**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">プルーフの作成**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">プルーフを削除**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">共有*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">システム全体で共有*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">ドキュメントをパブリックにして共有*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">外部の電子メールアドレスと共有</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">追加/削除</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">名前を変更</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">リンク（統合と）</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">リンク解除（統合と）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; アクションは、ドキュメントフォルダとドキュメントフォルダの両方で共有されます。

&#42;&#42; ドキュメントの配達確認をおこなうには、Workfrontアカウントに対応する個別の校正ライセンスが必要です。 校正ライセンスの取得については、担当のアカウントマネージャーにお問い合わせください。 Workfrontでの校正について詳しくは、 [校正](../../review-and-approve-work/proofing/proofing.md).
