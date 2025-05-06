---
navigation-topic: business-case-and-scorecards
title: プロジェクトのビジネスケースの作成
description: ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。ポートフォリオマネージャーまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 66%

---

# プロジェクトのビジネスケースの作成

ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。ポートフォリオマネージャーまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>Plan 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、財務データ、リソース管理へのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する「管理」以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへの利用申請</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

ビジネスケースを通じてプロジェクトをリクエストする際は、次の点を考慮してください。

* プロジェクトにビジネスケースのセクションが表示されるには、Adobe Workfront 管理者またはグループ管理者は当セクションを有効にする必要があります。\
  システムレベルでビジネスケースのセクションを有効にする方法については、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

  ビジネスケースの分野について詳しくは、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)を参照してください。

* ポートフォリオオプティマイザーでプロジェクトにスコアを割り当てる場合は、目標エリアを除き、ビジネスケースのすべてのエリアを完了する必要があります。目標エリアの設定はオプションです。このエリアが未完了の場合でも、プロジェクトはポートフォリオオプティマイザーでスコアを受け取ります。

  スコアカードの使用とポートフォリオオプティマイザーの使用の詳細については、[プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

## ビジネスケースの作成

{{step1-to-projects}}

1. **新規プロジェクト** をクリックし、表示されるドロップダウンから **プロジェクトをリクエスト** を選択します。 プロジェクトが作成され、**アイデア** ステータスがデフォルトで割り当てられます。

   >[!CAUTION]
   >
   >Workfront インスタンスで「アイデア」ステータスが削除されている場合、プロジェクトは、プロジェクトの環境設定エリアで定義された、新規プロジェクトのデフォルトのステータスに配置されます。プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. 「プロジェクトタイトル」フィールドに名前を入力します。
1. （任意） **詳細** アイコン ![ 詳細アイコン ](assets/qs-more-icon-on-an-object.png)、**テンプレートを添付** の順にクリックして、プロジェクトの作業分解構造を作成します。

   または

   手動でプロジェクトへのタスクの追加を開始します。

1. （条件付き）テンプレートを添付することを選択した場合、引き続きプロジェクトにテンプレートを添付します。
1. 左側のパネルで、「ビジネスケース **をクリック** ます。
1. （任意）「**プロジェクト情報**」セクションを編集するには、「**プロジェクト情報を編集**」をクリックします。 

   **プロジェクト情報** セクションフィールドの編集について詳しくは、記事 [ ビジネスケースの領域の概要 [ の ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) プロジェクト情報 ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md) の節を参照してください。

1. （任意）「**目標**」セクションを編集するには、「**目標を編集**」をクリックします。

   ビジネスケースの **目標** セクションの編集について詳しくは、記事 [ ビジネスケースの領域の概要 ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md) の [ 目標 ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) の節を参照してください。

1. （任意）「**費用**」セクションを編集するには、「**費用の編集**」をクリックします。

   ビジネスケースの **費用** セクションの編集について詳しくは、記事 [ ビジネスケースの領域の概要 ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md) の [ 費用 ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) の節を参照してください。

1. （任意）「**リソース予算の編集**」をクリックして、リソースを予算に計上し、プロジェクトの担当業務に関連する予算計上労力コストを取得します。 詳しくは、[ビジネスケースの予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

   >[!TIP]
   >
   >ここに表示される情報は、システムレベルのリソース予算計上ツールに表示される情報と同じです。

1. （オプション）このプロジェクトに潜在的なリスクを追加するには、「**リスクを編集**」をクリックします。ビジネスケースへのリスクの追加については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)記事の[リスク](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)の節を参照してください。
1. （任意）「**このプロジェクトにスコアカードを追加**」ドロップダウンメニューで **スコアカード** を選択します。

   プロジェクトに添付する前に、スコアカードを作成する必要があります。

   スコアカードの詳細については、[プロジェクトへのスコアカードの適用で整合性スコアを生成](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

1. （オプション）**カスタムフォーム**&#x200B;ドロップダウンメニューの「**カスタムフォーム**」を選択します。

   プロジェクトに添付する前に、カスタムフォームを作成する必要があります。

   カスタム Formsの詳細については、「[ カスタム フォームを作成する ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

1. **送信** をクリックします。 プロジェクトのステータスが「**リクエスト済み**」に変更されて、ビジネスケースの承認を得るために送信されます。

   ビジネスケースの承認について詳しくは、[ビジネスケースを承認](../../../manage-work/projects/define-a-business-case/approve-business-case.md)を参照してください。


>[!TIP]
>
> ビジネスケースが完了したら、そのコピーを.pdf ファイルに書き出すことができます。 ビジネスケースを.pdf ファイルにエクスポートする方法については、[ プロジェクトのビジネスケースのエクスポート ](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md) を参照してください。


