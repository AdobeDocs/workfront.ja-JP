---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントのインストール
description: ブループリントは、実稼動環境またはサンドボックス環境にインストールできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# ブループリントのインストール

ブループリントは、実稼動環境またはサンドボックス環境にインストールできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画</strong></td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL システム管理者 ]</p> </td> 
  </tr> 
 </tbody> 
</table>

## ブループリントはどこにインストールすればよいですか？ {#where-should-i-install-a-blueprint}

パッケージは、次のいずれかの環境にインストールできます。

<table style="table-layout:auto">
        <tr>
        <td><strong>実稼動</strong></td>
        <td>実稼動環境は実稼動環境です。</td>
    </tr>
    <tr>
        <td><strong>サンドボックス プレビュー</strong></td>
        <td>サンドボックスプレビューは、ライブ環境のレプリカとして機能し、Workfrontが週末に更新するテスト環境です。 すべてのサポートパッケージは、サンドボックスプレビューにアクセスできます。 詳しくは、 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">この [!DNL Adobe Workfront] サンドボックス環境をプレビュー</a>.</td>
    </tr>
    <tr>
        <td><strong>サンドボックス 1 および 2</strong></td>
        <td>カスタム更新サンドボックスは、個別のテスト環境で、手動で更新されます。 カスタム更新サンドボックスを取得するには、追加のコストが必要です。 詳しくは、 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">この [!DNL Adobe Workfront] カスタム更新サンドボックス環境</a>.</td>
    </tr>
</table>

>[!TIP]
>
>まず、サンドボックス環境にブループリントをインストールすることをお勧めします。 これにより、ライブデータを変更することなく、ブループリントのコンテンツをテストし、組織に適したコンテンツであることを確認できます。

>[!NOTE]
>
>特定のブループリントは、テスト目的でプレビュー環境にのみインストールできます。 実稼動環境、サンドボックス 1、またはサンドボックス 2 のプレビューのみのコンテンツにアクセスする場合、「インストール」ボタンがアクティブにならず、警告メッセージが表示されることがあります。\
>また、プレビューのみのコンテンツにアクセスする場合は、プレビュー環境にいる場合でも、環境の切り替え機能が制限されます。

## ブループリントをインストール

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL ブループリント]**.
1. インストールするブループリントを見つけます。 右側で、使用例、成熟度レベル、インストールステータスおよびタイプでフィルタリングできます。
1. （オプション）「 **[!UICONTROL 詳細]** ブループリントの動作の仕組みを学ぶには
1. クリック **[!UICONTROL インストール]**.
1. 実稼動環境またはサンドボックス環境にをインストールすることを選択します。\
   詳しくは、 [ブループリントはどこにインストールすればよいですか？](#where-should-i-install-a-blueprint) 」の節を参照してください。
1. の [!UICONTROL 設定] 」ページで、次のいずれかの操作を選択できます。

   * ブループリントをそのままインストールします。 設定が不要なブループリントタイプの場合は、これが唯一のオプションです。 設定が必要なブループリントの種類の場合は、オプションでブループリントを今すぐインストールし、後で設定することもできます。 クリック **[!UICONTROL そのままインストール]**.
   * 設定が必要なブループリント用に、インストール前にブループリントを設定します。 設定を選択し、 **[!UICONTROL ブループリントをインストール]**.\

      詳しくは、 [ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md).
インストールが完了すると、ブループリントと共に正常にインストールされた特定のオブジェクト（役割、チーム、グループなど）と、インストールに失敗したオブジェクトのリストがメッセージに表示されます。

ブループリントをインストールした後、完全にデプロイするには、追加のアクションが必要になる場合があります。 詳しくは、 [ブループリントのインストール後に実行するアクション](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
