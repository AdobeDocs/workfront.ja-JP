---
title: プロジェクトへの料金カードの添付
description: レートカードをプロジェクトに付加すると、場所別のすべての役割とそれに関連する請求率がプロジェクトに追加されます。
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# プロジェクトへの料金カードの添付

{{highlighted-preview-article-level}}

レートカードには、場所に基づいて、ジョブの役割ごとに複数の請求レートが保存されます。 それぞれ異なる請求率を持つ、パリに拠点を置く Designer と、ニューヨークに拠点を置く 2 人目の Designer という職務を持つことができます。 ただし、レートカードのジョブロールに場所は必要ありません。 レートカード上のジョブロール（場所など）の請求レートには、有効日も含まれる場合があります。

レートカードをプロジェクトに付加すると、場所別のすべての役割とそれに関連する請求率がプロジェクトに追加されます。

>[!NOTE]
>
>レートカードを添付すると、プロジェクト上の既存の請求率が上書きされます。

請求率は、プロジェクト内の料金カードから直接編集できます。 これは、デフォルトのレートカードに保存されるレートには影響しません。

レートカードの作成について詳しくは、 [レートカードの管理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

プロジェクトのジョブロール請求率の上書きおよびプロジェクト収益の計算に関する一般情報は、 [ジョブ・ロール請求率の上書きとプロジェクトの収益の計算の概要](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：標準</p><p>または</p><p>レガシープラン：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集</p> <p>ジョブロールの管理アクセス</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトへの料金カードの添付

1. プロジェクトに移動します。
1. クリック **請求率** をクリックします。 最初にクリックする必要がある場合があります **さらに表示**.
1. クリック **請求率の追加 > レートカードの添付**.

   料金カードの添付ページが開きます。 詳しくは、 [レートカードの管理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. プロジェクトに追加する料金カードを選択し、 **添付**.

   料金カードとそのすべてのジョブロールレートが請求率リストに追加されます。

   ![プロジェクトに追加されたレートカード](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >請求率リストでは、レートカードから 1 つ以上の役割を削除できます。 プロジェクトからジョブロールの請求率を削除しても、デフォルトの料金カードからは削除されません。

