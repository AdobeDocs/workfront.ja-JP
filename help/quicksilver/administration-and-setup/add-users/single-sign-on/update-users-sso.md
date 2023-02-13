---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: シングルサインオンのユーザーを更新
description: Workfrontでのシングルサインオン用にユーザーを更新できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# シングルサインオンのユーザーを更新

{{important-admin-console-onboard}}

Adobe Workfrontインスタンスでシングルサインオン (SSO) が有効になっている場合は、SSO 資格情報を使用してWorkfrontにログインできます。

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
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## SSO ユーザ名

使用する SSO ソリューションに応じて、SSO 環境でのユーザー名を次のいずれかと呼び出すことができます。

* SSO ユーザー名
* 連合 ID
* フェデレーションユーザー名

Workfrontでは、これらの名前はすべて、ユーザーオブジェクトの「SSO Username」フィールドに格納されます。

ユーザーが SSO 資格情報を使用してWorkfrontにログインできるようにするには、ユーザーのプロファイルを更新して、Workfrontユーザー名に加えて SSO ユーザー名を含める必要があります。

Workfront管理者は、Workfrontユーザーの「 SSO Username 」フィールドを一括で更新できます。そのためには、ユーザー名のリストを使用し、Workfrontに読み込みます。 このリストには、各ユーザーのWorkfrontユーザー ID(GUID) と対応する SSO ユーザー名が含まれている必要があり、CSV または TSV ファイルとして保存する必要があります。 このプロセスは、Workfrontの既存の SSO ユーザー名を更新するか、ユーザー名が見つからない場合は新しい SSO ユーザー名を追加します。

## インポートファイルを準備 {#prepare-the-import-file}

Workfrontで SSO ユーザー名フィールドを更新する必要があるすべてのユーザーのレポートを作成することで、インポートファイルの準備を開始できます。

1. Workfrontでユーザーレポートを作成します。

   Workfrontでユーザーレポートを作成する手順については、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. レポートの次のフィールドを選択します。

   | 名前 | Workfrontユーザーのフルネーム。 |
   |---|---|
   | ID | ID はWorkfront英数字の GUID です。 |
   | SSO ユーザー名 | 「 SSO ユーザー名」フィールドを選択して、インポートで上書きするユーザー名がないことを確認します。 ユーザーが SSO 用にまだ更新されていない場合、このフィールドはすべてのユーザーに対して空白にする必要があります。 |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. レポートを保存します。
1. クリック **書き出し** をクリックし、Excel にエクスポートします。
1. エクスポートした Excel ファイルを開き、「SSO ユーザー名」列のレポートで、各ユーザーの SSO ユーザー名の追加を開始します。

   >[!IMPORTANT]
   >
   >SSO ユーザー名では大文字と小文字が区別されます。

1. Excel ファイル内の、 **ID** そして **SSO ユーザー名** 列。

1. 列ヘッダーを削除し、レポートの上部に空白の行がないようにします。

   SSO ユーザー名でWorkfrontユーザーを更新するために使用するファイルには、次の順序で 2 列のみ含める必要があります。

   * 最初の列には、Workfrontユーザー ID(Workfrontで見つかったユーザー GUID) が表示されます。
   * 2 番目の列には、SSO システムに表示される SSO ユーザー名が含まれている必要があります。
   * 列にはヘッダーを含めず、名前のリストの先頭に空の行を含めないでください。

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. レポートを CSV または TSV ファイルとしてコンピューターに保存します。

## SSO 用にユーザーを更新します {#update-your-users-for-sso}

SSO のユーザーを更新するプロセスでは、SSO ユーザー名フィールドが存在しない場合はWorkfrontユーザーに追加し、既にユーザーに関連付けられている値がある場合はそのフィールドの値を更新します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** その後 **SSO のユーザーを更新**.

1. クリック **ファイルを選択** をクリックして、準備したファイルを参照します。

   このファイルの準備方法の詳細については、 [インポートファイルを準備](#prepare-the-import-file).

1. コンピューター上のファイルを選択し、「 **開く**.

   これにより、すべてのユーザーが SSO 資格情報を使用してWorkfrontにログインできるようになります。

   この **許可する `<SSO Configuration>` 認証** の設定は、CSV に含まれるすべてのユーザーに対して有効になります。

## ユーザーのWorkfrontユーザー名 SSO を検証します

SSO ユーザー名情報を含むユーザー・レポートの作成手順については、 [インポートファイルを準備](#prepare-the-import-file).

1. SSO ユーザー名情報を含むユーザーレポートを実行します。

   各ユーザーに対して SSO Username 列が設定されます。

1. SSO Username 列の値が SSO サーバー上の SSO Username と一致していることを確認します。
1. 「SSO Username」列が空白の場合は、ユーザーの SSO ユーザー名を更新します。

   ![](assets/users-with-sso-field-updated.png)

   SSO 用にユーザーを更新する手順については、 [SSO 用にユーザーを更新します](#update-your-users-for-sso).
