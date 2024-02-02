---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントをインストール
description: ブループリントは、実稼動環境またはサンドボックス環境にインストールできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: ht
source-wordcount: '467'
ht-degree: 100%

---

# ブループリントをインストール

ブループリントは、実稼動環境またはサンドボックス環境にインストールできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン</strong></td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## ブループリントはどこにインストールすればよいですか？ {#where-should-i-install-a-blueprint}

パッケージは、次のいずれかの環境にインストールできます。

<table style="table-layout:auto">
        <tr>
        <td><strong>実稼動</strong></td>
        <td>実稼動環境はライブ環境です。</td>
    </tr>
    <tr>
        <td><strong>サンドボックスプレビュー</strong></td>
        <td>サンドボックスプレビューは、ライブ環境のレプリカとして機能し、Workfront が週末に更新するテスト環境です。すべてのサポートパッケージは、サンドボックスプレビューにアクセスできます。詳しくは、<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">[!DNL Adobe Workfront]サンドボックス環境のプレビュー</a>を参照してください。</td>
    </tr>
    <tr>
        <td><strong>サンドボックス 1 および 2</strong></td>
        <td>カスタム更新サンドボックスは、個別のテスト環境で、ユーザーが手動で更新します。カスタム更新サンドボックスを取得するには、追加の費用がかかります。詳しくは、<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">[!DNL Adobe Workfront]カスタム更新サンドボックス環境</a>を参照してください。</td>
    </tr>
</table>

>[!TIP]
>
>まず、サンドボックス環境にブループリントをインストールすることをお勧めします。これにより、ライブデータを変更することなく、ブループリントのコンテンツをテストし、組織に適したコンテンツであることを確認できます。

>[!NOTE]
>
>特定のブループリントは、テスト目的でプレビュー環境にのみインストールできます。実稼動環境、サンドボックス 1、またはサンドボックス 2 でプレビューのみのコンテンツにアクセスする場合、「インストール」ボタンがアクティブにならず、警告メッセージが表示されることがあります。\
>また、プレビューのみのコンテンツにアクセスする場合は、プレビュー環境にいる場合でも、環境切り替え機能が制限されます。

## ブループリントのインストール

1. [!DNL Adobe] Workfront 右上隅の **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) をクリックし、「**[!UICONTROL ブループリント]**」をクリックします。
1. インストールするブループリントを見つけます。右側では、ユースケース、成熟度レベル、インストールステータス、タイプでフィルタリングできます。
1. （オプション）ブループリントの動作の仕組みを学ぶには、「**[!UICONTROL 詳細]**」をクリックします。
1. 「**[!UICONTROL インストール]**」をクリックします。
1. 実稼動環境にインストールするか、サンドボックス環境にインストールするかを選択します。\
   詳しくは、この記事の[ブループリントはどこにインストールすればよいですか？](#where-should-i-install-a-blueprint)の節を参照してください。
1. 「[!UICONTROL 設定]」ページで、次のいずれかの操作を選択できます。

   * ブループリントをそのままインストールします。設定を必要としないブループリントタイプの場合は、これが唯一のオプションです。設定が必要なブループリントの種類の場合は、オプションでブループリントを今すぐインストールし、後で設定することもできます。「**[!UICONTROL そのままインストール]**」をクリックします。
   * 設定が必要なブループリント用に、インストール前にブループリントを設定します。設定を選択し、「**[!UICONTROL ブループリントをインストール]**」をクリックします。

     詳しくは、[ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md)を参照してください。
インストールが完了すると、ブループリントと共に正常にインストールされた特定のオブジェクト（役割、チーム、グループなど）と、インストールに失敗したオブジェクトのリストがメッセージに表示されます。

ブループリントをインストールした後、完全にデプロイするには、追加のアクションが必要になる場合があります。詳しくは、[ブループリントのインストール後に実行するアクション](../../administration-and-setup/blueprints/best-next-actions-after-install.md)を参照してください。
