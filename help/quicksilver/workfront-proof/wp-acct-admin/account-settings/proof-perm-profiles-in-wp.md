---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Workfront Proof のプルーフ権限プロファイル
description: Workfront 管理者または Workfront Proof 管理者は、プルーフ権限プロファイルをユーザーに割り当てて、システム内のすべてのプルーフに対してユーザーが持つプルーフ機能を指定できます。ユーザーのプルーフ権限プロファイルの設定について詳しくは、「Workfront Proof でのユーザーのプルーフ権限プロファイルの設定」を参照してください。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: ht
source-wordcount: '1766'
ht-degree: 100%

---

# [!DNL Workfront Proof] のプルーフ権限プロファイル

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

[!DNL Workfront] 管理者または [!DNL Workfront Proof] 管理者は、プルーフ権限プロファイルをユーザーに割り当てて、システム内のすべてのプルーフに対してユーザーが持つプルーフ機能を指定できます。ユーザーのプルーフ権限プロファイルの設定について詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md) でのユーザーのプルーフ権限プロファイルの設定を参照してください。

>[!NOTE]
>
>次の操作も実行できます。
>
>* 個々のプルーフに対して特定の役割をユーザーに付与します。プルーフの役割について詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) でのプルーフの役割の管理を参照してください。
>* 組織内のユーザーのカスタムプロファイルを作成します。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md) でのカスタムプロファイルの設定を参照してください。
>

次の表に、各プルーフ権限プロファイルで使用できる権限を示します。

| **自分の項目** |  |  |  |  | **他のユーザーの項目** |  |  | **管理** | **請求** |
|---|---|---|---|---|---|---|---|---|---|
|   | **追加** | **表示** | **編集** | **削除** | **表示** | **編集** | **削除** | **編集と削除** | **編集** |
| 請求管理者 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| 管理者 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| スーパーバイザ－ | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| マネージャー | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| オブザーバー |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| 訪問者 |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

役割と権限について、次の点を考慮してください。

* 割り当てられたプロファイル権限は、自分のアカウントのユーザーとアイテムにのみ関係します。ただし、サテライトアカウントの場合は例外です。メイン（ハブ）アカウントの管理者と請求管理者は、ハブアカウントレベルからアカウント設定および請求にアクセスし、管理できます。
* 請求管理者および管理者は、ユーザーを削除できます。これは、アカウント設定でのみ実行できます。
* 請求管理者および管理者が、自分のアカウント内の他のユーザーが所有するプルーフを表示する場合は、レビュアーの役割でプルーフを表示します。
* 請求管理者と管理者は、読み取り専用の役割を使用して、自分と共有されたフォルダーまたは自分が作成したフォルダー内のプルーフにアクセスできます。

次の節では、標準の[!DNL Workfront Proof] 設定のプロファイルに関連付けられている各プロファイルと権限について説明します。

* [請求管理者](#billing-administrator)
* [管理者](#administrator)
* [スーパーバイザ－](#supervisor)
* [マネージャー](#manager)
* [オブザーバー](#observer)
* [訪問者](#visitor)
* [ゲスト](#guest)

## 請求管理者 {#billing-administrator}

請求管理者は、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof]  の請求ページのアカウント設定](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)へのアクセス権、および次の権限があります。

![](assets/cleaner2.png)プルーフの生成、ファイルのアップロード、およびフォルダーの作成ができます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でのプルーフの生成、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) へのファイルと web コンテンツのアップロード、および [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) でのフォルダーの作成を参照してください。

![](assets/cleaner2.png)自分が作成したまたは所有するプルーフおよびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)組織内のすべてのユーザーが作成したプルーフおよびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)他のユーザーの公開フォルダーを削除できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/cleaner2.png)アカウントで作成されたすべてのプルーフに対する編集権限を持ちます。

![](assets/cleaner2.png)ドロップゾーンの所有者として設定できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) でドロップゾーンを設定を参照してください。

![](assets/cleaner2.png)請求ページにアクセスし、請求の詳細を編集できます。詳しくは、[ [!DNL Workfront Proof]  請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)を参照してください。

![](assets/cleaner2.png)アカウント設定ページにアクセスし、アカウントの詳細を編集できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) でのアカウント設定を参照してください。

![](assets/cleaner2.png)ごみ箱を空にできます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) でごみ箱を復元して空にするを参照してください。

![](assets/cleaner2.png)ユーザーを追加、編集および削除できます。

![](assets/cleaner2.png)グループを作成し、新しい連絡先を追加できます。

![](assets/cleaner2.png)連絡先を削除できます。

![](assets/cleaner2.png)返信がない場合にプルーフを編集できます。

![](assets/no2.png)プルーフの返信は編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダーは削除できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

アカウントの設定について詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) でのアカウント設定を参照してください。

請求について詳しくは、[ [!DNL Workfront Proof]  の請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)を参照してください。

### 管理者 {#administrator}

管理者は、[アカウント設定](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)へのアクセス権、および次の権限があります。

