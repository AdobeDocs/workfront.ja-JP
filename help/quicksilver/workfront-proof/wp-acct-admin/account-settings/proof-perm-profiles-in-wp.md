---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Workfront Proof の配達確認権限プロファイル
description: Workfront管理者またはWorkfront配達確認管理者は、配達確認権限プロファイルをユーザーに割り当てて、システム内のすべての配達確認に対してユーザーが持つ検証機能を指定できます。 ユーザーの配達確認権限プロファイルの設定について詳しくは、 Workfront Proof でのユーザーの配達確認権限プロファイルの設定を参照してください。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 1%

---

# の配達確認権限プロファイル [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

As a [!DNL Workfront] 管理者または [!DNL Workfront Proof] 管理者は、配達確認権限プロファイルをユーザーに割り当てて、システム内のすべての配達確認に対してユーザーが持つ検証機能を指定できます。 ユーザーの配達確認権限プロファイルの設定について詳しくは、 [でのユーザーの配達確認権限プロファイルの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>次の操作も実行できます。
>
>* 個々の配達確認に対する特定の役割をユーザーに付与する。 配達確認の役割について詳しくは、 [での配達確認の役割の管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* 組織内のユーザーのカスタムプロファイルを作成します。 詳しくは、 [でのカスタムプロファイルの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


次の表に、各配達確認権限プロファイルで使用できる権限を示します。

| **独自の項目** |  |  |  |  | **他のユーザーの項目** |  |  | **管理** | **請求** |
|---|---|---|---|---|---|---|---|---|---|
|  | **追加** | **ビュー** | **編集** | **削除** | **ビュー** | **編集** | **削除** | **編集と削除** | **編集** |
| 請求管理者 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| 管理 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| スーパーバイザ－ | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| マネージャー | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| オブザーバー |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| 訪問者 |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

役割と権限について、次の点を考慮します。

* 割り当てられたプロファイル権限は、自分のアカウントのユーザーと項目にのみ関係します。 ただし、Satellite アカウントの場合は例外です。メイン（ハブ）アカウントの管理者と請求管理者は、ハブアカウントレベルからアカウント設定と請求にアクセスし、管理できます。
* 請求管理者および管理者は、ユーザーを削除できます。 これは、アカウント設定でのみ実行できます。
* 請求管理者および管理者が、自分のアカウント内の他のユーザーが所有する配達確認を表示する場合、レビュー担当者の役割を持つ配達確認を表示します。
* 請求管理者と管理者は、読み取り専用の役割を使用して、自分と共有されたフォルダまたは自分が作成したフォルダ内の配達確認にアクセスできます。

次の節では、標準のプロファイルに関連付けられている各プロファイルと権限について説明します [!DNL Workfront Proof] 設定：

* [請求管理者](#billing-administrator)
* [管理者](#administrator)
* [スーパーバイザ－](#supervisor)
* [マネージャー](#manager)
* [オブザーバー](#observer)
* [訪問者](#visitor)
* [ゲスト](#guest)

## 請求管理者 {#billing-administrator}

請求管理者は、 [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)、および次の権限を持っています。

![](assets/cleaner2.png)配達確認の生成、ファイルのアップロード、フォルダーの作成が可能です。 詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [ファイルと Web コンテンツのアップロード先 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)、および [でのフォルダーの作成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)独自に作成した配達確認およびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)組織内のすべてのユーザーが作成した配達確認およびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)他のユーザーの公開フォルダーを削除できます。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)アカウントで作成されたすべての配達確認に対する編集権限を持ちます。

![](assets/cleaner2.png)ドロップゾーンの所有者として設定できます。 詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)請求ページにアクセスし、請求の詳細を編集できます。 詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)アカウント設定ページにアクセスし、アカウントの詳細を編集できます。 詳しくは、 [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)ごみ箱を空にできます。 詳しくは、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)ユーザーを追加、編集および削除できます。

![](assets/cleaner2.png)グループを作成し、新しい連絡先を追加できます。

![](assets/cleaner2.png)連絡先を削除できます。

![](assets/cleaner2.png)返信がない場合に配達確認を編集できます。

![](assets/no2.png)配達確認の返信を編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダを削除できません。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

アカウントの設定について詳しくは、 [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

請求について詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### 管理者 {#administrator}

管理者は、 [アカウント設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)およびには次の権限があります。

![](assets/cleaner2.png)配達確認の作成、ファイルのアップロードおよびフォルダーの作成が可能です。 詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [ファイルと Web コンテンツのアップロード先 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)、および [でのフォルダーの作成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)作成した配達確認やファイルを表示、編集および削除できます。

![](assets/cleaner2.png)組織内のすべてのユーザーが作成した配達確認およびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)他のユーザーの公開フォルダーを削除できます。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)アカウントで作成されたすべての配達確認に対する編集権限を持ちます。

![](assets/cleaner2.png)ドロップゾーンの所有者として設定できます。 詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)アカウント設定ページにアクセスし、アカウントの詳細を編集できます。 詳しくは、 [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)ごみ箱を空にできます。 詳しくは、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)ユーザーを追加、編集および削除できます。

![](assets/cleaner2.png)グループを作成し、新しい連絡先を追加できます。

![](assets/cleaner2.png)連絡先を削除できます。

![](assets/cleaner2.png)返信がない場合に配達確認を編集できます。

![](assets/no2.png)配達確認の返信を編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダを削除できません。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)請求ページにアクセスしたり、請求の詳細を編集したりできません。 詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### スーパーバイザ－ {#supervisor}

