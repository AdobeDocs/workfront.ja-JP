---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: での配達確認の役割の管理 [!DNL Workfront Proof]
description: 配達確認の役割を使用すると、ユーザープロファイルに設定された権限プロファイルで制限されるユーザーに権限を付与できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# での配達確認の役割の管理 [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

配達確認の役割を使用すると、ユーザープロファイルに設定された権限プロファイルで制限されるユーザーに権限を付与できます。 ( 権限プロファイルについて詳しくは、 [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

配達確認の役割は、アカウントプロファイルとは異なります。 アカウントプロファイルは、アカウント内の全体的な権限レベルに関連しており、明示的に共有されていない配達確認でも、アカウント内のすべての配達確認に対する権限に影響を与えます。

詳しくは、 [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 配達確認の役割について

次の配達確認の役割は、ユーザーが配達確認のレビューに招待されたときに、個々の配達確認のユーザーに付与されます。

* [読み取り専用](#read-only)
* [レビュアー](#reviewer)
* [承認者](#approver)
* [レビュアーと承認者](#reviewer-approver)
* [作者](#author)
* [モデレーター](#moderator)

配達確認の役割は、特定の配達確認に関してレビュー担当者が実行できるアクションを定義します。

例えば、レビュー担当者の場合は、マークアップとコメントを追加して、配達確認を確認するように求められます。 レビュー担当者および承認者の場合は、配達確認を確認し、決定する必要があります。

特定の配達確認の役割は、レビュー担当者に対して（アカウントプロファイルがない場合でも）編集権限を付与し、コメントに対するアクションの追加、新しいバージョンの作成、配達確認へのレビュー担当者の追加などの追加機能を使用できます。

詳しくは、次の記事を参照してください。

* [配達確認コメントに対するアクションの使用](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [での配達確認の共有 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### 読み取り専用

{#read-only}

![cleaner.png](assets/cleaner.png) 配達確認を表示できます

![no.png](assets/no.png) マークアップを追加できません

![no.png](assets/no.png) コメントを追加できません

![no.png](assets/no.png) 決定できません

![no.png](assets/no.png) 他のユーザーが作成したコメントは削除できません

![no.png](assets/no.png) 配達確認の編集権限がありません

>[!NOTE]
>
>フォルダーが [!DNL Workfront Proof]に含まれない場合は、自動的にすべての既存の項目に対して読み取り専用権限が付与され、その後フォルダーに追加される項目も自動的に付与されます。

詳しくは、 [でフォルダーを共有 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### レビュアー {#reviewer}

![cleaner.png](assets/cleaner.png) 配達確認を表示できます

![cleaner.png](assets/cleaner.png) マークアップを追加できます

![cleaner.png](assets/cleaner.png) コメントを追加できます

![[!DNL cleaner].png](assets/cleaner.png) 返信がない場合は、自分のコメントを編集できます

![no.png](assets/no.png) 決定できません

![no.png](assets/no.png) 他のユーザーが作成したコメントを編集または削除することはできません

![no.png](assets/no.png) 配達確認の編集権限がありません

### 承認者 {#approver}

![cleaner.png](assets/cleaner.png) 配達確認を表示できます

![cleaner.png](assets/cleaner.png) 決定を下すことができます

![no.png](assets/no.png) マークアップを追加できません

![no.png](assets/no.png) コメントを追加できません

![no.png](assets/no.png) 他のユーザーが作成したコメントを編集または削除することはできません

![no.png](assets/no.png) 配達確認の編集権限がありません

### レビュアーと承認者 {#reviewer-approver}

![cleaner.png](assets/cleaner.png) 配達確認を表示できます

![cleaner.png](assets/cleaner.png) マークアップを追加できます

![cleaner.png](assets/cleaner.png) コメントを追加できます

![[!DNL cleaner].png](assets/cleaner.png) 返信がない場合は、自分のコメントを編集できます

![cleaner.png](assets/cleaner.png) 決定を下すことができます

![no.png](assets/no.png) 他のユーザーが作成したコメントを編集または削除することはできません

![no.png](assets/no.png) 配達確認の編集権限がありません

### 作者 {#author}

![cleaner.png](assets/cleaner.png) マークアップを追加できます

![cleaner.png](assets/cleaner.png) コメントを追加できます

![[!DNL cleaner].png](assets/cleaner.png) 返信がない場合は、自分のコメントを編集できます

![cleaner.png](assets/cleaner.png) 決定を下すことができます

![cleaner.png](assets/cleaner.png) 新しいバージョンを送信できます

![cleaner.png](assets/cleaner.png) 配達確認のコピーを作成できます

![cleaner.png](assets/cleaner.png) 他のユーザーと配達確認を共有できます

![cleaner.png](assets/cleaner.png) コメントにアクションを適用できます

![cleaner.png](assets/cleaner.png) コメントを解決できます

![no.png](assets/no.png) 他のユーザーが作成したコメントを編集または削除することはできません

>[!NOTE]
>
>この役割は、 [!DNL Workfront Proof].

### モデレーター {#moderator}

![cleaner.png](assets/cleaner.png) マークアップを追加できます

![cleaner.png](assets/cleaner.png) コメントを追加できます

![[!DNL cleaner].png](assets/cleaner.png) 返信がない場合は、自分のコメントを編集できます

![cleaner.png](assets/cleaner.png) 決定を下すことができます

![cleaner.png](assets/cleaner.png) 新しいバージョンを送信できます

![cleaner.png](assets/cleaner.png) 新しいレビュー担当者を追加できます

![cleaner.png](assets/cleaner.png) コメントにアクションを適用できます

![cleaner.png](assets/cleaner.png) コメントを解決できます

![cleaner.png](assets/cleaner.png) 配達確認に対するコメントや返信（自分自身または他のユーザーが作成）を削除できます

* コメントスレッド内の最初のコメントを削除すると、スレッド全体が削除されます
* コメントスレッドで返信を削除すると、その返信のみが削除されます

![no.png](assets/no.png) 他のユーザーが作成したコメントは編集できません

この役割を使用すると、配達確認のコメントを管理およびモデレートでき、配達確認に関連するコメントのみを保持し、関連しないコメントを削除できます。

>[!NOTE]
>
>この役割は、 [!DNL Workfront Proof].

## 配達確認の役割の割り当て

配達確認の役割は、新しい配達確認の作成時、既存の配達確認の新しいバージョンの作成時または既存の配達確認の既存の配達確認の作成時に割り当てることができます。

### 新しい配達確認 {#new-proofs}

配達確認の役割は、 [!UICONTROL 新しい配達確認] 配達確認の作成プロセス中のページ (1)

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### 新しいバージョン {#new-versions}

配達確認の新しいバージョンを作成すると、以前のバージョンのレビュー担当者が自動的に表示されます（以前のバージョンと同じ役割を持ちます）。

新しいバージョンの作成時にレビュー担当者に適用された配達確認の役割を編集できます (1)。

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### 既存の配達確認 {#existing-proofs}

既存の配達確認に関する個人の役割を変更する場合は、 [!UICONTROL 配達確認の詳細] ページを作成するには、ワークフローの節 (1) での役割をインライン編集します。

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## 配達確認ビューアでの役割の確認

レビュー担当者の役割は、配達確認ビューア (1) から直接確認し、必要に応じて編集できます (2)。

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## デフォルトの配達確認の役割

デフォルトの配達確認の役割は、 [!DNL Proofing Defaults] 」ページを個人設定に追加します。 つまり、配達確認に追加されると、デフォルトの配達確認の役割が自動的に設定されます。 この役割は、配達確認に対する編集権限を持つユーザーが配達確認レベルで変更できます。

>[!NOTE]
>
>管理者または請求管理者のプロファイルを持つユーザーのみが、自分のアカウント内の他のユーザーの校正のデフォルトを変更できます。

詳しくは、 [の個人設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## 作成者と所有者

作成者と所有者には、配達確認に対する完全な編集権限があります。

### 作成者 {#creators}

配達確認の作成者は、最初のインスタンスで配達確認をアップロードする人です。 配達確認の作成者は、配達確認のユーザーリスト（デフォルトの役割）に自動的に表示されます。

次の日： [!UICONTROL 新しい配達確認] ページを使用して、配達確認作成者に別の配達確認の役割を割り当てることができます（デフォルトの役割を除く）。

配達確認の作成者は、配達確認から変更または削除できません。

### 所有者 {#owners}

デフォルトでは、「作成者」も配達確認の所有者です。ただし、「作成者」は、( [!UICONTROL 新しい配達確認] ページ ) を参照してください。

新しい配達確認ページで所有者を変更するには：

1. 作成者名の横に表示される変更リンクをクリックします。
1. ドロップダウンメニューから新しい所有者を選択します。 (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

配達確認を作成した後でも、所有者を変更できます。 配達確認の編集権限を持つユーザーは誰でも、 [!UICONTROL 配達確認の詳細] ページを参照してください。

配達確認の所有者を変更する機能は、ワークフロー管理の観点から特に役立ちます。 これにより、プロジェクトの担当者が配達確認の所有権を引き継ぎ、配達確認の編集権限と、配達確認を [!UICONTROL 配達確認] 表示。

次を使用して配達確認の所有者を変更するには [!UICONTROL 配達確認の詳細] ページ：

* 所有者にする人の名前の横にある「アクション」メニューをクリックします。
* 選択 [!UICONTROL **所有者を作成**] を選択します。
* または、 [!UICONTROL **所有者**] 配達確認画像の横にある「 」フィールドを選択し、表示されるドロップダウンから新しい所有者を選択します。

これが完了すると、その人の名前の横に「所有者」という単語が表示されます。

>[!NOTE]
>
>配達確認の所有者にできるのは、同じアカウントまたはパートナーアカウントのユーザーのみです。 次の場合にのみ、パートナーアカウントのユーザーに配達確認の所有者を設定できます。
>
>* アカウント間に既存のパートナー関係が設定されています。 詳しくは、 [のパートナーアカウント [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* にカスタムフィールドがありません [!UICONTROL 新しい配達確認] ページに貼り付けます。
>* 配達確認はフォルダーに割り当てられていません。
>* 配達確認にタグが適用されていません。

内で配達確認の所有権を一時的に委任するには [!DNL Workfront Proof]を参照してください。 [での一時配達確認所有者の指定 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
