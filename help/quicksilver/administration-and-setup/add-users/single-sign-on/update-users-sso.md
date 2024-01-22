---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: シングルサインオンのユーザーを更新する
description: Workfrontでのシングルサインオン用にユーザーを更新できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: e4cd543aa9f47e6b93aa148ea3fb972fbd356c02
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 1%

---

# シングルサインオンのユーザーを更新する

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Adobe Workfrontインスタンスでシングルサインオン (SSO) が有効になっている場合、ユーザーは SSO 資格情報を使用してWorkfrontにログインできます。

既に SSO 資格情報に関連付けられたユーザーが設定されている既存のシステムがある場合は、コンマ区切り値 (CSV) ファイルをWorkfrontにインポートすることで、ユーザーの ID をWorkfrontにインポートできます。

Workfrontと SSO システムの統合について詳しくは、 [Adobe Workfrontでのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td><p>新規：標準</p><p>または</p><p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## SSO ユーザ名

使用する SSO ソリューションに応じて、SSO 環境でのユーザー名を次のいずれかと呼び出すことができます。

* SSO ユーザー名
* 連合 ID
* フェデレーションユーザー名

SSO 環境で呼び出されるユーザー名に関係なく、フィールドの値は User オブジェクトの「SSO Username」フィールドに格納されます。

ユーザーが SSO 資格情報を使用してWorkfrontにログインできるようにするには、ユーザーのプロファイルを更新して、Workfrontユーザー名に加えて SSO ユーザー名を含める必要があります。

Workfront管理者は、Workfrontユーザーの SSO Username フィールドを一括で更新できます。そのためには、ユーザー名のリストをWorkfrontに読み込みます。 このリストは、次の条件を満たす必要があります。

* Workfrontユーザー ID(GUID) と、各ユーザーに対応する SSO ユーザー名を含めます
* CSV または TSV ファイルとして保存します。

このプロセスは、Workfrontの既存の SSO ユーザー名を更新するか、ユーザー名が見つからない場合は新しい SSO ユーザー名を追加します。

## インポートファイルを準備 {#prepare-the-import-file}

Workfrontで SSO ユーザー名フィールドを更新する必要があるすべてのユーザーのレポートを作成することで、インポートファイルの準備を開始できます。

1. Workfrontでユーザーレポートを作成します。

   Workfrontでユーザーレポートを作成する手順については、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. レポートの次のフィールドを選択します。

   | フィールド | 説明 |
   |---|---|
   | 名前 | Workfrontユーザーのフルネーム。 |
   | ID | ID はWorkfront英数字の GUID です。 |
   | SSO ユーザー名 | 「SSO ユーザー名」フィールドを追加して、インポートで上書きするユーザー名がないようにします。 ユーザーが SSO 用にまだ更新されていない場合、このフィールドはすべてのユーザーに対して空白にする必要があります。 |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. レポートを保存します。
1. クリック **書き出し** をクリックし、Excel にエクスポートします。
1. エクスポートした Excel ファイルを開き、「SSO ユーザー名」列のレポートで各ユーザーの SSO ユーザー名を追加します。

   >[!IMPORTANT]
   >
   >SSO ユーザー名では大文字と小文字が区別されます。

1. Excel ファイル内の、「 **ID** そして **SSO ユーザー名** 列。

1. 列ヘッダーを削除し、レポートの上部に空白の行がないことを確認します。

   SSO ユーザー名でWorkfrontユーザーを更新するために使用するファイル **必須** 次の順序で、列が 2 つだけ含まれます。

   * 最初の列には、Workfrontユーザー ID(Workfrontで見つかったユーザー GUID) を表示する必要があります。
   * 2 番目の列には、SSO システムに表示される SSO ユーザー名を含める必要があります。
   * 列にはヘッダーを含めず、名前のリストの先頭に空の行を含めることはできません。

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. レポートを CSV または TSV ファイルとしてコンピューターに保存します。

## SSO 用にユーザーを更新します {#update-your-users-for-sso}

SSO のユーザーを更新するプロセスでは、SSO Username フィールドが存在しない場合はWorkfrontユーザーに追加し、既にユーザーに関連付けられている値がある場合はそのフィールドの値を更新します。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅で、「 **設定** ![](assets/gear-icon-settings.png).

1. クリックして、 **システム** 次に、 **SSO のユーザーを更新**.

1. クリック **ファイルを選択** をクリックして、準備したファイルを参照します。

   このファイルの準備方法の詳細については、 [インポートファイルを準備](#prepare-the-import-file).

1. ファイルの保存先となるコンピューターを選択し、「 **開く**.

   これにより、SSO 資格情報がWorkfrontに挿入され、すべてのユーザーが SSO 資格情報を使用してWorkfrontにログインできるようになります。

   The **許可するのみ `<SSO Configuration>` 認証** の設定は、CSV に含まれるすべてのユーザーに対して有効になります。 これにより、ユーザーは SSO を使用してログインする必要があります。

## ユーザーのWorkfrontユーザー名に対する SSO の検証

SSO ユーザー名情報を含むユーザー・レポートの作成手順については、 [インポートファイルを準備](#prepare-the-import-file).

1. SSO ユーザー名情報を含むユーザーレポートを実行します。

   各ユーザーに対して SSO Username 列が設定されます。

1. SSO Username 列の値が SSO サーバー上の SSO Username と一致していることを確認します。
1. 「SSO Username」列が空白の場合は、ユーザーの SSO ユーザー名を更新します。

   ![](assets/users-with-sso-field-updated.png)

   SSO 用にユーザーを更新する手順については、 [SSO 用にユーザーを更新します](#update-your-users-for-sso).
