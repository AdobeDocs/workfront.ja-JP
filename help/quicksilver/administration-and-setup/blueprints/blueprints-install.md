---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントのインストール
description: ブループリントは、実稼動環境またはサンドボックス環境にインストールできます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 74%

---

# ブループリントをインストール

<!-- Audited: 5/2025 -->

ブループリントは、実稼動環境またはサンドボックス環境にインストールできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!DNL Workfront] 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

この表にある情報についての詳細は、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ブループリントはどこにインストールすればよいですか？ {#where-should-i-install-a-blueprint}

パッケージは、次のいずれかの環境にインストールできます。

<table style="table-layout:auto">
        <tr>
        <td><strong>実稼動</strong></td>
        <td>実稼動環境はライブ環境です。</td>
    </tr>
    <tr>
        <td><strong>サンドボックスプレビュー</strong></td>
        <td>サンドボックスプレビューは、ライブ環境のレプリカとして機能するテスト環境で、Adobe Workfrontによって毎週週末に更新されます。 すべてのサポートパッケージは、サンドボックスプレビューにアクセスできます。詳しくは、<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">[!DNL Adobe Workfront]サンドボックス環境のプレビュー</a>を参照してください。</td>
    </tr>
    <tr>
        <td><strong>サンドボックス 1 および 2</strong></td>
        <td>カスタム更新サンドボックスは、個別のテスト環境で、ユーザーが手動で更新します。カスタム更新サンドボックスを取得するには、追加の費用がかかります。詳しくは、<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">[!DNL Adobe Workfront]カスタム更新サンドボックス環境</a>を参照してください。</td>
    </tr>
</table>

>[!TIP]
>
>まずサンドボックス環境にブループリントをインストールすることをお勧めします。 これにより、ライブデータを変更することなく、ブループリントのコンテンツをテストし、組織に適したコンテンツであることを確認できます。

>[!NOTE]
>
>特定のブループリントは、テスト目的でプレビュー環境にのみインストールできます。実稼動環境、サンドボックス 1、またはサンドボックス 2 でプレビューのみのコンテンツにアクセスする場合、「インストール」ボタンがアクティブにならず、警告メッセージが表示されることがあります。\
>さらに、プレビュー環境であっても、プレビューのみのコンテンツにアクセスすると、環境の切り替え機能が制限されます。

## ブループリントのインストール

{{step1-to-blueprints}}

1. インストールするブループリントを見つけます。ページの右側で、ユースケース、成熟度レベル、インストールステータスおよびタイプでフィルタリングできます。
1. （オプション）ブループリントの動作の仕組みを学ぶには、「**[!UICONTROL 詳細]**」をクリックします。
1. 「**[!UICONTROL インストール]**」をクリックします。
1. 実稼動環境にインストールするか、サンドボックス環境にインストールするかを選択します。\
   詳しくは、この記事の[ブループリントはどこにインストールすればよいですか？](#where-should-i-install-a-blueprint)の節を参照してください。
1. 「**設定**」ページで、次のいずれかの操作を選択できます。

   * ブループリントをそのままインストールします。設定を必要としないブループリントタイプの場合は、これが唯一のオプションです。設定が必要なブループリントの種類の場合は、オプションでブループリントを今すぐインストールし、後で設定することもできます。「**[!UICONTROL そのままインストール]**」をクリックします。
   * 設定が必要なブループリント用に、インストール前にブループリントを設定します。設定を選択し、「**[!UICONTROL ブループリントをインストール]**」をクリックします。

     詳しくは、[ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md)を参照してください。

   インストールが完了すると、ブループリントと共に正常にインストールされた特定のオブジェクト（役割、チーム、グループなど）と、インストールに失敗したオブジェクトのリストがメッセージに表示されます。

ブループリントをインストールした後、完全にデプロイするには、追加のアクションが必要になる場合があります。詳しくは、[ブループリントのインストール後に実行するアクション](../../administration-and-setup/blueprints/best-next-actions-after-install.md)を参照してください。
