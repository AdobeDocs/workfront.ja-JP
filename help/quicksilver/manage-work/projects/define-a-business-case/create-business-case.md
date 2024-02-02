---
navigation-topic: business-case-and-scorecards
title: プロジェクトのビジネスケースの作成
description: ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。ポートフォリオマネージャーまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '831'
ht-degree: 100%

---

# プロジェクトのビジネスケースの作成

ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。ポートフォリオマネージャーまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>Plan 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、財務データ、リソース管理へのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する「管理」以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

ビジネスケースを通じてプロジェクトをリクエストする際は、次の点を考慮してください。

* プロジェクトにビジネスケースのセクションが表示されるには、Adobe Workfront 管理者またはグループ管理者は当セクションを有効にする必要があります。\
  システムレベルでビジネスケースのセクションを有効にする方法については、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

  ビジネスケースの分野について詳しくは、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)を参照してください。

* ポートフォリオオプティマイザーでプロジェクトにスコアを割り当てる場合は、目標エリアを除き、ビジネスケースのすべてのエリアを完了する必要があります。目標エリアの設定はオプションです。このエリアが未完了の場合でも、プロジェクトはポートフォリオオプティマイザーでスコアを受け取ります。

  スコアカードの使用とポートフォリオオプティマイザーの使用の詳細については、[プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

## ビジネスケースの作成

1. **メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**プロジェクト**&#x200B;の順にクリックします。
1. 「**新規プロジェクト**」、「**プロジェクトをリクエスト**」の順に選択します。\
   デフォルトでは、プロジェクトのステータスは&#x200B;**アイデア**&#x200B;になっています。

   >[!CAUTION]
   >
   >Workfront インスタンスで「アイデア」ステータスが削除されている場合、プロジェクトは、プロジェクトの環境設定エリアで定義された、新規プロジェクトのデフォルトのステータスに配置されます。プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. プロジェクトの名前を指定し、Enter キーを押します。
1. （オプション）**その他**&#x200B;アイコン ![](assets/qs-more-icon-on-an-object.png)、「**テンプレートを添付**」の順にクリックして、プロジェクトの作業分類構造を作成します。

   または

   手動でプロジェクトへのタスクの追加を開始します。

1. （条件付き）テンプレートの添付を選択した場合は、引き続きテンプレートをプロジェクトに添付します。
1. 左パネルの「**ビジネスケース**」をクリックします。
1. （オプション）「**プロジェクト情報の編集**」をクリックします。

   ビジネスケースのプロジェクト情報セクションのフィールドの編集の詳細については、[ビジネスケースの領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)記事で[プロジェクト情報](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)の節を参照してください。

1. （オプション）「**目標を編集**」をクリックします。

   ビジネスケースの目標セクションの編集について詳しくは、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)記事内の[目標](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals)の節を参照してください。

1. （オプション）「**費用の編集**」をクリックします。

   ビジネスケースの費用セクションの編集について詳しくは、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)記事内の[費用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses)の節を参照してください。

1. （オプション）リソース予算計上エリアを使用して、リソースを予算計上し、プロジェクトの担当業務に関連する予算計上労力コストを取得します。詳しくは、[ビジネスケースの予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

   >[!TIP]
   >
   >ここに表示される情報は、システムレベルのリソース予算計上ツールに表示される情報と同じです。

1. （オプション）このプロジェクトに潜在的なリスクを追加するには、「**リスクを編集**」をクリックします。ビジネスケースへのリスクの追加については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)記事の[リスク](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)の節を参照してください。
1. （オプション）**このプロジェクトにスコア****カードを追加**&#x200B;ドロップダウンメニューの「**スコアカード**」を選択します。

   プロジェクトに添付する前に、スコアカードを作成する必要があります。

   スコアカードの詳細については、[プロジェクトへのスコアカードの適用で整合性スコアを生成](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

1. （オプション）**カスタムフォーム**&#x200B;ドロップダウンメニューの「**カスタムフォーム**」を選択します。

   プロジェクトに添付する前に、カスタムフォームを作成する必要があります。

   カスタムフォームの詳細については、[カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

1. 「**送信**」をクリックします。

   プロジェクトのステータスが「**リクエスト済み**」に変更されて、ビジネスケースの承認を得るために送信されます。

   ビジネスケースの承認について詳しくは、[ビジネスケースを承認](../../../manage-work/projects/define-a-business-case/approve-business-case.md)を参照してください。

1. （オプション）ビジネスケースが完了したら、そのコピーを .pdf ファイルに書き出すことができます。ビジネスケースを .pdf ファイルに書き出す方法の詳細については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の「ビジネスケースの書き出し」の節を参照してください。
