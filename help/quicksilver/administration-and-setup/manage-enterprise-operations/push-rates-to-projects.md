---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: プロジェクトへのプッシュ率の変更
description: レートカードとは、クライアントとの契約上の契約を表します。この契約では、作業を完了する担当業務に対して時間単位のレートが定義されます。 レートカードでは、属性に基づいて、担当業務ごとに複数の請求レートを定義できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 20%

---

# プロジェクトへのプッシュ率の変更

プロジェクト <!--or a staffing plan-->にレートカードが添付されている場合でも、レートカードのレートを調整できます。 その後、レートカードが添付されているプロジェクト <!--and staffing plans -->に対して、オプションでこれらのレートをプッシュできます。 新しいレートをプッシュしない場合、元のレートはプロジェクト <!-- or staffing plan-->に残ります。

プロジェクトへのレートカードの添付について詳しくは、[ プロジェクトへのレートカードの添付](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td>ワークフロー Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL レートカード ]へのアクセスを編集</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>共有されているレートカードを編集するには、レートカードの管理権限が必要です。</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プロジェクトへのプッシュ率の変更

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. 「レート・カード」リストでレート・カード名をクリックします。
1. レート・カード/担当業務およびレート画面で、レートが正しいことを確認し、必要に応じてレートを編集します。
1. [!UICONTROL **変更をプッシュ**]&#x200B;をクリックします。
1. [!UICONTROL **すべてのプロジェクトに適用**]<!--/staffing plans--> ダイアログで、このレートカードを使用するすべてのプロジェクト <!--and staffing plans -->がデフォルトで選択されます。 プロジェクト <!--or staffing plan -->でレート変更を適用しない場合は、その選択を解除する必要があります。
1. 「[!UICONTROL **保存**]」をクリックします。

   新しいレートは、レートカードを使用するプロジェクト <!--and staffing plans -->に反映されるようになりました。
