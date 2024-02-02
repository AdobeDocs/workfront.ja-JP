---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe Unified Experience の FAQ
description: ' [!DNL Workfront]  および Adobe Experience Cloud の間にはいくつかの機能には違いがあり、 [!DNL Workfront]  インスタンスは統合エクスペリエンスに移行されるため、お客様の疑問をお答えします。'
author: Lisa
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: ht
source-wordcount: '1265'
ht-degree: 100%

---

# [!DNL Adobe Unified Experience] の FAQ

[!DNL Workfront] の [!DNL Adobe Unified Experience] を使用すると、[!DNL Adobe] アプリケーションのすべてを 1 回のログインで 1 か所で管理できます。[!DNL Adobe] ナビゲーションエリアは、[!DNL Workfront] とシームレスに統合されています。いくつかの機能には違いがあり、[!DNL Workfront] インスタンスは統合エクスペリエンスに移行されるため、お客様の疑問にお答えします。

[!DNL Adobe Unified Experience] にログインする方法について詳しくは、 [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) の [[!DNL Adobe Unified Experience]  を参照してください。.

## [!DNL Adobe Unified Experience] および [!DNL Workfront only] エクスペリエンスの比較

[!DNL Adobe Business Platform]／[!DNL Adobe Admin Console] を使用している顧客に限り [!DNL Adobe Unified Experience] にアクセスできます。まだ移行していないお客様には、[!DNL Adobe] アプリケーション間の切り替え機能はなく、[!DNL Workfront only] エクスペリエンスが表示されます。

次の表に、2 つのエクスペリエンスの違いを示します。

| [!DNL Adobe Unified Experience] | [!DNL Workfront] のみのエクスペリエンス |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] メインメニュー] は![メインメニュー](assets/main-menu-icon-left-nav.png)の左側にあります | [!UICONTROL [!DNL Workfront] メインメニュー] は![メインメニュー](assets/main-menu-icon.png)の右側にあります |
| すべての [!DNL Adobe Experience Cloud] アプリで 1 回ログイン URL が利用可能 | カスタム [!DNL Workfront] URL で [!DNL Workfront] へのログイン |
| 「組織の切り替え」の使用で [!DNL Workfront] 組織と環境間を移動可能 | 「組織の切り替え」は使用できません。 |
| ナビゲーションには、[!DNL Workfront] ナビゲーションバーに加えて、[!DNL Adobe] 製品、[!DNL Adobe] 通知、ヘルプおよびユーザープロファイルの最上位ナビゲーションエリアを含みます。 | ナビゲーションは [!DNL Workfront] ナビゲーションバーのみを含みます |
| ヘルプは、[!UICONTROL メインメニュー]および上部ナビゲーションエリアを介してアクセスします | ヘルプは、[!UICONTROL メインメニュー]および [!DNL Workfront] ナビゲーションバーを介してアクセスします |

{style="table-layout:auto"}

## よくある質問

**[!DNL Adobe Admin Console]?** について詳しく学ぶには。

[!DNL Admin Console] について詳しくは、次の記事を確認します。

