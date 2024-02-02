---
product-area: reporting
keywords: 変更,所有者,共有,レポート,共有,実行,ユーザー,アクセス,権限,入力,最終,表示,日付,レポート,アクティビティ
navigation-topic: report-usage
title: レポートアクティビティに関するレポートの作成
description: レポートに関するレポートを作成すると、特定のレポート情報を特定できます。例えば、非アクティブ化されたユーザーにレポートが割り当てられているかどうか、非アクティブ化されたユーザーのアクセス権で実行されるようにレポートが設定されているかどうか、削除する予定のレポートにユーザーがアクセスしているかどうかなどです。
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: ht
source-wordcount: '670'
ht-degree: 100%

---

# レポートアクティビティに関するレポートの作成

レポートに関するレポートを作成すると、特定のレポート情報を特定できます。例えば、非アクティブ化されたユーザーにレポートが割り当てられているかどうか、非アクティブ化されたユーザーのアクセス権で実行されるようにレポートが設定されているかどうか、削除する予定のレポートにユーザーがアクセスしているかどうかなどです。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 既存のレポートに関するレポートの作成 {#create-the-report-about-existing-reports}

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。
1. 「**レポート**」をクリックし、次に「**新規報告書**」を選択します。
1. **新規報告書**&#x200B;ドロップダウンメニューで、「**レポート**」を選択して、既存のレポートに関するレポートを作成します。

1. 「**カラム （表示）**」タブで、レポートに必要な列を追加します。\
   次のフィールドの一部が役立つ場合があります。

   | フィールド | 説明 |
   |---|---|
   | **ユーザーとして実行：名前** | これは、レポートの「**次のアクセス権限でこの報告書を作成する:**」フィールドで指定されたユーザーです。このユーザーが非アクティブ化されている場合、レポートは、そのレポートを共有しているどのユーザーにも表示されません。 |
   | **共有者** | これらは、レポートの共有先となるすべてのエンティティです。 |
   | **入力者** | これはレポートの所有者です。 |
   | **最終表示日** | これは、レポートが最後にユーザーに閲覧された日時です。 |

   {style="table-layout:auto"}

1. （オプション）レポートのリストを非アクティブ化された特定のユーザーに制限するには、次の手順に従います。

   1. 「**フィルター**」タブを選択し、「**フィルター規則の追加**」をクリックします。

   1. **ユーザー ID として実行**／**が次に等しい**&#x200B;というフィルターを追加します。

   1. このフィルターに追加する非アクティブ化されたユーザーの名前を入力し、リストに表示された名前をクリックします。
   1. レポートに含める非アクティブ化されたユーザーをすべて選択するまで、手順 c を繰り返します。

1. （オプション）レポートのリストをスケジュール済みレポートに限定するには、次の手順に従います。

   1. 「**フィルター**」タブを選択し、「**フィルター規則の追加**」をクリックします。

   1. **スケジュール済み報告書 ID**／**が空白ではない**&#x200B;というフィルターを追加します。

1. 「**保存して閉じる**」をクリックし、レポートの名前を入力して、「**報告書の保存**」をクリックします。

   レポート情報が表示されます。

1. （オプション）このレポートを Excel に書き出し、お使いのコンピューターに保存します。\
   レポートの書き出しについて詳しくは、[データの書き出し](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)を参照してください。

## レポートに関する情報の更新

レポートを作成した後、必要に応じてレポートを更新できます。

1. 更新するレポートに移動します。
1. 実行するアクションに応じて、以下の操作のいずれかを行います。

   * **次のアクセス権限でこの報告書を作成する:**&#x200B;フィールドを、アクティブユーザーで更新する：詳細については、[別のユーザーのアクセス権を使用してレポートを実行して配信](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)を参照してください。

   * レポートのコピーを作成：詳細については、[レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)を参照してください。
   * レポートを削除：詳細については、[レポートのコピーを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)の[レポートの正確なコピーを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2)セクションを参照してください。

   * レポートを共有：詳しくは、[Adobe Workfront でのレポートを共有](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)を参照してください。

1. （条件付き）オリジナルレポートをコピーする場合は、[既存のレポートに関するレポートの作成](#create-the-report-about-existing-reports)で作成したレポートの情報を使用して、新しいコピーをオリジナルレポートと同じエンティティと共有します。
