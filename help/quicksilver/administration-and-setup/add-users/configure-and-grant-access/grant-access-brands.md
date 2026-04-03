---
title: ブランド権限へのアクセス権の付与
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Adobe Workfront管理者は、Admin Consoleでユーザーグループを作成し、GenStudio System Manager製品プロファイルを割り当てることで、ブランドの権限を設定できます。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: ebc342b65bee6a8c5ba0edbe2e990ec2775a9055
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 9%

---

# ブランド権限へのアクセス権の付与

{{highlighted-preview-article-level}}

ユーザーは、ユーザーグループに追加されると、Adobe GenStudio システムマネージャーのブランドの作成、編集、公開権限を付与されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console権限</td> 
   <td> <p>Adobe Admin Consoleのシステム管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 要件

* Workfront インスタンスでは、統合承認が有効になっている必要があります。

* 組織にはGenStudio Foundationが必要です。
   * WorkfrontのContent Reviewerには、GenStudio Foundationでアセットのレビューおよび承認ワークフローに使用できる機能が用意されています。 作業を完了するためにGenStudio Foundationに直接アクセスする必要はありません。 Content Reviewerを介したGenStudio Foundation機能へのアクセスは、Workfront契約の条件に該当します。
* Adobeには、署名済みのAdobe Gen AI契約書がファイルに登録されている必要があります。
契約書への署名について詳しくは、[Adobe Gen AI契約書への署名](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)を参照してください。

## &#x200B;1. Admin Consoleでのブランド権限の設定

### 手順1：ユーザーグループの作成

Admin Consoleで新しいユーザーグループを作成し、ブランドの作成と編集に関する権限を管理します。

### 手順2：製品プロファイルのユーザーグループへの割り当て

割り当てられたプロファイルに関連付けられた権限は、このグループのすべてのユーザーにGenStudio Brands権限（ブランドの作成、更新、削除）を与えます。

プロファイルを割り当てるには：

1. 新しく作成したユーザーグループに移動します。
1. 「**割り当て済み製品プロファイル**」タブをクリックします。
1. 「**プロファイルを割り当て**」をクリックします。
1. ポップアップで、商品リストから&#x200B;**Adobe GenStudio**&#x200B;を選択し、**適用**&#x200B;をクリックします。
1. **Adobe GenStudio system manager** プロファイルを選択します。
1. 「**適用**」をクリックします。
1. 「**保存**」をクリックします。

### 手順3：ユーザーグループにユーザーを追加する

ブランドの作成、編集、公開にユーザー権限を割り当てるには、ユーザーをユーザーグループに追加します。

>[!NOTE]
>
>手順4の説明に従って、グループをプロジェクトに追加する前に、少なくとも1人のユーザーを追加する必要があります。

ユーザーを追加するには：

1. **Admin Console** > **ユーザー** > **ユーザーグループ**&#x200B;に移動します。
1. ユーザーグループを選択します。
1. ユーザー名またはメールアドレスでユーザーを追加します。
1. 既存のユーザーに対して提案された一致から選択します。

### ステップ 4：ブランドプロジェクトの作成

プロジェクトでは、ユーザーがブランドアセットを保存できる保存場所を提供します。

プロジェクトを作成するには：

1. Admin Consoleの「**ストレージ**」タブに移動します。
1. 「**プロジェクト**」をクリックします。
1. 「**プロジェクトを作成**」をクリックします。
1. ポップアップに、プロジェクト名を入力します：**Adobe GenStudio Brands**。

   >[!IMPORTANT]
   >
   >プロジェクト名を正確に入力します。 余分なスペースを追加したり、ケースを変更したりしないでください。

1. 「**作成**」をクリックします。

### 手順5：ユーザーグループをプロジェクトに招待する

Brands プロジェクトにユーザーグループを追加し、アセットにアクセスして管理できるようにします。

1. **プロジェクトに招待** ポップアップで、作成したユーザーグループを追加します。
1. 「**権限を編集できます**」を選択します。
1. 「**招待**」をクリックします。

### 結果

グループ内のユーザーには、Workfront内でブランドアセットを作成、編集、公開する権限が付与されました。

## &#x200B;2. Workfrontのアクセスレベルでのブランドへのアクセス権の付与

Workfrontのアクセスレベルで個々のユーザーにブランドへのアクセス権を付与する前に、前の節のすべての手順を完了する必要があります。

>[!IMPORTANT]
>
>* Admin ConsoleのGenStudio system manager製品プロファイルを持つユーザーグループに割り当てられたユーザーのみが、他のユーザーがアクセスレベル設定でブランドにアクセスできる場合でも、Workfrontでブランドを作成、編集、公開できます。
>* ブランドへのアクセスが有効になっているアクセスレベルに追加されたが、Admin Consoleのユーザーグループに追加されていないユーザーは、ブランドのみを表示できます。


Workfrontのアクセスレベルでブランドにアクセス権を付与するには：

{{step-1-to-setup}}

1. 左側のパネルで「**アクセスレベル**」をクリックします。
1. 編集するアクセスレベルを見つけ、編集アイコン ![編集アイコン &#x200B;](assets/edit-icon.png)をクリックして編集します。

   または

   「**新しいアクセスレベル**」をクリックして、新しいアクセスレベルを作成します。 アクセス レベルの作成について詳しくは、[&#x200B; カスタム アクセス レベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
1. **追加の制限を設定**&#x200B;まで下にスクロールし、**ユーザーがブランドにアクセスすることを許可**&#x200B;を選択します。
   ![&#x200B; ブランド設定へのアクセスを許可](assets/access-for-brands.png)
1. 「**保存**」をクリックします。

ブランドを設定したら、コンテンツレビュー担当者を作成して、レビューと承認のワークフローでアセットをブランドガイドラインに照らし合わせてレビューできます。 詳しくは、[AI コラボレーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)を参照してください。