* [ [!DNL Adobe Admin Console] の準備](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [プラットフォームベースの管理上の違い（[!DNL Adobe Workfront]／[!DNL Adobe Business Platform]）](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] の概要](https://helpx.adobe.com/jp/enterprise/using/admin-console.html)

**移行を促すために顧客として行うべきことを教えてください。**

既存のお客様には、移行のスケジュールするためにご連絡させていただきます。移行チームのサポート員からお客様にプロセスを説明し、できるだけ簡単で手間のかからない移行を行うために、[!DNL Admin Console] の設定についてアドバイスおよび移行に必要なドキュメントへのリンクを提供します。

* [[!DNL Adobe Workfront] サポートの概要](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html?lang=ja)
* [[!DNL Workfront Admin Console] 情報](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html?lang=ja)
* [[!DNL Adobe Business Platform] and [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html?lang=ja)

**[!DNL Workfront] SSO 設定とは異なる Federated ID に対して既にこれを有効にしている会社の [!DNL Adobe Admin Console] にはどのように対処しますか？**

[!DNL Adobe Admin Console] には、[!DNL Workfront] を含めるオプションがあり、SSO を IMS に置き換えます。すべてのユーザープロビジョニングは [!DNL Admin Console] で実行され、ユーザーには [!DNL Adobe] ログイン画面が表示され、[!DNL Experience Cloud] に移動すると [!DNL Workfront] がオプションとして（アクセス権が付与されている場合）表示されます。

**[!DNL Adobe Assets] の AEM 管理パネルを既に持っているが、SSO は[!DNL Workfront?]** とは異なる設定である場合、どのような影響がありますか？

[!DNL Workfront] が [!DNL Admin Console] アプリケーションとして追加されると、[!DNL Adobe Assets] の既存の SSO 設定を活用するには、[!DNL Workfront] に対して他に操作をする必要はありません。

**これは SSO で設定されたものに対してどのような影響を与えますか？**

SSO は [!DNL Admin Console] で設定され、[!DNL Workfront] アプリケーションによって継承されます。

**内部の [!DNL Active Directory] との SSO は IMS と併用するオプションになるのでしょうか？**

IMS は SSO の代わるもので、ほとんど同じ機能です。すべてのユーザー権限は、[!DNL Adobe Admin Console] で付与され、プロビジョニングされます。ユーザーは、[!DNL Adobe] ログイン画面で「[!UICONTROL 個人用アカウント]」または「[!UICONTROL 会社アカウント]」を選択します（[!DNL Active Directory] がある場合、ほとんどの場合は、会社アカウントでログインします）。

**SSO を使用していない場合は、[!DNL Workfront] ログイン URL に変更はありますか？**

ログイン URL は変更されますが、古い URL は新しいログイン URL にリダイレクトされます。再度ユーザーに移動先を伝える必要があります。

**設定したエイリアスはまだ機能しますか、またはこの移行に伴って、[!DNL Workfront] リンクに変更はありますか？**

[!DNL Workfront] のリダイレクトやエイリアスを使用して、ホームページにアクセスできます。

**リダイレクトが無効になる場合はありますか？それとも、常に my.company.workfront.com で入力できますか？**

いつでも任意のカスタム URL を使用できます。任意のリンクをクリックすると [!DNL Workfront] に誘導され、別の URL が表示されます。ただし、 experience.adobe.com にログインし、[!DNL Experience Cloud] 内からリンクをブックマークする方が良い [!DNL experience] です。リダイレクトが速いと、遅延時間や読み込み時間も短くなります。

**リクエストキューへの直接リンクは壊れますか？**

すべての直接リンクは、新しい URL パターンにリダイレクトする必要があります。ただし、リンクをユーザーに配布している場合は、直接リンクを利用するためにアップデートを送信し、想定されるページにアクセスする際の遅延を防ぐ必要があります。

**[!DNL Experience Cloud] にすべてのユーザーが移行されますか？それとも特定のユーザー（すべてのユーザーが他の Adobe 製品を使用しているわけではない）のみを選択できますか？**

[!DNL Workfront] の顧客アカウント全体が移行されます。ユーザー単位で移行することはできません。

**すべての [!DNL Workfront] ユーザーが [!DNL Experience Cloud] 経由でログインする必要がありますか。それとも管理者だけですか。**

はい、すべてのユーザーが [!DNL Experience Cloud] 経由でログインします。SSO は IMS ログインに置き換えられます。ログイン画面が異なるだけで、エクスペリエンスは非常に似ています。

**ユーザーがすでに [!DNL Adobe] アカウントと [!DNL Workfront] アカウントの両方を持っている場合は、これらのアカウントをリンクする必要がありますか？**

はい、そのための手順が用意されており、組織が IMS に移行する準備ができた時点で、詳細が提供されます。

**[!DNL Adobe] アカウントを持たない [!DNL Workfront] ユーザーはどうなりますか？**

[!DNL Workfront] にアクセスするための権限が [!DNL Adobe Admin Console] で付与されていないユーザーがログインするには、「[!UICONTROL 個人アカウント]」または [!DNL Adobe] ID アカウントを作成する必要があります。これにより、リクエストを承認または拒否するためのメールが管理者に送信され、ユーザーが持つアクセス権のタイプを管理者が設定できるようになります。ログインして experience.adobe.com に移動し、メールアドレスを入力して「[!UICONTROL 個人アカウント]」を選択します。ここから、[!DNL Workfront] にアクセスできるようになります。

**[!DNL Workfront?]** 以外の [!DNL Adobe] 製品を利用していない場合はどうなりますか？

組織を [!DNL Adobe Unified Experience] に移行することを、引き続きお勧めします。上記のメリットとともに [!DNL Adobe] ID を入手していただけます。

**[!DNL Workfront] インスタンスに外部ユーザーが含まれています。[!DNL Adobe] に含まれる他の製品に外部ユーザーがアクセスできるのは望ましくありません。コンソールでアクセスをどのように制限できますか？**

管理者は [!DNL Admin Console] で、ユーザーによるアクセスの範囲をきめ細かく制御できます。外部ユーザーがアクセス必要をとする場合は、その都度 [!DNL Adobe] ID を作成する必要があり、これによって管理者にメールが送信されます。管理者は、製品へのアクセスを承認または却下し、組織が所有する製品に対してアクセスできるものとできないものを定義します。さらに [!DNL Workfront] システム管理者は [!DNL Workfront] の [!UICONTROL ユーザー]エリアに移動して、外部ユーザーに対してさらに細分化された権限を付与することができます。

**グループ管理者は、[!DNL Workfront] でユーザーを作成するために使用されます。[!DNL Experience Cloud] に移行しても、グループ管理者は引き続きユーザーを作成できますか？**

はい、[!DNL Workfront] からユーザーを作成することができます。これらのユーザーは、自動的に [!DNL Experience Cloud] に追加されます。[!DNL Admin Console] でグループ管理者を製品所有者として設定し、ユーザーへの [!DNL Workfront] の割り当てを許可することもできます。

**[!DNL Experience Cloud] に切り替える期限はいつですか？**

現在、[!DNL Adobe Experience Cloud] への移行に期限はありません。準備が整った時点で移行できるよう、お客様をサポートいたします。

**この変更に関して、サポートチームに必要なことはありますか？**

サポートチームがユーザーの新規作成を担当している場合は、ユーザーの作成と Workfront への資格の割り当てに使用される [!DNL Admin Console] のインターフェイスに慣れていただく必要があります。それ例外には、社内のサポートチームに大きな変更は発生しないでしょう。

**これは、API 機能を介した統合にどのような影響を与えますか？**

既存の URL パスは、引き続き API トラフィックで使用できます。統合内のエンドポイントは、何も対応しなくても更新されます。ただし、ユーザー名とパスワードを使用した直接ログインはサポートされません。API キーを使用する必要があります（[!DNL Workfront Fusion] コネクタは例外）。

**[!DNL Creative Cloud] ユーザーについてはどうですか。移行が及ぼす影響はありますか。ユーザーには何か利点がありますか。**

[!DNL Adobe Unified Experience] に移行しても [!DNL Creative Cloud] ユーザーへの影響はありません。

**[!DNL Workfront] モバイルユーザーのログインは変更されますか。**

[!DNL Workfront] モバイル ユーザーは [!DNL Adobe Unified Experience] への移行による影響を受けません。
