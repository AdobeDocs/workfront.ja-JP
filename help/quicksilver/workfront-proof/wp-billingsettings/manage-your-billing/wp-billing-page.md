---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: この [!DNL Workfront] 配達確認の請求ページ
description: 次の手順で [!UICONTROL 請求] ページで、画面の右上にある「設定」メニューを開き、ドロップダウンメニューの「課金」を選択します。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# この [!DNL Workfront Proof] 請求ページ

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

## 請求ページ

次の手順で [!UICONTROL 請求] ページで、 **[!UICONTROL 設定]** 画面の右上にあるメニューを選択し、 **[!UICONTROL 請求]** 」と入力します。

この [!UICONTROL 請求] ページには次の情報が含まれます。

* アカウント名 (1)
* アカウントリスト（例： Satellite アカウントを持っている場合）(2)
* 変更計画 (3)
* 支払の詳細の変更 (4)
* 新しい Satellite アカウント (5)
* 口座をクローズする (6)
* 現在のプラン情報 (7)
* 請求先住所 (8)
* 使用状況の統計 (9)
* 請求履歴 (10)
* 請求活動 (11)

   ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL 現在のプラン]

このセクション (7) では、次の内容を含む現在の計画の詳細を示します。

* プランの名前
* 現在の支払い方法
* 現在のプランの開始日と終了日
* 次のプランタイプ
* 次のプランの支払い方法

   詳しくは、 [支払い方法の選択 [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL 請求先住所]

このセクション (8) では、お客様のアカウントの主な請求先と住所の詳細を示します。

請求連絡先は、お客様のアカウントで請求管理者として設定されているユーザーからのみ選択できます。 Satellite アカウントでは、このフィールドにはメインアカウントからの請求管理者のみを設定できます。

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> アカウントには複数の請求管理者を割り当てることができますが、そのうちの 1 人のみが、 [!UICONTROL 請求連絡先] フィールドには、すべての請求通知とアカウント使用状況アラートが届きます。

これには、次の通知 E メールが含まれます。

* 配達確認の使用状況
* 請求書
* ダウングレード
* 遅延支払/アカウント停止アラート
* クレジットカードエラー

   ![Billin_CC.png](assets/billin-cc-350x103.png)

この [!UICONTROL 請求 CC] 「 」フィールドを使用して、すべての請求関連 e メールにコピーする e メールアドレスを追加することもできます。 「 」フィールドをクリックして、傾斜編集を有効にし、目的の電子メールアドレスを入力します（既存のユーザーの電子メールアドレスも入力できます）。

## [!UICONTROL 請求先住所]

このセクションではインライン編集を使用するので、フィールドをクリックするだけでテキストを入力または編集できます。

>[!NOTE]
>
> この住所はサブスクリプション請求書に含めるので、このデータが常に最新の状態に保たれます。

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL 使用状況の統計]

このセクションには、次を含む、現在の請求期間内のアカウントの使用状況の統計が表示されます。

* 使用済みストレージ
* 使用した配達確認
* 使用ユーザー数制限

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL 使用状況の警告]

この [[!UICONTROL 配達確認権限プロファイル] in [!DNL Workfront] 配達確認](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) アカウントが以下の条件に達すると、お客様のアカウントに関するお客様の請求先 (1) に電子メールで通知されます。

* ストレージ容量の 75 %と 98 %
* 配達確認の 75%と 100%の制限

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

配達確認またはストレージの制限に達すると、 [!UICONTROL 請求] ページ：

* 配達確認の上限に達した場合

   ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* ストレージの上限に達した場合

![Storage_limit_reached.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>配達確認の数は、アカウントで配達確認が作成された時点で使用され、配達確認を削除して復元することはできません。

配達確認とファイルを削除し、 [!UICONTROL ごみ箱] 後で

配達確認、ストレージ、ユーザーを増やす必要がある場合は、いつでもアカウントをアップグレードできます。そしてすぐに効く

## [!UICONTROL 請求履歴]

このセクションには、最近の請求期間のアクティビティが表示されます。 また、このセクションから請求書をダウンロードすることもできます。

詳しくは、 [のダウンロード [!DNL Workfront Proof] 請求書](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL 請求アクティビティ]

このセクションには、購読、アップグレード、ダウングレード、更新など、請求設定に対する最近の変更が表示されます [!DNL Workfront Proof] 計画

プランをユーザー数の少ないプラン (1) に変更すると、新しいプランの開始時に、新しい制限を超えるユーザーが自動的に無効化されます。 このアクティビティは、アカウントログにもキャプチャされます (2)。

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
