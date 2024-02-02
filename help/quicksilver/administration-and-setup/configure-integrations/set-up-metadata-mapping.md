---
title: メタデータマッピングの設定
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: メタデータは、ドキュメントに関連付けられた記述的情報です。 [!DNL Workfront]  アプリケーションに送信するドキュメントにメタデータが入るように  [!DNL Adobe Workfront]  を設定することができます。
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: ht
source-wordcount: '614'
ht-degree: 100%

---

# メタデータマッピングの設定

メタデータは、ドキュメントに関連付けられた記述的情報です。[!DNL Workfront] アプリケーションに送信するドキュメントにメタデータが入るように [!DNL Adobe Workfront] を設定することができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!DNL Workfront] メタデータについて

[!DNL Workfront] 内のドキュメントのメタデータは、関連するプロジェクト名、タスクの説明、予定完了日などの情報を入れることができます。[!DNL Workfront] 管理者は、[!DNL Workfront] から次の [!DNL Workfront] アプリケーションに送信されるドキュメントにメタデータが入るように、[!DNL Workfront] を設定することができます。

* [!DNL Workfront DAM]

メタデータをドキュメントと共に送信する前に、まず入れたいメタデータを指定またはマッピングする必要があります。[!DNL Workfront] で使用するどのフィールドでもマッピングできます。メタデータマッピングを設定すると、[!DNL Workfront] アプリケーションにアップロードされたすべてのドキュメントには、マッピングされたメタデータが入ります。

ユーザーが [!DNL Workfront] から [!DNL Workfront] アプリケーションにドキュメントを送信すると、マッピングされたメタデータは、ドキュメントと共に転送されます。[!DNL Workfront] アプリケーションのドキュメントのバージョンが [!DNL Workfront] にリンクされている場合、[!DNL Workfront] のドキュメントのメタデータに対して行われた変更は、[!DNL Workfront] アプリケーションのドキュメントのメタデータには反映されません。[!DNL Workfront] にマッピングされたフィールドが変更された場合、更新されたメタデータが入った新しいバージョンのドキュメントを [!DNL Workfront] アプリケーションに送信する必要があります。

>[!NOTE]
>
>メタデータのマッピングは、[!DNL Workfront] から [!DNL Workfront DAM]. への 1 方向にのみ実行できます。[!DNL Workfront DAM] から [!DNL Workfront] にリンクされたドキュメントのメタデータは、Workfront に転送できません。

様々な [!DNL Workfront DAM] のメタデータフィールドに同じ [!DNL Workfront] フィールドをマッピングできますが、複数の [!DNL Workfront] メタデータフィールドに対しては、そのアプリケーションのどれでも、メタデータフィールドを使用することはできません。

複数の [!DNL Workfront] フィールドを構成して [!DNL Workfront] アプリケーションの 1 つのメタデータフィールドに書き出すには、最初に [!DNL Workfront] に計算カスタムフィールドを作成して、オブジェクトの個々のカスタムフィールドをすべて表示します。次に、計算 [!DNL Workfront] フィールドを [!DNL Workfront] アプリケーションのメタフィールドにマッピングします。計算カスタムフィールドについて詳しくは、[カスタムフォームに計算データを追加](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)を参照してください。

メタデータマッピングプロセスのフィールドをマッピングする前に、[!DNL Workfront] でアプリケーションを有効にする必要があります。詳しくは、[ドキュメント統合を設定](../../administration-and-setup/configure-integrations/configure-document-integrations.md)を参照してください。

## メタデータを送信するように [!DNL Workfront] を設定

1. [!DNL Adobe Workfront] の右上にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン（![](assets/main-menu-icon.png)）をクリックし、**[!UICONTROL 設定]**&#x200B;アイコン（![](assets/gear-icon-settings.png)）をクリックします。

1. 左側のパネルで、**[!UICONTROL ドキュメント]**／**[!UICONTROL メタデータ マッピング]**&#x200B;をクリックします。

   ![](assets/metadata-mapping.png)

1. 「**[!UICONTROL マッピングのソース フィールドを選択]**」ボックスで、[!DNL Workfront DAM] にマッピングする Workfront フィールドの名前を一部入力し、名前がリストに表示されたらそれを選択します。
1. 「**[!UICONTROL マッピングのターゲット フィールドを選択]**」ボックスで、選択した [!DNL Workfront] フィールドの情報を入力するフィールドを選択します。

1. 「**[!UICONTROL マッピングを追加]**」をクリックします。

   マッピングされたフィールドは、ページの下部にリストアップされるマッピングされたフィールドに表示されます。

1. 必要なすべての [!DNL Workfront] フィールドとそれに対応する [!DNL Workfront DAM] フィールドを追加するまで、手順 5 と 6 を繰り返します。

## マッピングされたフィールドを削除

1. [!DNL Workfront] に管理者としてログインします。
1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、**[!UICONTROL ドキュメント]**／**[!UICONTROL メタデータ マッピング]**&#x200B;をクリックします。

1. マッピングされたフィールドのリストで、メタデータマッピングから削除するフィールドを選択します。
1. 「**[!UICONTROL 削除]**」をクリックします。

   指定されたフィールドはもうマッピングされていません。ユーザーが [!DNL Workfront] から [!DNL Workfront DAM] にドキュメントを送信しても、削除されたフィールド内にあったメタデータは、ドキュメントと共に転送されなくなりました。

   マッピングされたフィールドを削除する前に送信されたドキュメントには、削除されたフィールドのメタデータを含む、送信された元のメタデータが保持されます。