スーパーバイザーには、次の権限があります。

![](assets/cleaner2.png)配達確認の作成、ファイルのアップロードおよびフォルダーの作成が可能です。 詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [ファイルと Web コンテンツのアップロード先 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)、および [でのフォルダーの作成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)作成した独自の配達確認およびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)組織内のすべてのユーザーが作成した配達確認およびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)他のユーザーの公開フォルダーを削除できます。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)アカウントで作成されたすべての配達確認に対する編集権限を持ちます。

![](assets/cleaner2.png)ドロップゾーンの所有者として設定できます。 詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)グループを作成し、新しい連絡先を追加できます。

![](assets/cleaner2.png)連絡先を削除できます。

![](assets/cleaner2.png)返信がない場合に配達確認を編集できます。

![](assets/no2.png)配達確認の返信を編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダを削除できません。 詳しくは、 [内のフォルダー [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)請求ページまたはアカウント設定にアクセスできません。 詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) および [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)ユーザーを追加、編集、または削除できません。

![](assets/no2.png)ごみ箱を空にすることはできません。 詳しくは、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### マネージャー {#manager}

マネージャーには次の権限があります。

![](assets/cleaner2.png)配達確認の作成、ファイルのアップロードおよびフォルダーの作成が可能です。 詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [ファイルと Web コンテンツのアップロード先 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)、および [でのフォルダーの作成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)独自に作成または所有する配達確認およびファイルを表示、編集および削除できます。

![](assets/cleaner2.png)明示的に共有されている他のユーザーの配達確認を、表示、確認および承認できます（共有フォルダー内のすべてのユーザーに対する読み取り専用権限）。 詳しくは、 [での配達確認の役割の管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)グループを作成し、新しい連絡先を追加できます。

![](assets/no2.png)組織内の他のユーザーが作成した配達確認やファイルを表示、編集または削除することはできません。

![](assets/no2.png)配達確認または返信を編集できません。

![](assets/no2.png)他のユーザーのプライベートフォルダを削除できません。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)他のユーザーのパブリックフォルダを削除できません。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)請求ページまたはアカウント設定にアクセスできません。 詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) および [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)ドロップゾーンの所有者として設定できません。 詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)ごみ箱を空にすることはできません。 詳しくは、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)ユーザーを追加、編集、または削除できません。

![](assets/no2.png)連絡先を削除できません。

### オブザーバー {#observer}

監視者には次の権限があります。

![](assets/cleaner2.png)明示的に共有されている他のユーザーの配達確認を、表示、確認および承認できます（共有フォルダー内のすべてのユーザーに対する読み取り専用権限）。 詳しくは、 [での配達確認の役割の管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)明示的に共有されているファイルを表示できます。

![](assets/cleaner2.png) 連絡先とグループを表示できます

![](assets/no2.png)配達確認の作成、ファイルのアップロード、フォルダーの作成はできません。 詳しくは、 [ファイルと Web コンテンツのアップロード先 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)組織内の他のユーザーが作成した配達確認やファイルを表示、編集または削除することはできません。

![](assets/no2.png)配達確認または返信を編集できません。

![](assets/no2.png)組織で作成された項目は削除できません。

