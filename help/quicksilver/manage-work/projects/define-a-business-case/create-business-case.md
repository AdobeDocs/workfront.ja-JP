---
navigation-topic: business-case-and-scorecards
title: プロジェクトのビジネスケースの作成
description: ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。 ポートフォリオマネージャーまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。
author: Becky
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
TQID: https://experienceleague.adobe.com/LqbRptv6SejiN1K5SsAHDKzXDbKCwFeFT9W1rPjRafo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 783
ht-degree: 63%

---

# プロジェクトのビジネスケースの作成

<!--Audited: 6/2025-->

ビジネスケースを使用して、プロジェクトをリクエストし、プロジェクトの目的、予算および潜在的な利益を定義できます。 ポートフォリオマネージャーまたはプロジェクトスポンサーは、ビジネスケースの情報を使用して、プロジェクトを承認する前に分析し、優先順位を付けます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
   <p>Prime以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
   <p>標準 </p> 
   <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>プロジェクト、財務データ、リソース管理へのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>プロジェクトに対する「管理」以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

ビジネスケースを通じてプロジェクトをリクエストする際は、次の点を考慮してください。

* プロジェクトにビジネスケースのセクションが表示されるには、Adobe Workfront 管理者またはグループ管理者は当セクションを有効にする必要があります。\
  システムレベルでビジネスケースのセクションを有効にする方法については、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

  ビジネスケースの分野について詳しくは、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)を参照してください。

* ポートフォリオオプティマイザーでプロジェクトにスコアを割り当てる場合は、目標エリアを除き、ビジネスケースのすべてのエリアを完了する必要があります。 目標エリアの設定はオプションです。 このエリアが未完了の場合でも、プロジェクトはポートフォリオオプティマイザーでスコアを受け取ります。

  スコアカードの使用とポートフォリオオプティマイザーの使用の詳細については、[プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

## ビジネスケースの作成

{{step1-to-projects}}

1. **新規プロジェクト**&#x200B;をクリックし、表示されるドロップダウンから「**プロジェクトをリクエスト**」を選択します。 プロジェクトが作成され、デフォルトで&#x200B;**Idea** ステータスが割り当てられます。

   >[!CAUTION]
   >
   >Workfront インスタンスで「アイデア」ステータスが削除されている場合、プロジェクトは、プロジェクトの環境設定エリアで定義された、新規プロジェクトのデフォルトのステータスに配置されます。 プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. プロジェクトタイトル フィールドに名前を入力します。
1. （オプション）「**More**」アイコン「![More」アイコン「](assets/qs-more-icon-on-an-object.png)」をクリックし、**テンプレートを添付**」をクリックして、プロジェクトの作業分解構成図を作成します。

   または

   手動でプロジェクトへのタスクの追加を開始します。

1. （条件付き）テンプレートの添付を選択した場合は、引き続きテンプレートをプロジェクトに添付します。
1. 左側のパネルで、**ビジネスケース**&#x200B;をクリックします。
1. （オプション）「**プロジェクト情報**」セクションを編集するには、「**プロジェクト情報を編集**」をクリックします。

   **プロジェクト情報** セクション フィールドの編集について詳しくは、記事[ ビジネスケースの領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の[ プロジェクト情報](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)の節を参照してください。

1. （オプション） **目標** セクションを編集するには、**目標を編集**&#x200B;をクリックします。

   ビジネスケースの&#x200B;**目標** セクションの編集について詳しくは、記事[ ビジネスケースの領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の[目標](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals)の節を参照してください。

1. （オプション）「**費用**」セクションを編集するには、「**費用を編集**」をクリックします。

   ビジネスケースの&#x200B;**費用** セクションの編集について詳しくは、記事[ ビジネスケースの領域の概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の[費用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses)の節を参照してください。

1. （オプション）「**リソース予算を編集**」をクリックして、リソースを予算し、プロジェクトの担当業務に関連付けられている予算計上労力コストを取得します。 詳しくは、[ビジネスケースの予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

   >[!TIP]
   >
   >ここに表示される情報は、システムレベルのリソース予算計上ツールに表示される情報と同じです。

1. （オプション）「**リスクを編集**」をクリックして、このプロジェクトに潜在的なリスクを追加します。 ビジネスケースへのリスクの追加については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)記事の[リスク](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)の節を参照してください。
1. （オプション）「**このプロジェクトにスコアカードを追加**」ドロップダウンメニューで&#x200B;**スコアカード**&#x200B;を選択します。

   プロジェクトに添付する前に、スコアカードを作成する必要があります。

   スコアカードの詳細については、[プロジェクトへのスコアカードの適用で整合性スコアを生成](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

1. （オプション）**カスタムフォーム**&#x200B;ドロップダウンメニューの「**カスタムフォーム**」を選択します。

   プロジェクトに添付する前に、カスタムフォームを作成する必要があります。

   カスタム Formsについて詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

1. 「**送信**」をクリックします。 プロジェクトのステータスが「**リクエスト済み**」に変更されて、ビジネスケースの承認を得るために送信されます。

   ビジネスケースの承認について詳しくは、[ビジネスケースを承認](../../../manage-work/projects/define-a-business-case/approve-business-case.md)を参照してください。


>[!TIP]
>
> ビジネスケースが完了したら、そのコピーを.pdf ファイルに書き出すことができます。 ビジネスケースを.pdf ファイルに書き出す方法について詳しくは、[ プロジェクトのビジネスケースの書き出し](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md)を参照してください。