![](assets/cleaner2.png)プルーフを作成、ファイルをアップロード、フォルダーを作成できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でのプルーフの生成、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) へのファイルと web コンテンツのアップロード、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) でのフォルダーの作成を参照してください。

![](assets/cleaner2.png)作成したプルーフおよびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)組織内のすべてのユーザーが作成したプルーフおよびファイルを表示、編集、削除できます。

![](assets/cleaner2.png)他のユーザーの公開フォルダーを削除できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/cleaner2.png)アカウントで作成されたすべてのプルーフに対する編集権限を持ちます。

![](assets/cleaner2.png)ドロップゾーンの所有者として設定できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) でのドロップゾーンの設定を参照してください。

![](assets/cleaner2.png)アカウント設定ページにアクセスし、アカウントの詳細を編集できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) でのアカウント設定を参照してください。

![](assets/cleaner2.png)ごみ箱を空にできます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) のごみ箱のアイテムの復元と完全削除を参照してください。

![](assets/cleaner2.png)ユーザーを追加、編集、削除できます。

![](assets/cleaner2.png)グループを作成し、連絡先を新規に追加できます。

![](assets/cleaner2.png)連絡先を削除できます。

![](assets/cleaner2.png)返信がない場合にプルーフを編集できます。

![](assets/no2.png)プルーフの返信は編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダーは削除できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/no2.png)請求ページにアクセスしたり、請求の詳細を編集したりはできません。詳しくは、[ [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)を参照してください。

### スーパーバイザ－ {#supervisor}

スーパーバイザーには、次の権限があります。

![](assets/cleaner2.png)プルーフを作成、ファイルをアップロード、フォルダーを作成できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でのプルーフの生成、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) へのファイルと web コンテンツのアップロード、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) でのフォルダーの作成を参照してください。

![](assets/cleaner2.png)作成したプルーフおよびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)組織内のすべてのユーザーが作成したプルーフおよびファイルを表示、編集、削除できます。

![](assets/cleaner2.png)他のユーザーの公開フォルダーを削除できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/cleaner2.png)アカウントで作成されたすべてのプルーフに対する編集権限を持ちます。

![](assets/cleaner2.png)ドロップゾーンの所有者として設定できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) でのドロップゾーンの設定を参照してください。

![](assets/cleaner2.png)グループを作成し、連絡先を新規に追加できます。

![](assets/cleaner2.png)連絡先を削除できます。

![](assets/cleaner2.png)返信がない場合にプルーフを編集できます。

![](assets/no2.png)プルーフの返信は編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダーは削除できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md) でのフォルダーを参照してください。

![](assets/no2.png)請求ページまたはアカウント設定にはアクセスできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) での [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)と [ アカウント設定を参照してください。

![](assets/no2.png)ユーザーを追加、編集、削除できません。

![](assets/no2.png)ごみ箱を空にすることはできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) のごみ箱のアイテムの復元と完全削除を参照してください。

### マネージャー {#manager}

マネージャーには次の権限があります。

![](assets/cleaner2.png)プルーフを作成、ファイルをアップロード、フォルダーを作成できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でのプルーフの生成、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) へのファイルと web コンテンツのアップロード、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) でのフォルダーの作成を参照してください。

![](assets/cleaner2.png)自分が作成したまたは所有するプルーフおよびファイルを表示、編集、削除できます。

![](assets/cleaner2.png)明示的に共有されている他のユーザーのプルーフを表示、レビュー、承認できます（共有フォルダー内のすべてに対する読み取り専用権限）。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) でのプルーフの役割の管理を参照してください。

![](assets/cleaner2.png)グループを作成し、新しい連絡先を追加できます。

![](assets/no2.png)組織内の他のユーザーが作成したプルーフおよびファイルは表示、編集、削除できません。

![](assets/no2.png)プルーフまたは返信は編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダーは削除できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/no2.png)他のユーザーのパブリックフォルダーは削除できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/no2.png)請求ページまたはアカウント設定にはアクセスできません。詳しくは、[ [!DNL Workfront Proof]  の請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)と [ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) でのアカウント設定を参照してください。

![](assets/no2.png)ドロップゾーンの所有者として設定できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) でのドロップゾーンの設定を参照してください。

![](assets/no2.png)ごみ箱を空にすることはできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) でのごみ箱の復元と削除を参照してください。

![](assets/no2.png)ユーザーを追加、編集、削除できません。

![](assets/no2.png)連絡先を削除できません。

### オブザーバー {#observer}

オブザーバーには次の権限があります。

![](assets/cleaner2.png)明示的に共有されている他のユーザーのプルーフを表示、レビュー、承認できます（共有フォルダー内のすべてに対する読み取り専用権限）。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) でのプルーフの役割の管理を参照してください。

![](assets/cleaner2.png)明示的に共有されているファイルを表示できます。

![](assets/cleaner2.png)連絡先とグループを表示できます。

![](assets/no2.png)プルーフの作成、ファイルのアップロード、フォルダーの作成は行うことができません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) へのファイルと web コンテンツのアップロードを参照してください。

