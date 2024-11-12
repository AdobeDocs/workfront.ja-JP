---
title: Workfront計画レコードの自動作成を使用したWorkfront オブジェクトの作成
description: Workfront Planning で自動化を構成し、アクティブ化するとWorkfrontにオブジェクトを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: d8631e16234486479aa70233aa3770b28ea0d218
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Workfront計画レコードの自動作成を使用したWorkfront オブジェクトの作成

Workfront Planning で自動化を構成し、アクティブ化するとWorkfrontにオブジェクトを作成できます。

レコードの自動処理をアクティブ化します。 Workfrontのオブジェクトは、自動処理をアクティブ化した計画レコードに接続されています。

例えば、Workfront Planning キャンペーンを受け取り、Workfrontでプロジェクトを作成して、そのキャンペーンの進行状況を追跡する自動処理を作成できます。 プロジェクトは、Workfront Planning キャンペーンに接続されます。

接続されたレコードについて詳しくは、「[ 接続されたレコードの概要 ](/help/quicksilver/planning/records/connected-records-overview.md)」を参照してください。


## Workfront Planning での自動処理の設定

Workfront Planning を使用してWorkfront オブジェクトを作成する前に、自動処理を設定する必要があります。

1. **その他** メニュー ![](assets/more-menu.png) をクリックし、**Automations** を選択します。

   使用可能な自動化のリストが開きます。

1. 画面の右上隅にある「**新しい自動化を作成**」をクリックします。
1. 「**ボタンテキスト**」フィールドで、ボタンに表示するテキストを入力します。 自動処理を使用してWorkfront オブジェクトを作成する際に、このボタンをクリックします。
1. （オプション）ボタンにアイコンを追加するには、利用可能なオプションからアイコンを選択します。
1. **タイプを作成** フィールドで、オートメーションで作成するオブジェクトを選択します。

   使用可能なオブジェクトは次のとおりです。

   * プロジェクト
   * ポートフォリオ
   * プログラム
   * グループ

1. **プロジェクト名で使用するフィールドを選択** フィールドで、レコードフィールドを選択します。 Workfrontの新しいプロジェクトには、このフィールドの内容が名前として含まれます。
1. **作成したプロジェクトをリンクするフィールドを選択** フィールドで、レコードフィールドを選択します。 Workfront Planning でレコードを表示すると、Workfrontの新しいプロジェクトがこのフィールドに表示されます。
1. 作成するオブジェクトのタイプに使用できるその他のオプションを選択します。
1. **作成** をクリックします。

自動処理は自動処理のリストに表示され、レコードで使用できます。

## Workfront Planning 自動処理を使用したWorkfrontオブジェクトの作成

1. Workfront Planning で、Workfrontオブジェクトの作成に使用するレコードを含む「レコード・タイプ」ページを開きます。
1. 1 つ以上のレコードを選択します。
1. 画面の右下隅付近にあるオートメーションボタンをクリックします。

   この例では、「プロジェクトを作成」ボタンです。

   ![ オートメーションボタン ](assets/automation-custom-button.png)

>[!NOTE]
>
>オブジェクトが作成され、期待どおりに接続されたことを確認することをお勧めします。

