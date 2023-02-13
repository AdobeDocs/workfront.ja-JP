---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 配達確認遅延 E メール
description: 配達確認が期限に近づいたり期限に近づいたりした場合は、配達確認遅延 E メールが受信者に送信されます。 この種の E メールは、配達確認レベルで無効にすることはできませんが、アカウントおよびユーザーの個人設定レベルで設定できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL 遅延配達確認] 電子メール

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

この [!UICONTROL 配達確認が遅れました] 配達確認が期限に近づいたり期限に近づいたりした場合に、E メールが受信者に送信されます。 この種の E メールは、配達確認レベルで無効にすることはできませんが、アカウントおよびユーザーの個人設定レベルで設定できます。

* [!UICONTROL 遅延配達確認] 配達確認の期限が切れると、すべてのレビューや決定がおこなわれていない場合、電子メールはレビュー担当者に自動的に送信されます。

   これらのメールはデフォルトで有効になっており、アカウント全体に対して調整できませんが、ユーザーが自分の校正のデフォルトで無効にすることができます。

* リスクが高い E メールは、配達確認が期限に近づくとレビュー担当者に送信されます。 これらはデフォルトで無効になっており、 [!UICONTROL アカウント設定]. 有効にした後は、 [!UICONTROL 校正の既定値].

これらの通知はカスタマイズできません。

通知を受け取る人は次のとおりです。

* 所有者 ( [!UICONTROL 電子メール] 配達確認が遅れた場合のアラート： [!UICONTROL 所有者の校正の既定値].
* まだ配達確認に対する決定を行っていない承認者。 決定について詳しくは、 [校正ビューアで配達確認を決定する](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>電子メール通知がデフォルトで [!UICONTROL アカウント設定]，いいえ [!UICONTROL 遅延配達確認] レビュー担当者や承認者がまだコメントや決定を送信していない場合でも、電子メールが送信されます。 また、 [!UICONTROL 遅延配達確認] [ 校正 ] の既定のメールアドレスです。

配達確認通知について、次の点を考慮します。

* お使いの [!DNL Workfront] 管理者または [!DNL Workfront Proof] 管理者は、電子メール通知に組織のロゴを含めることができます。詳しくは、 [ブランド化 [!DNL Workfront Proof] サイト](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* 同じレビュー担当者と複数の配達確認を共有する必要があり、複数のメールを受け取りたくない場合は、複数の配達確認を同時にアップロードできます。 すべてのレビュー担当者が、すべての配達確認の詳細と、各配達確認の個人 URL を含む 1 つの E メールを受け取ります。

   >[!NOTE]
   >
   >配達確認の作成者は、別の [!UICONTROL 作成された配達確認] 電子メールを送信します。 詳しくは、 [この [!UICONTROL 作成された配達確認] 電子メール](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* 自分または自分のレビュー担当者に、期待どおりの電子メール通知が届かない場合は、  [設定 [!DNL Workfront Proof] スパムフィルターを避けるための E メール](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