![](assets/no2.png)請求ページまたはアカウント設定にアクセスできません。 詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) および [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)ドロップゾーンの所有者として設定できません。 詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)ごみ箱を空にすることはできません。 詳しくは、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)ユーザーを追加、編集、または削除できません。

![](assets/no2.png)グループを作成したり、新しい連絡先を追加することはできません。

![](assets/no2.png)連絡先を削除できません。

>[!NOTE]
>
>Observers が使用できるメニューと機能は制限されます。
>
>* 監視者のダッシュボードに、ヘッダーメニューや緑色の新規メニューが表示されない
>* 監視者の設定には、次のリンクは表示されません。アカウント設定、課金
>


### 訪問者 {#visitor}

訪問者には次の権限があります。

![](assets/cleaner2.png)明示的に共有されている他のユーザーの配達確認を、表示、確認および承認できます（共有フォルダー内のすべてのユーザーに対する読み取り専用権限）。 詳しくは、 [での配達確認の役割の管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)明示的に共有されているファイルを表示できます。

![](assets/no2.png) 連絡先とグループを表示できません

![](assets/no2.png)配達確認の作成、ファイルのアップロード、フォルダーの作成はできません。 詳しくは、 [ファイルと Web コンテンツのアップロード先 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)組織内の他のユーザーが作成した配達確認やファイルを表示、編集または削除することはできません。

![](assets/no2.png)配達確認または返信を編集できません。

![](assets/no2.png)組織で作成された項目は削除できません。

![](assets/no2.png)請求ページまたはアカウント設定にアクセスできません。 詳しくは、 [この [!DNL Workfront Proof] 請求ページ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) および [のアカウント設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)ドロップゾーンの所有者として設定できません。 詳しくは、 [でのドロップゾーンの設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)ごみ箱を空にすることはできません。 詳しくは、 [でごみ箱を復元して空にする [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)ユーザーを追加、編集、または削除できません。

![](assets/no2.png)グループを作成したり、新しい連絡先を追加することはできません。

![](assets/no2.png)連絡先を削除できません。

>[!NOTE]
>
>訪問者が利用できるメニューや機能は制限されています。
>
>* 訪問者のダッシュボードにヘッダーメニューや緑の新規メニューが表示されない
>* 訪問者の設定には次のリンクは表示されません。アカウント設定、課金
>


### ゲスト {#guest}

ゲストプロファイルは、独自のWorkfront Proof アカウントを持たないレビュー担当者向けに、配達確認へのアクセス権を付与するために使用されます。 ゲストは、自分の個人用電子メール通知を通じて、自分と共有した配達確認に直接アクセスできます。

![](assets/cleaner2.png)明示的に共有されている配達確認を表示、確認および承認できます。

![](assets/cleaner2.png)明示的に共有されているファイルを表示できます。

![](assets/no2.png)ダッシュボードにアクセスできません。

![](assets/no2.png)フォルダを共有することはできません。 詳しくは、 [でのフォルダーの管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)配達確認には、作成者またはモデレーターとして追加できません。 詳しくは、 [での配達確認の役割の管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>ゲストはWorkfront Proof ユーザーではないので、自分のダッシュボードで共有されているすべての配達確認を表示することはできません。

## ユーザーの配達確認権限プロファイルの編集

管理者と請求管理者は、アカウント内のすべてのユーザーの権限プロファイルを編集できます。

1. 編集するユーザーを検索するには、次のいずれかの操作を行います。

   * に移動します。 **[!UICONTROL アカウント設定]**」、「 **[!UICONTROL ユーザー]** タブをクリックします。

   * 次に移動： **[!UICONTROL 連絡先]** ページ。

1. 権限を編集するユーザーの名前をクリックします。 ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. 次をクリック： **[!UICONTROL 権限プロファイル]** ドロップダウンメニューから、新しい権限プロファイルを選択します。:

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   権限プロファイルは、管理者、スーパーバイザー、マネージャー、監視者です。

1. メニューの外側の任意の場所をクリックして保存します。

>[!NOTE]
>
>管理者は請求管理者プロファイルを割り当てることができません。 プロファイルの変更のリストは、次のログに記録されています。
>
>* アカウントアクティビティログ
>* ユーザーのプロファイルログ（そのユーザーのみがアクセス可能）
>


アクティビティログについて詳しくは、 [について [!DNL Workfront Proof] アクティビティ監査証跡](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
