---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントのインストール
description: ブループリントは、本番環境またはサンドボックス環境にインストールできます。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 75%

---

# ブループリントをインストール

<!-- Audited: 5/2025 -->

ブループリントは、本番環境またはサンドボックス環境にインストールできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
        <td>サンドボックスプレビューは、ライブ環境のレプリカとして機能するテスト環境で、Adobe Workfrontによって毎週末更新されます。 すべてのサポートパッケージは、サンドボックスプレビューにアクセスできます。詳しくは、<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">[!DNL Adobe Workfront]サンドボックス環境のプレビュー</a>を参照してください。</td>
    </tr>
    <tr>
        <td><strong>サンドボックス 1 および 2</strong></td>
        <td>カスタム更新サンドボックスは、個別のテスト環境で、ユーザーが手動で更新します。カスタム更新サンドボックスを取得するには、追加の費用がかかります。詳しくは、<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">[!DNL Adobe Workfront]カスタム更新サンドボックス環境</a>を参照してください。</td>
    </tr>
</table>

>[!TIP]
>
>まず、ブループリントをサンドボックス環境にインストールすることをお勧めします。 これにより、ライブデータを変更することなく、ブループリントのコンテンツをテストし、組織に適したコンテンツであることを確認できます。

>[!NOTE]
>
>特定のブループリントは、テスト目的でプレビュー環境にのみインストールできます。本番環境、サンドボックス 1、またはサンドボックス 2 でプレビューのみのコンテンツにアクセスする場合、「インストール」ボタンがアクティブにならず、警告メッセージが表示されることがあります。\
>さらに、プレビュー環境であっても、プレビュー専用コンテンツにアクセスする場合、環境の切り替え機能は制限されます。

## ブループリントのインストール

{{step1-to-blueprints}}

1. インストールするブループリントを見つけます。ユースケース、成熟度、インストール状況、タイプ別にフィルタリングできます。
1. （オプション）ブループリントの動作の仕組みを学ぶには、「**[!UICONTROL 詳細]**」をクリックします。
1. 「**[!UICONTROL インストール]**」をクリックします。
1. 本番環境にインストールするか、サンドボックス環境にインストールするかを選択します。\
   詳しくは、この記事の[ブループリントはどこにインストールすればよいですか？](#where-should-i-install-a-blueprint)の節を参照してください。
1. 「**設定**」ページで、次のいずれかの操作を選択できます。

   * ブループリントをそのままインストールします。設定を必要としないブループリントタイプの場合は、これが唯一のオプションです。設定が必要なブループリントの種類の場合は、オプションでブループリントを今すぐインストールし、後で設定することもできます。「**[!UICONTROL そのままインストール]**」をクリックします。
   * 設定が必要なブループリント用に、インストール前にブループリントを設定します。設定を選択し、**[!UICONTROL ブループリントのインストール]**&#x200B;をクリックします。

     詳しくは、[ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md)を参照してください。

   インストールが完了し、ブループリントで正常にインストールされた特定のオブジェクト（役割、チーム、グループなど）と、インストールに失敗したオブジェクトのリストがメッセージに表示されます。

ブループリントをインストールした後、完全にデプロイするには、追加のアクションが必要になる場合があります。詳しくは、[ブループリントのインストール後に実行するアクション](../../administration-and-setup/blueprints/best-next-actions-after-install.md)を参照してください。
