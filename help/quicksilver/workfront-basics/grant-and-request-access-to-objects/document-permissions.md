---
title: ドキュメントの共有
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 管理者は、ドキュメントへのアクセス権の付与で説明されているように、アクセスレベルを割り当てる際に、ドキュメントの表示または編集のためのアクセス権をユーザーに付与します。
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 56%

---

# ドキュメントの共有

Adobe Workfront 管理者は、[ドキュメントへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)で説明されているように、アクセスレベルを割り当てる際に、ドキュメントの表示または編集のためのアクセス権をユーザーに付与します。

Workfront 管理者がユーザーに付与するアクセスレベルによって、ユーザーはドキュメントの表示または編集を行うことができます。これに加えて、他のユーザーも、自分でアップロードしたか、あるいは自分が共有のアクセス権を持つ特定のドキュメントを表示または管理する権限を他のユーザーに付与することができます。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。オブジェクトの権限について詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

Workfront にドキュメントをアップロードするユーザーには、デフォルトで、そのドキュメントに対する管理権限が付与されています。

ドキュメントフォルダー全体の共有について詳しくは、[ドキュメントフォルダーの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

オブジェクトを共有するには、次の条件を満たしている必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：標準</p> 
   または
   <p>現在：ワーク以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>共有するオブジェクトに対する表示以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>共有するオブジェクトに対する表示またはそれ以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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

## ドキュメントの共有

{{step1-to-documents}}

1. **ドキュメント** ページで、共有するドキュメントの上にマウスポインターを置き、表示される **ドキュメントの詳細** リンクをクリックします。 **ドキュメントの詳細** ページが開きます。

   ![ ドキュメントの詳細リンク ](assets/document-details-link.png)

1. ドキュメント名の右側にある **その他** アイコン ![ その他のアイコン ](assets/more-icon.png) をクリックし、「**共有**」をクリックします。 **共有 [ ドキュメント名]** ダイアログボックスが開きます。

   ![ドキュメントを共有](assets/share-a-document-350x160.png)

1. **ドキュメントへのアクセスの許可** フィールドに、ドキュメントを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >ドキュメントを共有できるのは、アクティブなユーザー、チーム、役割または会社のみです。


1. （オプション） **アクセスできるユーザー** ドロップダウンを選択し、ドキュメントのアクセスレベルを選択します。

   * **招待されたユーザーのみがアクセスできます：** ドキュメントに招待されたユーザーのみがドキュメントにアクセスできます（デフォルト）。
   * **システム内の全員が閲覧可能**：システム内のすべてのユーザーが、招待なしにドキュメントを閲覧できます。

1. （オプション）ドキュメントを公開するには、歯車アイコンをクリック ![ 歯車アイコンを選択 ](assets/gear-icon.png) し、「**これを外部ユーザーに公開** とインラインのボックスをクリックします。 **公開リンクをコピー** ボタンがダイアログボックスの下部に表示されます。

1. ユーザー名の右側のドロップダウンをクリックし、このドキュメントに対する権限レベルを選択します。

   * **表示**：ユーザーは、ドキュメントをレビューおよび共有できます。
   * **管理**：ユーザーは、管理者権限を持たずにドキュメントへのフルアクセス権を持ちます。これは、アクセスレベルで付与されます（すべての表示権限も含まれます）。

1. （オプション）付与した権限レベルの横にある「詳細オプション」アイコンをクリックして、ドキュメントに対する特定の権限を設定します。

   ![ 設定済みの高度な権限オプション ](assets/advanced-options-icon.png)

1. （オプション）ドキュメントの子オブジェクトに対する継承された権限をオフにするには、**継承された権限** でインライン **オフ** をクリックします。

1. （任意）ドキュメントを外部ユーザーと共有できる公開リンクをコピーするには、「**公開リンクをコピー**」をクリックします。

   >[!CAUTION]
   >
   >機密情報を含むドキュメントを外部ユーザーと共有する場合は注意が必要です。 Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

1. 「**保存**」をクリックします。

## ドキュメントの一括共有

{{step1-to-documents}}

1. **文書** ページの **すべての文書** タブで、キーボードの **Command** （Mac）または **Ctrl** （Windows）を押しながら、共有する各文書をクリックします。

1. ページの上部にある「**共有**」アイコン ![ 共有アイコン ](assets/share-icon.png) をクリックします。 共有モーダルが開きます。

   ![ 共有アイコン ](assets/share-documents-in-bulk.png)

1. **ドキュメントへのアクセスの許可** フィールドに、ドキュメントを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >ドキュメントを共有できるのは、アクティブなユーザー、チーム、役割または会社のみです。


1. （オプション） **アクセスできるユーザー** ドロップダウンを選択し、ドキュメントのアクセスレベルを選択します。

   * **招待されたユーザーのみがアクセスできます：** ドキュメントに招待されたユーザーのみがドキュメントにアクセスできます（デフォルト）。
   * **システム内の全員が閲覧可能**：システム内のすべてのユーザーが、招待なしにドキュメントを閲覧できます。

1. ユーザー名の右側にあるドロップダウンをクリックし、ドキュメントに対する権限レベルを選択します。

   * **表示**：ユーザーは、ドキュメントをレビューおよび共有できます。
   * **管理**：ユーザーは、管理者権限を持たないドキュメントへのフルアクセス権を持ちます。これは、アクセスレベルで付与されます（すべての表示権限も含まれます）。

1. （オプション）付与した権限レベルの横にある「詳細オプション」アイコンをクリックして、ドキュメントに対する特定の権限を設定します。

   ![ 設定済みの高度な権限オプション ](assets/advanced-options-icon.png)

1. **保存**&#x200B;をクリックします。


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
