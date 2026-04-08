---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: AI共同作業者の設定
description: Adobe Workfront管理者は、AI共同作業者を設定し、プロジェクトやタスクに割り当てることができます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25d5fef46bc8f02e92d778685c2ad6e93439f9ff
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 8%

---

# AI共同作業者の設定

{{highlighted-preview-article-level}}

AI協力者とは、AI エージェントをプロジェクトやタスクに組み込む手法のひとつです。 AI共同作業者を設定し、ユーザーと同じように割り当てることができます。

例えば、ブランドガイドラインを使用してレビューアータイプのAI コラボレーターを設定し、そのコラボレーターにドキュメントのレビューを割り当てることができます。

利用可能なAI共同作業者タイプは次のとおりです。

* レビュアー：ブランド <!-- or Adobe Brand Intelligence-->を使用して共同作業者を作成し、その共同作業者をアセットのレビュアーとして割り当てます。

  詳しくは、[Workfront Content Reviewerの基本を学ぶ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)を参照してください。

  >[!NOTE]
  >
  >現在、レビュアーは利用可能なAI コラボレーターの種類として唯一です。 AI Collaboratorの機能は、今後さらに追加される予定です。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>Standard、Prime、またはUltimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件



* 署名済みのAdobe Gen AI契約書がファイルに登録されている必要があります。

  詳しくは、「[Adobe生成AI契約書に署名する](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)」を参照してください。WorkfrontのAI アシスタントの記事を参照してください。
* レビューアータイプのAI コラボレーターに使用するには、Workfrontでブランドを設定しておく必要があります。

  手順については、[ コンテンツレビュアーのブランドの作成と管理](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)を参照してください。

## レビュー担当者タイプのAI コラボレーターを新規作成する

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. 画面の右上隅にある「**新しい共同作業者**」をクリックします。
1. **Reviewer**&#x200B;をクリックしてから、**Continue**&#x200B;をクリックします。

   >[!NOTE]
   >
   >現在、レビューアータイプのみが使用できます。 将来的には、より多くのAI コラボレーターのタイプが利用可能になる予定です。

1. 「共同作業者の名前」フィールドに、共同作業者の名前を入力します。 これは、タスクで使用可能な担当者のリストに表示される名前です。
   <!--1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.-->
   <!--1. (Conditional) If the AI Collaborator will use Adobe Brand Intelligence, select the tenant that it will use.-->
1. <!--(Conditional) If the AI Collaborator will use a Brand,-->使用するブランドとブランドのガイドラインを選択します。
1. 「**保存**」をクリックします。

## AI共同作業者の管理

既存のAI共同作業者を編集、コピー、削除できます。

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. （条件付き）共同作業者を編集するには、編集する共同作業者の名前をクリックし、「共同作業者を編集」ウィンドウで編集を行い、**保存**&#x200B;をクリックします。
1. （条件付き）共同作業者をコピーするには、コピーするAI共同作業者の行にあるコピーアイコン ![ コピーアイコン ](assets/copy-ai-collaborator.png)をクリックし、コピーの名前をクリックして、共同作業者を編集ウィンドウで編集し、**保存**&#x200B;をクリックします。
1. （条件付き）共同作業者を削除するには、削除するAI共同作業者の行にある削除アイコン ![削除アイコン ](assets/delete-collaborator-icon.png)をクリックし、**削除**&#x200B;をクリックします。
