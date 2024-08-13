---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: シングルサインオンのユーザーの更新
description: Workfront でのシングルサインオン用にユーザーを更新できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 97%

---

# シングルサインオンに対応するためのユーザーの更新

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Adobe Workfront インスタンスでシングルサインオン（SSO）が有効になっている場合は、ユーザーは SSO 資格情報を使用して Workfront にログインできます。

既に SSO 資格情報に関連付けられたユーザーが設定されている既存のシステムがある場合は、コンマ区切り値（CSV）ファイルを Workfront に読み込むことで、Workfront にユーザーの ID を読み込むことができます。

Workfront と SSO システムの統合について詳しくは、[](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md) でのシングルサインオンの概要を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p><p>または</p><p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## SSO ユーザー名

使用する SSO ソリューションに応じて、SSO 環境でのユーザー名を次のいずれかに名づけることができます。

* SSO ユーザー名
* フェデレーション ID
* フェデレーションユーザー名

SSO 環境で呼ばれるユーザー名に関係なく、フィールドの値はユーザーオブジェクトの「SSO ユーザー名」フィールドに格納されます。

ユーザーが SSO 資格情報を使用して Workfront にログインできるようにするには、ユーザーのプロファイルを更新して、Workfront ユーザー名に加えて SSO ユーザー名を含める必要があります。

Workfront 管理者は、ユーザー名のリストを Workfront に読み込むことで、Workfront ユーザーの「SSO ユーザー名」フィールドを一括で更新できます。このリストは、次の条件を満たす必要があります。

* Workfront ユーザー ID（GUID）と、各ユーザーに対応する SSO ユーザー名を含める
* CSV または TSV ファイルとして保存

このプロセスは、Workfront の既存の SSO ユーザー名を更新するか、ユーザー名が見つからない場合は新しい SSO ユーザー名を追加します。

## 読み込みファイルの準備 {#prepare-the-import-file}

Workfront で SSO ユーザー名フィールドを更新する必要があるすべてのユーザーのレポートを作成することで、読み込みファイルの準備を開始できます。

1. Workfront でユーザーレポートを作成します。

   Workfront でユーザーレポートを作成する手順については、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

1. レポートの次のフィールドを選択します。

   | フィールド | 説明 |
   |---|---|
   | 名前 | Workfront ユーザーのフルネーム。 |
   | ID | ID は Workfront の英数字の GUID です。 |
   | SSO ユーザー名 | 「SSO ユーザー名」フィールドを追加して、読み込みで上書きされるユーザー名がないことを確認します。ユーザーが SSO 用にまだ更新されていない場合、このフィールドはすべてのユーザーに対して空白です。 |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. レポートを保存します。
1. リストの上部にある「**書き出し**」をクリックして、Excel にレポートを書き出します。
1. 書き出した Excel ファイルを開き、レポート内の各ユーザーの SSO ユーザー名を「SSO ユーザー名」列に追加します。

   >[!IMPORTANT]
   >
   >SSO ユーザー名では大文字と小文字が区別されます。

1. Excel ファイル内の「**ID**」列と「**SSO ユーザー名**」列を除くすべての列を削除します。

1. 列ヘッダーを削除し、レポートの上部に空白の行がないことを確認します。

   SSO ユーザー名で Workfront ユーザーを更新するために使用するファイルには、次の順序で 2 列のみを含める&#x200B;**必要があります**。

   * 最初の列には、Workfront ユーザー ID（Workfront にあるユーザー GUID）が表示される必要があります。
   * 2 番目の列には、SSO システムに表示される SSO ユーザー名を含める必要があります。
   * 列にはヘッダーを含めないようにし、また名前のリストの先頭に空の行を含めないようにします。

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. レポートを CSV または TSV ファイルとしてコンピューターに保存します。

## SSO 用にユーザーを更新 {#update-your-users-for-sso}

SSO 向けにユーザーを更新するプロセスでは、SSO ユーザー名フィールドが存在しない場合は Workfront ユーザーに追加し、既にユーザーに関連付けられている値がある場合はそのフィールドの値を更新します。

{{step-1-to-setup}}

1. **システム** をクリックし、「**SSO のユーザーを更新**」を選択します。

1. 「**ファイルを選択**」をクリックして、準備したファイルを選択します。

   このファイルの準備方法の詳細については、[読み込みファイルの準備](#prepare-the-import-file)を参照してください。

1. コンピューターに保存されているファイルを選択し、「**開く**」をクリックします。

   これにより、SSO 資格情報が Workfront に挿入され、すべてのユーザーが SSO 資格情報を使用して Workfront にログインできるようになります。

   CSV に含まれるすべてのユーザーに対して、「**`<SSO Configuration>` 認証のみを許可**」設定が有効になります。これにより、ユーザーは SSO を使用してログインする必要があります。

## ユーザーの Workfront ユーザー名に対する SSO の検証

SSO ユーザー名情報を含むユーザーレポートの作成手順については、[読み込みファイルの準備](#prepare-the-import-file)を参照してください。

1. SSO ユーザー名情報を含むユーザーレポートを実行します。

   各ユーザーに対して「SSO ユーザー名」列が設定されます。

1. 「SSO ユーザー名」列の値が SSO サーバー上の「SSO ユーザー名」と一致していることを確認します。
1. 「SSO ユーザー名」列が空白の場合は、ユーザーの SSO ユーザー名を更新します。

   ![](assets/users-with-sso-field-updated.png)

   SSO 用にユーザーを更新する手順については、[SSO 用にユーザーを更新](#update-your-users-for-sso)を参照してください。
