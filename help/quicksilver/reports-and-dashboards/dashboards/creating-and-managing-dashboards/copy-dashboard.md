---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードのコピー
description: ダッシュボードとそのすべての内容（レポート、カレンダー、および外部ページ）をコピーできます。 ダッシュボードの内容をコピーする際に、元のダッシュボードに表示される内容を保持するか、新しい項目を作成して元のダッシュボードに表示することができます。 また、新しいダッシュボードで項目を転送またはコピーしないように選択することもできます。
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# ダッシュボードのコピー

ダッシュボードとそのすべての内容（レポート、カレンダー、および外部ページ）をコピーできます。 ダッシュボードの内容をコピーする際に、元のダッシュボードに表示される内容を保持するか、新しい項目を作成して元のダッシュボードに表示することができます。 また、新しいダッシュボードで項目を転送またはコピーしないように選択することもできます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードへのアクセスの表示</p> <p>コピーしたダッシュボードへの「管理」アクセス権が取得されます</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

ダッシュボードをコピーする前に、ダッシュボードを作成する必要があります。

ダッシュボードの作成について詳しくは、 [ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## ダッシュボードのコピー

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png)を選択し、「 **ダッシュボード**.

1. コピーするダッシュボードを選択し、「 」をクリックします。 **コピー** ![](assets/copy-icon.png).\
   または\
   コピーするダッシュボードを開き、「 」をクリックします。 **ダッシュボードのアクション** > **コピー**.\
   [ ダッシュボードコピー ] ダイアログボックスが表示されます。 元のダッシュボード上のすべての項目が表示されます。

1. 内 **ダッシュボード名** 「 」フィールドで、ダッシュボードの新しい名前を指定します。
1. 既存のダッシュボード上のすべての項目を選択し、コピーしたダッシュボードにコピーするには、そのままにします。 **すべてを選択** 選択済み デフォルトでは、既存のダッシュボード上のレポート、カレンダー、またはリストは、新しいダッシュボードにコピーされます。\
   または\
   元のダッシュボードから新しいダッシュボードに特定の項目のみを転送するには、新しいダッシュボードに表示しない項目の選択を解除し、選択した項目ごとに次のオプションを選択します。

   * **コピーを作成：** 元のダッシュボードから項目がコピーされ、その項目の新しいバージョンが新しいダッシュボードに表示されます。 新しいダッシュボードで項目に加えた変更は、元のダッシュボードの項目には反映されません。 同様に、元のダッシュボード上でアイテムに加えた変更は、新しいダッシュボード上のアイテムには反映されません。\
      元のダッシュボードの元のレポートを変更する場合は、このオプションを使用します。\
      たとえば、「Team B」という名前のダッシュボードをコピーし、名前を「Team A」に変更します。 「チーム B」ダッシュボードには、「チーム B レポート」というレポートがあります。 このレポートにはチーム B に固有のデータが含まれるので、このレポートのコピーを作成するオプションを選択して、チーム A 用にカスタマイズし、後で「チーム A レポート」に名前を変更できます。\
      このオプションを選択すると、コピーしたレポートから元のレポートの共有権限が削除されます。 「情報のアクセス権を使用してこのレポートを実行」は、コピーされたレポートにそのまま残ります。

   * **オリジナルを使用：** 元の項目を新しいダッシュボードに表示します。 新しいダッシュボードで項目に加えた変更は、元のダッシュボードの項目にも反映されます。 同様に、元のダッシュボード上の項目に加えた変更は、新しいダッシュボード上の項目に反映されます。\
      このオプションを使用すると、元のレポートの共有権限を保持できます。 「情報のアクセス権を使用してこのレポートを実行」も変更されません。

1. （オプション）選択した項目の名前を変更します。
1. クリック **ダッシュボードをコピー**.
1. （オプション）コピーしたダッシュボードで、コピーしたレポート、カレンダー、外部ページのいずれかを編集する場合は、次のいずれかの操作を行います。

   * コピーした任意のレポートの情報を編集するには、ダッシュボードでレポート名をクリックし、 **レポートのアクション** > **編集**.

      たとえば、表示、フィルタ、グループ化、プロンプト、またはグラフやコピーしたレポートを編集できます。

   * コピーしたレポートの権限を回復するには、新しいダッシュボードでレポート名をクリックし、 **レポートのアクション** > **共有** レポートの権限を更新します。

      ダッシュボードのコピー中にレポートをコピーすると、そのレポートに対する権限は削除されます。

   * 「情報のアクセス権を使用してこのレポートを実行する」を変更するには、新しいダッシュボードでレポートの名前をクリックし、 **レポートのアクション** > **編集** > **レポートのオプション**.\
      レポートをコピーした後、次の状況でのみ、「アクセス権限を持つこのレポートを実行」権限が維持されます。

      （これらの条件がいずれも true でない場合、「アクセス権限を持つこのレポートを実行する」権限は削除され、新しい「アクセス権を持つこのレポートを実行する」がコピーしたレポートを作成したユーザーに変更されます）。

      ダッシュボードとそのレポートをコピーするユーザーが管理者アクセス権を持っている場合。

      * ダッシュボードとそのレポートをコピーするユーザーが管理者アクセス権を持っている場合。
      * ダッシュボードとそのレポートをコピーするユーザーが、現在、コピーするレポートのアクセス権を持つ「このレポートを実行」として設定されている場合。
      * レポートをコピーするユーザーがレポートに対する管理権限を持っている場合。
