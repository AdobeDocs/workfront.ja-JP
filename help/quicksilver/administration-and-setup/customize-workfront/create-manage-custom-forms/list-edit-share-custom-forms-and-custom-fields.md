---
title: カスタムフォームに追加されたカスタムフォームとウィジェットを一覧表示して編集する
description: 組織のカスタムフォームと、それらに追加されたカスタムフィールドおよびウィジェットのリストを表示する場合、ツールバーのオプションを使用して、プロパティの編集、プロパティの共有者の制限、コピー、削除を行うことができます。また、各カスタムフォームに関連付けられているオブジェクトタイプなど、表示される列のその他の情報を表示することもできます。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
hidefromtoc: true
hide: true
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 92%

---


# カスタムフォームに追加されたカスタムフォームとウィジェットを一覧表示して編集する

組織のカスタムフォームと、それらに追加されたカスタムフィールドおよびウィジェットのリストを表示する場合、ツールバーのオプションを使用して、プロパティの編集、プロパティの共有者の制限、コピー、削除を行うことができます。また、各カスタムフォームに関連付けられているオブジェクトタイプなど、表示される列のその他の情報を表示することもできます。

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、[フォームデザイナーを使用してフォームをデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>プラン</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## カスタムフォームに追加されたカスタムフォームと項目を一覧表示して編集する

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 「**カスタムフォーム**」をクリックします。

   「**フォーム**」タブが選択されると、組織のすべてのカスタムフォームがその説明とともに表示され、関連付けられたオブジェクトタイプ、作成したユーザーの名前、システム内でアクティブかどうかが表示されます。

   リストでカスタムフォームを選択する際に実行できる操作について詳しくは、次の記事を参照してください。

   * [フォームデザイナーでフォームをデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [カスタムフォームを共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
   * [カスタムフォームをコピーして新しいフォームを作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md)
   * [カスタムフォームを削除または非アクティブ化](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md)

1. 「**フィールド**」タブをクリックします。

   このタブには、システム内のユーザーがカスタムフォームに追加したカスタムフィールドとウィジェット、各項目のタイプに関する情報、手順と詳細、およびそれを含むカスタムフォームのリストが表示されます。

   このリストには、次の条件の 1 つ以上を満たすカスタムフォーム項目のみが含まれます。

   * 編集可能なシステム全体
   * システム全体に表示
   * ユーザーによる作成
   * 表示または管理アクセス権を持つ共有された項目

   >[!NOTE]
   >
   >セクション区切りは、「フィールド」タブには表示されません。

   リスト内の項目を選択した場合に実行できる操作について詳しくは、次の記事を参照してください。

   * [ カスタムフィールド、セクション区切りまたはウィジェットの追加または編集 ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md)
   * [フォームのカスタムフィールドとウィジェットの共有を設定する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md)
   * [システムからカスタムフィールドまたはウィジェットを削除](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md)

1. 「**セクション**」タブを選択して、**パラメーターグループ**&#x200B;がリストの&#x200B;**表示**&#x200B;として選択されていることを確認してください。

   このビューには、すべてのセクション区切りが表示され、各セクション区切りを含むカスタムフォームのリストも表示されます。

   リストから選択したカスタム セクションの編集の詳細については、「[ フォームの整理とプレビュー ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)」を参照してください。

