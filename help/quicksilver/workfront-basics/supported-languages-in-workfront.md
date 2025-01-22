---
content-type: reference
navigation-topic: get-started-with-workfront
title: Adobe Workfront でサポートされている言語
description: ブラウザーの言語設定と Workfront 内のデフォルトのメールロケールを調整することで、Adobe Workfront とWorkfront からのメールを表示する言語を変更できます。
feature: Get Started with Workfront
author: Nolan
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 72%

---

# Adobe Workfront でサポートされている言語

ブラウザー（IMS 上にない場合）またはAdobe Experience Cloud プロファイルの言語環境設定（IMS 上にある場合）およびWorkfront内のデフォルトのメールのロケールを調整することで、WorkfrontおよびAdobe Workfrontからのメールを表示する言語を変更できます。

Workfront の用語は、Workfront が更新されるたびに、サポート対象の言語に合わせて更新されます。

Workfront は、次の言語をサポートしています。

* 英語（en-US）
* フランス語（fr-FR）
* ドイツ語（de-DE）
* 日本語（ja）
* スペイン語（es）
* イタリア語（it_IT）
* ポルトガル語（pt-BR）
* 韓国語（ko）
* 中国語 - 簡体字（zh-CN）
*   中国語 - 繁体字（zh-TW）

ブラウザーでWorkfrontを表示する際に使用する言語は、組織が IMS に準拠していない場合はブラウザーの言語設定によって、組織が IMS に準拠していない場合はAdobe Experience Cloud プロファイル言語によって制御されます。 どちらの場合も、「サポートされる言語」リストに表示されている言語を選択していることを確認してください。

