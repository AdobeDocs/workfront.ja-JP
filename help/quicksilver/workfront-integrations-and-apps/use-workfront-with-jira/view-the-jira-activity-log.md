---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira のアクティビティログの表示
description: ' [!DNL Jira]  管理者は、  [!DNL Adobe Workfront]  と  [!DNL Jira]  の間の同期中またはチケットの作成中に発生した例外やエラーをアクティビティログで参照できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: ht
source-wordcount: '308'
ht-degree: 100%

---

# [!UICONTROL [!DNL Jira]アクティビティログ]の表示

[!DNL Jira] 管理者は、[!DNL Adobe Workfront] と [!DNL Jira] の間の同期中またはチケットの作成中に発生した例外やエラーを[!UICONTROL アクティビティログ]で参照できます。

アクティビティログには、最大 500 個の項目が新しい順に表示されます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] プラン</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：ユーザーが属する既存のユーザーアカウントを使用するのではなく、この統合専用に [!DNL Jira] と [!DNL Workfront] で個別のシステム管理者アカウントを作成することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!DNL Workfront] 管理者であることが必要です。[!DNL Workfront] 管理者について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> <p>注：アクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されていないか確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権については、[!DNL Workfront] 管理者にお問い合わせのうえご確認ください。

## 前提条件

[!DNL Workfront] と [!DNL Jira] 間の項目をリンクするには、まず以下が必要です

* [!DNL Workfront for Jira] をインストールする

  [!DNL Workfront for Jira] をインストールする手順については、[インストール [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)を参照してください。

## [!UICONTROL [!DNL Jira]アクティビティログ]にアクセスする

1. システム管理者として Jira にログインします。
1. [!DNL Jira] のメインメニューで「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL アドオン]**」をクリックしてから「**[!UICONTROL アドオンを管理]**」をクリックします。

1. **[!DNL Workfront]** アドオンを展開します。
1. 「**[!UICONTROL 設定]**」をクリックします。
1. システム管理者として [!DNL Workfront] にログインします。
1. 「**[!UICONTROL アクティビティログ]**」タブを選択します。

   アイテムの作成中、または 2 つのアプリケーションのフィールドの同期中に発生した例外およびエラーに関する情報が表示されます。

   ログには、次のフィールドが含まれます。

   * 発生日
   * Jira のユーザーの名前
   * Jira のイシュー番号
   * 発生したエラーの簡単な説明。
