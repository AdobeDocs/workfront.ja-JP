---
navigation-topic: business-case-and-scorecards
title: プロジェクトのビジネスケースの作成
description: ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。 Portfolioマネージャまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# プロジェクトのビジネスケースの作成

ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。 Portfolioマネージャまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>プラン以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、財務データ、およびリソース管理へのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限を管理するか、それ以上に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ビジネスケースを通じてプロジェクトをリクエストする際は、次の点を考慮してください。

* Adobe Workfront管理者またはグループ管理者は、ビジネスケースのセクションを有効にしてから、プロジェクトに表示する必要があります。\
   システムレベルでビジネスケースのセクションを有効にする方法については、この記事を参照してください。 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   ビジネス事例の分野については、 [ビジネス事例の領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Portfolio・オプティマイザでプロジェクトにスコアを割り当てる場合は、「目標」領域を除き、ビジネス・ケースのすべての領域を完了する必要があります。 「目標」領域の設定はオプションです。 この領域が未完了の場合でも、プロジェクトはPortfolio・オプティマイザでスコアを受け取ります。

   スコアカードの使用と Scorecard Optimizer の使用の詳細については、「Portfolio・オプティマイザ」を参照してください。 [プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## ビジネスケースの作成

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png)を選択し、「 **プロジェクト**.
1. クリック **新規プロジェクト** を選択し、 **プロジェクトをリクエスト**.\
   デフォルトでは、プロジェクトは **アイデア** ステータス。

   >[!CAUTION]
   >
   >Workfrontインスタンスでアイデアのステータスが削除されている場合、プロジェクトは、プロジェクトの環境設定領域で定義された、新規プロジェクトのデフォルトのステータスに配置されます。 プロジェクトの環境設定の詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. プロジェクトの名前を指定し、Enter キーを押します。
1. （オプション） **詳細** アイコン ![](assets/qs-more-icon-on-an-object.png)を、 **テンプレートを添付**&#x200B;を使用して、プロジェクトの作業分類構造を作成します。

   または

   手動でプロジェクトへのタスクの追加を開始します。

1. （条件付き）テンプレートの添付を選択した場合は、引き続きテンプレートをプロジェクトに添付します
1. クリック **ビジネス事例** をクリックします。
1. （オプション）「 **プロジェクト情報の編集**. 

   ビジネスケースの「プロジェクト情報」セクションのフィールドの編集の詳細については、「 [プロジェクト情報](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) 記事内 [ビジネス事例の領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （オプション）「 **目標を編集**.

   ビジネスケースの「目標」セクションの編集の詳細については、 [目標](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) 記事内 [ビジネス事例の領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （オプション）「**費用の編集**.

   ビジネスケースの費用セクションの編集の詳細については、 [費用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) 記事内 [ビジネス事例の領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （オプション）「生産資源予算設定」領域を使用して、生産資源を予算し、プロジェクトの役職ロールに関連する予算労務費を取得します。 詳しくは、 [ビジネス事例の予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >ここに表示される情報は、システムレベルのリソース予算ツールに表示される情報と同じです。

1. （オプション）「 **リスクを編集** このプロジェクトに潜在的なリスクを追加する ビジネス事例へのリスクの追加については、 [リスク](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) 記事のセクション [ビジネス事例の領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. （オプション）**スコアカード** 内 **このプロジェクトにスコ****カードを追加します** ドロップダウンメニュー。

   スコアカードをプロジェクトに添付する前に作成する必要があります。

   スコアカードの詳細については、「 [プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. （オプション） **カスタムフォーム** 内 **カスタムForms** ドロップダウンメニュー。

   カスタムFormsをプロジェクトに添付するには、事前に作成しておく必要があります。

   カスタムFormsについて詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. クリック **送信**.

   プロジェクトのステータスが **リクエスト** ビジネスケースの承認を得るために送信されます。

   ビジネス事例の承認の詳細については、「 [ビジネスケースの承認](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

1. （オプション）ビジネスケースの作成が完了したら、そのコピーを.pdf ファイルに書き出すことができます。 ビジネスケースを.pdf ファイルにエクスポートする方法の詳細については、この記事の「ビジネスケースのエクスポート」の節を参照してください [ビジネス事例の領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