サポートされている言語のいずれかで送信メールを表示するには、Workfront のユーザーのメールロケールまたは顧客情報の設定を変更します。\
顧客情報の設定を変更するには、Workfront 管理者である必要があります。\
顧客情報とユーザーのメールロケールの変更について詳しくは、[Workfront とユーザーのメールロケールを変更](#change-the-workfront-and-user-locales)を参照してください。

サードパーティに契約して、Workfront インターフェイスと Workfront からの送信メールを他の言語に翻訳することができます。これらの翻訳は Workfront ではサポートされておらず、上記以外の言語はサポートされていません。

>[!NOTE]
>
>インターフェイスの一部は、次の場合に未翻訳になる可能性があります。
>
>* サポートされていない言語を使用している場合、インターフェイスは英語で表示されます
>* ヘルプメニューと、そのメニューからアクセスするヘルプコンテンツは、英語で表示されます
>* ユーザーが入力したテキストは、入力した元の言語のままです。これには、以下のものが含まれますが、これらに限定されません。
>
>   * プロジェクト名
>   * タスク名
>   * イシュー名
>   * ポートフォリオ名
>   * プログラム名
>   * 承認名
>   * 説明
>   * カスタムフォーム名
>   * 時間タイプ名
>   * 費用タイプ
>   * マイルストーン
>   * カスタムタブ
>   * ステータス
>   * レポート名
>

## プルーフを使用する際にサポートされる言語の不一致

Workfront 内の web プルーフビューアは、Workfront でサポートされているほとんどの言語をサポートしています。

次の言語は、プルーフツールではサポートされていません。

* 中国語 - 簡体字（zh-CN）
*   中国語 - 繁体字（zh-TW）
* ポルトガル語（pt-BR）

Web プルーフビューアにアクセスするには、会社がプルーフ用ライセンスを購入する必要があります。

プルーフについて詳しくは、[プルーフ](../review-and-approve-work/proofing/proofing.md)を参照してください。

Workfront をプルーフツールでサポートされていない言語で表示する場合、web プルーフビューアは英語で表示されます。

Workfront でサポートされていない言語で Workfront Proof（スタンドアロンプルーフツール）を使用する場合、Workfront 内の web プルーフビューアは英語で表示されます。\
Workfront Proof でサポートされる言語について詳しくは、[Workfront Proof の言語設定](../workfront-proof/wp-getstarted/system-information/language-settings.md)を参照してください。

## Adobe Workfront Fusion でサポートされている言語

現在、Workfront Fusion は英語のみをサポートしています。

* Workfront Fusion のすべてのコンテンツと、Workfront Fusion に関連するヘルプコンテンツは、英語で表示されます。
* Workfront Fusion では、ユーザー入力フィールドで英語以外のテキスト文字の使用はサポートされていません。

Workfront Fusion にアクセスするには、会社が Workfront Fusion ライセンスを購入している必要があります。\
Workfront Fusion について詳しくは、[Adobe Workfront Fusion の概要](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。

## 言語を変更

以下の設定を変更することで、Workfront を表示する言語と送信メールの言語を変更できます。

* ブラウザーの言語（IMS 以外のユーザー用）
* AEM プロファイルのプライマリおよびセカンダリ言語（IMS 上のユーザー用）
* Workfront アカウントの「顧客情報」および「ユーザーメールのロケール」設定。

選択した言語で使用可能なすべての翻訳を表示するには、Workfront のロケールとブラウザーのロケールの両方を同じ言語に設定する必要があります。

* [ブラウザーの言語の変更](#change-the-browser-language)
* [Adobe Experience Cloudの言語の変更](#change-the-adobe-experience-cloud-language)
* [Workfront とユーザーのメールロケールの変更](#change-the-workfront-and-user-locales)

### ブラウザーの言語の変更 {#change-the-browser-language}

組織が IMS 上にない場合、ブラウザーの言語を変更すると、Workfront インターフェイスはその言語で表示されます。\
Workfront でサポートされている言語について詳しくは、[Adobe Workfront でサポートされている言語](#supported-languages)を参照してください。

ブラウザーの言語は、個々のユーザー単位で変更する必要があります。

ブラウザーの言語を変更する方法について詳しくは、ブラウザーの「ヘルプ」メニューを参照してください。

### Adobe Experience Cloudの言語の変更

組織が IMS 上にある場合、Workfrontに表示される言語はAdobe Experience Cloud プロファイル言語によって決まります。

1. Adobe Experience Cloud ツールバーの右端にあるプロフィール写真をクリックし、「環境設定 **をクリックし** す。 Adobe Experience Cloud ツールバーは、メインのWorkfront ツールバーのすぐ上にあります。

1. **プロファイル** の下の自分の名前とメールアドレスの下で、現在選択されている言語の名前をクリックします。

1. ドロップダウンで優先言語 **第 1 言語** と **第 2 言語** を選択します。 第 1 言語はデフォルトの言語の選択ですが、第 2 言語は、第 1 言語が特定のアプリケーションでサポートされていない場合にのみ表示されます。

### Workfront とユーザーのメールロケールの変更 {#change-the-workfront-and-user-locales}

* [デフォルトの Workfront メールロケールを変更](#change-the-workfront-locale)
* [ユーザーのメールロケールを変更](#change-the-user-locale)

### デフォルトの Workfront メールロケールを変更 {#change-the-workfront-locale}

デフォルトの Workfront メールロケールを変更する場合は、すべての Workfront ユーザー向けに送信メッセージで使用される言語、日付、数値の形式を変更します。これらの設定は、作成するすべての新しいユーザーのデフォルトになります。

デフォルトの Workfront メールロケールを変更するには：

1. Workfront 管理者として Workfront にログインします。
1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. **システム**／**顧客情報**&#x200B;をクリックします。

1. 「**基本情報**」セクションで、**デフォルトのメールロケール**&#x200B;ドロップダウンリストをクリックして、Workfront のメールを表示する言語を選択します。

1. 「**保存**」をクリックします。

### ユーザーのメールロケールを変更 {#change-the-user-locale}

ユーザーのメールロケールを変更する場合は、送信メッセージで使用される言語、日付、数値の形式を変更します。これらの設定は、「設定」の「顧客情報」エリアで選択したシステム設定を上書きします。

>[!NOTE]
>
>組織がAdobe統合エクスペリエンスを使用している場合、言語環境設定はAdobeプロファイルに保存され、メールのロケールは使用されません。 この記事の [Adobe Experience Cloud言語の変更 ](#change-the-adobe-experience-cloud-language) を参照してください。

ユーザーのメールロケールを変更するには：

1. Adobe Workfront の右上隅で&#x200B;**メインメニュー**&#x200B;アイコン![](assets/main-menu-icon.png)、ユーザープロファイルの画像の順にクリックします。

1. その他メニュー![](assets/more-icon.png)、「**編集**」の順にクリックします。

1. 「**環境設定**」セクションで、**メールのロケール**&#x200B;ドロップダウンリストをクリックして、Workfront のメールを表示する言語を選択します。

1. 「**変更を保存**」をクリックします。
