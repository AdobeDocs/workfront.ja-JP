---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: での電子署名について [!DNL Workfront Proof]
description: 電子署名を使用すると、配達確認のセキュリティを強化し、ISO などの業界標準に準拠できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# での電子署名について [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

電子署名を使用すると、配達確認のセキュリティを強化し、ISO などの業界標準に準拠できます。

この設定は、アカウントレベルで必須または非必須に設定できます。 デフォルトで必須の場合は、アカウントで作成されるすべての配達確認で有効になり、配達確認レベルで無効にすることはできません。 この設定がデフォルトで必須でない場合は、配達確認レベルで有効/無効を切り替えることができます。

詳しくは、を参照してください。

配達確認で電子署名設定が有効になっている場合、電子署名ボックスが表示され、配達確認に関する決定を行ったレビュー担当者に対して、電子メールとパスワードの入力を求めます。

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## 電子署名 [!UICONTROL 配達確認の詳細] ページ

レビュー担当者が、 [!UICONTROL 配達確認の詳細] (1) [!UICONTROL 電子署名] ポップアップボックスが表示され、詳細 (2) を入力し、その決定 (3) を確認するように求められます。

ポップアップにデフォルトのメッセージセット（存在する場合）が表示され、レビュー担当者は E メールとパスワードを入力する必要があります。

この [!UICONTROL 電子署名] ポップアップが校正ビューアに表示され、 [!UICONTROL 配達確認の詳細] レビュー担当者がそのレベルから決定した場合は、ページ。

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

この [!UICONTROL シングルサインオン] 「 」オプションが配達確認で有効になっている場合、E メールとパスワードの詳細は [!UICONTROL 電子署名] 決定する際にポップアップが表示されます。

代わりに、 [!UICONTROL 確認] (4) レビュー担当者は、このポップアップ上の「 [!UICONTROL シングルサインオン] ページ。

SSO 資格情報を入力すると、レビュー担当者は自動的に [!UICONTROL 配達確認の詳細] ページ ( または戻る [!UICONTROL 配達確認ビューア] もしそこから決定が下されれば )。

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> 決定が電子署名された場合、 **[!UICONTROL 署名アイコン]** (5) は、 [!UICONTROL ワークフロー] セクション [!UICONTROL 配達確認の詳細] ページ。 レビュー担当者ではなく、配達確認の編集権限を持つ他のユーザーによって決定が変更された場合、そのユーザーは決定に電子署名を求められず、決定の横に署名アイコンは表示されません (6)。

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)シングルサインオンについては、 [Workfront Proof でのシングルサインオン](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

配達確認の詳細ページについて詳しくは、 [で配達確認の詳細を管理 [!DNL Workfront] 配達確認](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
