---
title: ドキュメントの共有
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 管理者は、ドキュメントへのアクセス権の付与で説明されているように、アクセスレベルを割り当てる際に、ドキュメントの表示または編集のためのアクセス権をユーザーに付与します。
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '580'
ht-degree: 100%

---

# ドキュメントの共有

Adobe Workfront 管理者は、[ドキュメントへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)で説明されているように、アクセスレベルを割り当てる際に、ドキュメントの表示または編集のためのアクセス権をユーザーに付与します。

Workfront 管理者がユーザーに付与するアクセスレベルによって、ユーザーはドキュメントの表示または編集を行うことができます。これに加えて、他のユーザーも、自分でアップロードしたか、あるいは自分が共有のアクセス権を持つ特定のドキュメントを表示または管理する権限を他のユーザーに付与することができます。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。オブジェクトの権限について詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

Workfront にドキュメントをアップロードするユーザーには、デフォルトで、そのドキュメントに対する管理権限が付与されています。

ドキュメントフォルダー全体の共有について詳しくは、[ドキュメントフォルダーの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)を参照してください。

## ドキュメントの共有に関する考慮事項

以下の考慮事項に加えて、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)も参照してください。

>[!NOTE]
>
>Workfront 管理者は、システム内のすべてのユーザーに対して、システム内のアイテムに対する権限の追加や削除を、それらのアイテムの所有者にならなくても行うことができます。

* ドキュメントの共有は、Workfront で他のオブジェクトを共有する方法と同様です。Workfront でドキュメントを共有する方法について詳しくは、[オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。
* ドキュメントには、次の権限を付与できます。

   * 表示
   * 管理

* ドキュメントを公開またはシステム全体で共有することもできます。

  >[!CAUTION]
  >
  >機密情報を含んだオブジェクトを外部ユーザーと共有する場合は、注意することをお勧めします。Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

* 「ドキュメントへのアクセス権の付与先」フィールドにメールアドレスを追加することで、Workfront アカウントを持たないユーザーとドキュメントを共有できます。
* ドキュメントを共有すると、ユーザーはすべてのドキュメントバージョンとすべてのドキュメントプルーフに同じアクセス権を持ちます。\
  Workfront でのプルーフについて詳しくは、[プルーフ](../../review-and-approve-work/proofing/proofing.md)の節を参照してください。

* ドキュメントに対する権限は、ドキュメントに関連付けられているオブジェクトから継承できます。Workfront 管理者は、アクセスレベルでドキュメントの権限の継承を制限できます。

  ドキュメントに対する継承された権限の制限について詳しくは、[カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

  ドキュメントの継承された権限は手動で削除できます。詳しくは、[オブジェクトからの権限の削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください

* 添付されたドキュメントは、添付されたオブジェクトからのみ権限を継承します。オブジェクト上にフォルダーを作成し、ドキュメントをフォルダーに移動すると、そのフォルダーの権限が継承されます。ただし、親オブジェクトまたは祖父母オブジェクト上にフォルダーを作成し、ドキュメントをそのフォルダーに移動した場合、そのフォルダーの権限は継承されません。

## ドキュメント権限

次の表に、ユーザーにドキュメントの表示または管理を許可する際に付与できる権限を示します。

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>アクション</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>表示</strong> </p> </th> 
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
   <td scope="row">カスタムフィールドを編集</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移動（オブジェクト）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">送信先（統合）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">アップデート／コメント</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">新しいバージョンのアップロード</td> 
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
   <td scope="row">外部のメールアドレスと共有</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">追加／削除</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">名前を変更</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">リンク（統合を使用）</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">リンク解除（統合を使用）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; アクションは、ドキュメントとドキュメントフォルダーの両方で共有されます。

&#42;&#42; ドキュメントのプルーフを行えるようにするには、Workfront アカウントに対応する個別のプルーフライセンスが必要です。プルーフライセンスの取得については、アカウントマネージャーにお問い合わせください。Workfront でのプルーフについて詳しくは、[プルーフ](../../review-and-approve-work/proofing/proofing.md)を参照してください。
