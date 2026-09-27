---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 遅延プルーフメール
description: 遅延プルーフメールは、プルーフが期限に近づいたり期限に達したり場合に受信者に送信されます。 このタイプのメールは、プルーフレベルで無効にすることはできませんが、アカウントおよびユーザーの個人設定レベルで設定できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
TQID: 'https://experienceleague.adobe.com/7mN20lz57PSto-MAK1EqBg19RdMwIjnEUnzEIEpNxvU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 100%
---
# [!UICONTROL プルーフ遅延]メール

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。 [!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

[!UICONTROL プルーフ遅延]メールは、プルーフが期限に近づいたり期限に達したり場合に受信者に送信されます。 このタイプのメールは、プルーフレベルで無効にすることはできませんが、アカウントおよびユーザーの個人設定レベルで設定できます。

* [!UICONTROL プルーフ遅延]メールは、プルーフが期日に達したにもかかわらず、レビューや決定がすべて完了していない場合に、レビュアーに自動的に送信されます。

  これらのメールはデフォルトで有効になっており、アカウント全体に対して調整できませんが、ユーザーが自分のプルーフのデフォルトで無効にすることができます。

* 「危険あり」メールは、プルーフが期限に近づくとレビュアーに送信されます。 これらはデフォルトで無効になっており、[!UICONTROL アカウント設定]で有効にすることができます。 有効にした後は、「[!UICONTROL プルーフのデフォルト]」で調整することもできます。

これらの通知はカスタマイズできません。

通知は次のメンバーに送信されます。

* 所有者（[!UICONTROL 所有者のプルーフデフォルト]でプルーフが遅れた場合の[!UICONTROL メール]アラートが有効になっている場合のみ）
* まだプルーフに対する決定を行っていない承認者。 決定について詳しくは、[プルーフビューアーでプルーフに関する決定を行う](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を参照してください。

>[!NOTE]
>
>メール通知が[!UICONTROL アカウント設定]でデフォルトで無効になっている場合、レビュアーや承認者がまだコメントや決定を送信していない場合でも、[!UICONTROL プルーフ遅延]メールは送信されません。 また、プルーフデフォルトで[!UICONTROL 遅延プルーフ]を無効にすることもできます。

プルーフ通知について、次の点を考慮してください。

* [!DNL Workfront] 管理者または [!DNL Workfront Proof] 管理者は、メール通知に組織のロゴを含めることができます。詳しくは、[ [!DNL Workfront Proof] サイトのブランド化](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)を参照してください。
* 同じレビュアーと複数のプルーフを共有する必要があるけれど、複数のメールを送りたくない場合は、複数のプルーフを同時にアップロードできます。 レビュアーは全員、すべてのプルーフの詳細と、各プルーフの個人 URL が含まれた 1 件のメールを受け取ります。

  >[!NOTE]
  >
  >プルーフの作成者は、作成したプルーフごとに別の[!UICONTROL プルーフ作成]メールを受信します。 詳しくは、[[!UICONTROL プルーフ作成]メール](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)を参照してください。

* 自分または自分のレビュアーに期待どおりのメール通知が届かない場合は、[スパムフィルターを回避するための [!DNL Workfront Proof] メール設定](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md)を参照してください。