![](assets/no2.png)組織内の他のユーザーが作成したプルーフおよびファイルは表示、編集、削除できません。

![](assets/no2.png)プルーフまたは返信は編集できません。

![](assets/no2.png)組織で作成された項目は削除できません。

![](assets/no2.png)請求ページまたはアカウント設定にはアクセスできません。詳しくは、[ [!DNL Workfront Proof]  の請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)と [ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) でのアカウント設定を参照してください。

![](assets/no2.png)ドロップゾーンの所有者として設定できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) でのドロップゾーンの設定を参照してください。

![](assets/no2.png)ごみ箱を空にすることはできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) でのごみ箱の復元と削除を参照してください。

![](assets/no2.png)ユーザーを追加、編集、削除できません。

![](assets/no2.png)グループを作成したり、新しい連絡先を追加することはできません。

![](assets/no2.png)連絡先を削除できません。

>[!NOTE]
>
>オブザーバーが使用できるメニューと機能は制限されます。
>
>* オブザーバーのダッシュボードには、ヘッダーメニューや緑色の新規メニューが表示されません。
>* オブザーバーの設定には、アカウント設定と請求のリンクは表示されません。
>

### 訪問者 {#visitor}

訪問者には次の権限があります。

![](assets/cleaner2.png)明示的に共有されている他のユーザーのプルーフを表示、レビュー、承認できます（共有フォルダー内のすべてに対する読み取り専用権限）。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) でのプルーフの役割の管理を参照してください。

![](assets/cleaner2.png)明示的に共有されているファイルを表示できます。

![](assets/no2.png)連絡先とグループは表示できません。

![](assets/no2.png)プルーフの作成、ファイルのアップロード、フォルダーの作成は行うことができません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) へのファイルと web コンテンツのアップロードを参照してください。

![](assets/no2.png)組織内の他のユーザーが作成したプルーフおよびファイルは表示、編集、削除できません。

![](assets/no2.png)プルーフまたは返信は編集できません。

![](assets/no2.png)組織で作成された項目は削除できません。

![](assets/no2.png)請求ページまたはアカウント設定にはアクセスできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) での [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)と [ アカウント設定を参照してください。

![](assets/no2.png)ドロップゾーンの所有者として設定できません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md) でのドロップゾーンの設定を参照してください。

![](assets/no2.png)ごみ箱を空にすることはできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md) でごみ箱を復元して空にするを参照してください。

![](assets/no2.png)ユーザーを追加、編集、削除できません。

![](assets/no2.png)グループを作成したり、新しい連絡先を追加することはできません。

![](assets/no2.png)連絡先を削除できません。

>[!NOTE]
>
>訪問者が利用できるメニューや機能は制限されています。
>
>* 訪問者のダッシュボードには、ヘッダーメニューや緑色の新規メニューが表示されません。
>* 訪問者の設定には、次のリンクは表示されません。アカウント設定、課金
>

### ゲスト {#guest}

ゲストプロファイルは、独自の Workfront Proof アカウントを持たないレビュアー向けに、プルーフへのアクセス権を付与するために使用されます。ゲストは、自分の個人用メール通知を通じて、自分と共有されたプルーフに直接アクセスできます。

![](assets/cleaner2.png)明示的に共有されているプルーフを表示、確認、承認できます。

![](assets/cleaner2.png)明示的に共有されているファイルを表示できます。

![](assets/no2.png)ダッシュボードにアクセスできません。

![](assets/no2.png)フォルダーを共有してもらうことはできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) でのフォルダーの管理を参照してください。

![](assets/no2.png)プルーフに作成者またはモデレーターとして追加されることはできません。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) でのプルーフの役割の管理を参照してください。

>[!NOTE]
>
>ゲストは Workfront Proof ユーザーではないので、自分のダッシュボードで共有されているすべてのプルーフを表示することはできません。

## ユーザーのプルーフ権限プロファイルの編集

管理者と請求管理者は、アカウント内のすべてのユーザーの権限プロファイルを編集できます。

1. 編集するユーザーを検索するには、次のいずれかの操作を行います。

   * **[!UICONTROL アカウント設定]**&#x200B;に移動し、「**[!UICONTROL ユーザー]**」タブをクリックします。

   * **[!UICONTROL 連絡先]**&#x200B;ページに移動します。

1. 権限を編集するユーザーの名前をクリックします。![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. **[!UICONTROL 権限プロファイル]**&#x200B;ドロップダウンメニューをクリックし、新しい権限プロファイルを選択します。

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   権限プロファイルは、管理者、スーパーバイザー、マネージャーおよびオブザーバーです。

1. メニューの外側をクリックして保存します。

>[!NOTE]
>
>管理者は請求管理者プロファイルを割り当てることができません。プロファイルの変更のリストは、次のログに記録されています。
>
>* アカウントアクティビティログ
>* ユーザーのプロファイルログ（そのユーザーのみがアクセス可能）
>

アクティビティログについて詳しくは、[ [!DNL Workfront Proof]  アクティビティ監査証跡について](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md)を参照してください。
