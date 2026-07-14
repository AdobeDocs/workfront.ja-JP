---
product-area: documents;workfront-integrations;system-administration
navigation-topic: adobe-cloud-drive
title: Adobe Cloud Driveの設定と管理
description: 管理者は、組織にAdobe Cloud Driveを設定し、ユーザーデバイスにデプロイし、Adobe Admin Consoleで継続的なアクセスを管理できます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps, System Setup and Administration
role: Admin
source-git-commit: f1dd9555df2adcf8a1afc48982bc2d52a14df54f
workflow-type: tm+mt
source-wordcount: '3139'
ht-degree: 2%

---

# Adobe Cloud Driveの設定と管理

管理者は、macOSのFinderとWindowsのFile Explorerを使用して、Adobe Cloud Driveを設定し、Adobe クラウドストレージ内のプロジェクトファイルにデスクトップから直接アクセスできるようにすることができます。 この記事では、Adobe Admin Consoleでアクセスを有効にし、アプリケーションをユーザーデバイスにデプロイし、継続的にアクセスを管理する方法について説明します。

Adobe Cloud Driveは、ユーザーのMacおよびWindows コンピューター上にWorkfront ドキュメントを仮想ドライブとしてAdobe クラウドストレージにマウントするエンタープライズデスクトップアプリケーションです。 インストール後、ユーザーはFinderまたはファイルエクスプローラーでWorkfront プロジェクトフォルダーを確認し、ファイルを手動でダウンロードしたり、ブラウザーで作業したりすることなく、任意のデスクトップアプリケーションを使用してプロジェクトファイルを開いたり、編集したり、保存したりできます。

Adobe Cloud Driveを使用するには、Adobe クラウドストレージが有効になっているWorkflow Ultimate パッケージを組織で使用する必要があります。

Adobe Cloud Driveについて詳しくは、次の記事を参照してください。

* [Adobe Cloud Driveの概要](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)
* [Adobe Cloud Driveのインストール](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)
* [Adobe Cloud Driveの使用](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront版</td> 
   <td>Adobe クラウドストレージが有効になっているWorkflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アドビ管理者権限</td> 
   <td>Adobe Admin ConsoleのWorkfrontのシステム管理者である必要があります</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Adobe Admin ConsoleでのAdobe Cloud Driveへのアクセス権の割り当て

Adobe クラウドストレージが有効になっている場合、Adobe Cloud DriveはWorkflow Ultimate パッケージに含まれます。 Admin Consoleの&#x200B;**製品** セクションにスタンドアロン製品として表示されません。 代わりに、**ユーザー**&#x200B;の&#x200B;**役割** セクションを通じて管理されます。

**Users** > **Roles**&#x200B;に移動すると、Workfront製品に関連付けられている2つの役割が表示されます。

| 役割 | 自動割り当て先 | Adobe Cloud Driveとの関連性 |
| --- | --- | --- |
| **メンバー** | 組織内のすべてのユーザー | 組織レベルのAdobe Cloud Drive機能スイッチが含まれています。 デフォルトではオンです。 |
| **ACD ユーザー** | デフォルトでは誰もいません | 組織レベルのスイッチがオフの場合、個々のアクセス権を付与します。 |

![Admin Consoleの役割](assets/admin-console-roles.png)

### アクセス制御

**コントロール 1：組織レベルの機能制御（メンバーロール内）**

**メンバー**&#x200B;の役割は、組織内のすべてのユーザーに自動的に割り当てられます。 このロール内には、**Adobe Cloud Drive**&#x200B;機能スイッチがあります。 このスイッチをオンにすると、Workflow Ultimate ライセンスを持つすべてのユーザーがAdobe Cloud Driveにアクセスできるようになります。 オフの場合、ライセンスに関係なく、Adobe Cloud Driveにアクセスすることはできません。

Adobeが組織のAdobe Cloud Driveをアクティブ化すると、デフォルトでスイッチがオンになります。

**コントロール 2: ACD ユーザーの役割**

**ACD ユーザー**&#x200B;の役割は、組織レベルのスイッチがオフの場合にのみ関連します。 組織レベルのスイッチをオフにして制御されたパイロットを実行する場合でも、**ACD ユーザー**&#x200B;の役割にユーザーを追加することで、特定のユーザーにアクセス権を付与できます。 このロールのユーザーは、組織レベルのスイッチがオフになっている場合でも、Adobe Cloud Driveにアクセスできます。 組織レベルのスイッチがオンの場合、**ACD ユーザー**&#x200B;の役割は無効です。

**基本的な要件：ワークフローUltimate ライセンス**

Adobe Cloud Driveは、Workflow Ultimate パッケージでのみ使用できます。 役割オプションは、他のパッケージでは使用できません。

Workflow Ultimate パッケージ内のライセンスは、Standard、Light、Contributorのいずれかのライセンスタイプにすることができます。 ライセンスについて詳しくは、[ ライセンスの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)を参照してください。

次の表は、これらのコントロールがどのように相互作用するかを示しています。

| 組織レベルスイッチ | ACD ユーザーの役割のユーザー | Workflow Ultimate ライセンス | アクセス結果 |
| --- | --- | --- | --- |
| オン | 任意 | はい | 付与 |
| オフ | はい | はい | 付与 |
| オフ | いいえ | はい | Denied |
| どちらか | どちらか | いいえ | Denied |

<!-- Sarah said to delete the second line. Commenting it out within the table messed up the display for the rest of the table, so keeping the line here until I can delete it. | On | Not required | No | Denied | -->

## 前提条件

開始する前に、次の点を確認してください。

* プロビジョニングするユーザーには、Workfront Workflow ライセンスが割り当てられています。
* IT チームとの[ ネットワーク要件](#network-requirements)を確認しました。
* Adobe Cloud Driveが示す内容（Workfront プロジェクトアセットのみ）とインストール方法についてユーザーに説明するコミュニケーションを作成しました。

  >[!NOTE]
  >
  >アクセスが有効になっているが、Workfront プロジェクトにアクセスできないユーザーは、ログイン後に空のマウントされたドライブを見ることができます。 今期待されているものです。 Workfront プロジェクトへのアクセスは、Workfrontでは個別に管理されます。 詳しくは、[ プロジェクトの共有](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。
  >
  >また、プロジェクトをドライブに表示するには、Creative Cloudの使用権限がWorkfrontと同じIMS組織にある必要があります。

## Adobe Admin Consoleでのアクセス権の設定

Adobe Cloud Driveへのアクセスは、Adobe Admin Consoleで設定されます。 ロールアウト戦略に合ったオプションを選択します。

### オプション A：組織全体のアクセスを有効にする

Adobeが組織のAdobe Cloud Driveをアクティブ化すると、組織レベルの機能スイッチがデフォルトでオンになり、すべてのユーザーがすぐにアクセスできるようになります。 アプリケーションをデプロイする前に、スイッチがオンになっていることを確認するには、次の手順を実行します。

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)にログインします。
1. 上部のナビゲーションバーで「**ユーザー**」をクリックします。
1. 左側のパネルで「**役割**」をクリックします。
1. 役割リストの&#x200B;**メンバー**&#x200B;をクリックします。
1. 右側に表示される&#x200B;**メンバー** パネルで、**権限**&#x200B;の下に&#x200B;**Adobe Cloud Drive**&#x200B;が表示され、そのスイッチがオンになっていることを確認します。

   Adobe Cloud Driveがオンになっている![ メンバーの役割の詳細パネル ](assets/member-permissions.png)

   >[!NOTE]
   >
   >Adobe Cloud Driveが&#x200B;**メンバー**&#x200B;の役割の&#x200B;**権限**&#x200B;の下に表示されない場合、Adobe Cloud Driveは組織に対してまだアクティブ化されていない可能性があります。 Adobe サポートにお問い合わせください。

1. 変更を加えた場合は、**保存**&#x200B;をクリックします。

### オプション B：特定のユーザーグループのアクセスを有効にする

このオプションは、より広範なロールアウトの前に試験運用を行う場合など、定義されたユーザーのセットへのアクセスを制限する場合に使用します。 これには、組織レベルのスイッチをオフにし、パイロットユーザーを&#x200B;**ACD ユーザー**&#x200B;の役割に追加することが含まれます。

>[!IMPORTANT]
>
>組織レベルのスイッチをオフにすると、現在ログインしているユーザーを含む、組織内のすべてのユーザーのAdobe Cloud Drive アクセスが即座に削除されます。 組織レベルの機能をオフにして、同じセッションにパイロットユーザーを追加する必要があります。

組織レベルの機能をオフにするには：

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)にログインします。
1. 上部のナビゲーションバーの&#x200B;**ユーザー**&#x200B;をクリックし、左側のパネルの&#x200B;**役割**&#x200B;をクリックします。
1. 役割リストの&#x200B;**メンバー**&#x200B;をクリックします。
1. **メンバー** パネルで、**権限**&#x200B;の下の&#x200B;**Adobe Cloud Drive**&#x200B;を見つけてオフにします。
1. 「**保存**」をクリックします。

ACD ユーザーロールにパイロットユーザーを追加するには：

1. 左側のパネルで「**役割**」をクリックして、役割リストに戻ります。
1. 役割リストで「**ACD user**」をクリックします。

   ![ACD ユーザー詳細パネル ](assets/acd-user-panel.png)

1. 「**ユーザーを追加**」をクリックします。
1. 各パイロットユーザーのメールアドレスを入力します。
1. 「**保存**」をクリックします。

   **ACD ユーザー**&#x200B;の役割に追加されたユーザーは、すぐにアクセスできます。 この役割に属していないユーザーは、役割に追加するか、組織レベルのスイッチをオンに戻すまで、アクセス権がありません。

   >[!TIP]
   >
   >時間の経過とともにアクセスを拡大するには、**ACD ユーザー**&#x200B;の役割に戻り、必要に応じてユーザーを追加します。 完全なロールアウトの準備ができたら、組織レベルのスイッチを&#x200B;**メンバー**&#x200B;の役割でオンに戻します。 組織レベルのスイッチがオンになると、**ACD ユーザー**&#x200B;の役割は影響を受けず、維持する必要はありません。

## Adobe Cloud Drive アプリケーションのデプロイ

Adobe Admin Consoleでアクセス権を設定すると、使用権限が確立されます。 アプリケーションをデプロイすると、ユーザーのデバイスにインストールされます。 これらは2つの独立した必要なステップです。

Adobe Cloud Driveはスタンドアロンアプリケーションです。 Creative Cloud デスクトップアプリケーションを通じて配布されず、Creative Cloud パッケージマネージャーにも表示されません。 ただし、Adobe Cloud Driveのユーザープロファイルは、Creative Cloud アプリの使用権限に関連付けられています。 つまり、ユーザーがドライブ内のWorkfront プロジェクトにアクセスするには、Creative Cloud アプリケーションにWorkfrontと同じIMS組織で権限を付与する必要があります。

組織のデバイス管理方法に合ったデプロイメント方法を選択します。

### 方法A: Admin Console パッケージを使用したIT管理デプロイメント

この方法は、Microsoft Intune、SCCM、Jamf Pro、Apple Remote Desktopなどの一元的なデプロイメントツールを使用している場合に使用します。 これは、Adobe エンタープライズ版の標準的なデプロイメントワークフローであり、他のAdobe アプリケーションで使用されるものと同じパッケージ作成プロセスに従います。

Adobe Admin Consoleでパッケージを作成するには：

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)にログインします。
1. 上部のナビゲーションバーで「**パッケージ**」をクリックします。
1. 左側のパネルで「**事前生成パッケージ**」をクリックします。
1. 「**テンプレート**」タブをクリックします。

   Adobe Cloud Driveがテンプレートリストに2回表示されます。macOSは1回、Windowsは1回です。

   ![事前生成されたパッケージテンプレート ](assets/pre-generated-packages.png)

1. 対象のプラットフォームに一致する&#x200B;**Adobe Cloud Drive**&#x200B;行を見つけ、その行の詳細アイコンをクリックします。

   サイドパネルには、パッケージメタデータが表示されます。

   ![ パッケージの詳細とメタデータ ](assets/template-details-and-metadata.png)

1. 「**カスタマイズ**」をクリックします。

   パッケージカスタマイズウィザードが開き、**Configure**、**アプリの選択**、**Options**、および&#x200B;**Finalize**&#x200B;の4つの手順が実行されます。

1. **Configure**&#x200B;手順で、ターゲットマシンのアーキテクチャを選択し、言語設定を確認して、**Next**&#x200B;をクリックします。

   * **macOS:** **macOS （Intel）**&#x200B;または&#x200B;**macOS （Apple Silicon）**&#x200B;を選択します。
   * **Windows:** **Windows （64 ビット）**&#x200B;または&#x200B;**Windows （ARM）**&#x200B;を選択します。

   ![ パッケージウィザードの手順の設定](assets/configure-step-in-wizard.png)

1. **アプリを選択**&#x200B;手順で、Adobe Cloud Driveが必要なバージョンで選択されていることを確認します。

   Adobe Cloud Driveは、利用可能な最新バージョンで事前に選択されています。 古いバージョンを使用するには、**その他のバージョン**&#x200B;をクリックし、**古いバージョン**&#x200B;を選択します。

   ![ パッケージウィザードでアプリの手順を選択](assets/choose-apps-step-in-wizard.png)

1. 「**次へ**」をクリックします。
1. **オプション** ステップで、オプションを選択せずに&#x200B;**次へ**&#x200B;をクリックします。

   これらの設定はCreative Cloud デスクトップアプリケーションに適用され、Adobe Cloud Driveには適用されません。

   ![ パッケージウィザードのオプション手順](assets/options-step-in-wizard.png)

1. **最終版**&#x200B;の手順で、パッケージの名前を入力し、**フラットパッケージ**&#x200B;を選択します。
1. 概要を確認し、**パッケージを作成**&#x200B;をクリックします。

   ![ パッケージウィザードで手順を最終決定](assets/finalize-step-in-wizard.png)

   ウィザードが閉じます。 新しいパッケージは、ビルド中に&#x200B;**準備中** ステータスでパッケージリストの上部に表示されます。 準備が整うと、ステータスが&#x200B;**最新**&#x200B;に変更され、ダウンロードリンクが表示されます。

   ![準備中のパッケージ ](assets/package-is-preparing.png)

1. 「**ダウンロード**」をクリックし、選択した場所にパッケージファイルを保存します。

### 方法B：ソフトウェア配布からのセルフサービスの直接ダウンロード

この方法は、小規模な組織の場合、自己管理デバイスの場合、または個々のユーザーにアプリケーションを自分でインストールするように指示する場合に使用します。

開始する前に、次の点を確認してください。

* Adobe Admin Consoleのユーザーに対してアクセスが有効になっています。
* ソフトウェア配布URLとログイン手順がユーザーに通知されました。
* 必要なエンドポイントへのネットワーク接続が検証されました。 詳しくは、この記事の「[ ネットワーク要件](#network-requirements)」を参照してください。

Adobe Cloud Driveをセルフインストールするには：

1. Adobe Admin Consoleでユーザーのアクセスが有効になっていることを確認します。
1. ユーザーを[experience.adobe.com/#/downloads](https://experience.adobe.com/#/downloads)に誘導します。

   >[!NOTE]
   >
   >Adobe Cloud Drive インストーラーを表示するには、Adobe Admin ConsoleでAdobe Cloud Drive アクセスを有効にする必要があります。 アクセス権を持たないユーザーには、インストーラーが表示されません。

1. ユーザーは、Enterprise IDまたはFederated IDでログインします。 Adobe Cloud Drive インストーラーは、「ソフトウェア配布」の「**Workfront**」タブに表示されます。
1. ユーザーはプラットフォームのインストーラーをダウンロードし、[Adobe Cloud Driveのインストール ](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)のインストール手順に従います。

   ![Workfront用Adobe Cloud Drive インストーラー](assets/wf-downloads.png)

デプロイ後、テストデバイスでこの検証を完了します。

1. **アプリケーション** フォルダー（macOS）または&#x200B;**開始** メニュー（Windows）からAdobe Cloud Driveを起動します。
1. Adobe Admin ConsoleでAdobe Cloud Drive アクセスが有効になっているユーザーアカウントでログインします。
1. Finderまたはファイルエクスプローラーで、マウントされたドライブにWorkfront プロジェクトフォルダーが表示されることを確認します。

   >[!NOTE]
   >
   >正常にログインしたが、フォルダーが表示されないユーザーは、Workfront プロジェクトにアクセスできません。 Workfrontのプロジェクトにユーザーを追加して、ドライブにデータを入力します。

1. プロジェクトフォルダーに移動し、小さなテストファイルを作成します。
1. ブラウザーでWorkfrontを開き、テストファイルが対応するプロジェクトに表示されていることを確認します。
1. 検証後にテストファイルを削除します。

## Adobe Cloud Driveへの継続的なユーザーアクセスを管理する

Adobe Cloud Driveを使用したら、次の手順に従って新しいユーザーを追加するか、アクセスする必要がなくなったユーザーを削除します。

### 新規ユーザーの追加

組織レベルのスイッチがオンの場合、Adobe Admin Consoleの操作は必要ありません。 Adobe Cloud Driveのダウンロードとインストールをユーザーに依頼します。 ライセンスを取得したユーザーが引き続きAdobe Cloud Driveにアクセスできない場合は、Adobe サポートに連絡して、アカウントが正しく移行されたことを確認してください。

組織レベルのスイッチがオフの場合：

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)にログインします。
1. 上部のナビゲーションバーの&#x200B;**ユーザー**&#x200B;をクリックし、左側のパネルの&#x200B;**役割**&#x200B;をクリックします。
1. 役割リストで「**ACD user**」をクリックします。
1. 「**ユーザーを追加**」をクリックし、ユーザーの電子メールアドレスを入力して、**保存**&#x200B;をクリックします。

### ユーザーの削除

組織レベルのスイッチがオンの場合、ライセンスを取得したユーザーは誰でもAdobe Cloud Driveにアクセスできます。 Workfront ライセンスを削除せずに特定のユーザーのアクセス権を削除するには、組織レベルのスイッチをオフにして、ブロックするユーザーを除く&#x200B;**ACD ユーザー** ロールに他のすべてのユーザーを追加します。

組織レベルのスイッチがオフで、ユーザーが&#x200B;**ACD ユーザー**&#x200B;の役割にある場合：

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)にログインします。
1. 上部のナビゲーションバーの&#x200B;**ユーザー**&#x200B;をクリックし、左側のパネルの&#x200B;**役割**&#x200B;をクリックします。
1. 役割リストで「**ACD user**」をクリックします。
1. ユーザーを選択し、**削除**&#x200B;をクリックします。

ユーザーは、マウントされたドライブに直ちにアクセスできなくなります。 Workfrontに保存されているファイルは削除されません。 ユーザーのローカルキャッシュは、アプリケーションをアンインストールするまでデバイス上に残ります。

>[!IMPORTANT]
>
>**ACD ユーザー**&#x200B;のロールからユーザーを削除しても、WorkfrontやWorkfront プロジェクトからユーザーが削除されることはありません。 Workfront プロジェクトへのアクセスを個別に管理できます。

## Workfront プロジェクトへのアクセスの管理

Adobe Cloud Driveは、ユーザーがアクセスできるWorkfront プロジェクトを表示します。 プロジェクトへのアクセスは、Adobe Admin ConsoleではなくWorkfrontで管理されます。 Adobe Cloud Driveへのアクセス権を持っているが、Workfront プロジェクトに属していないユーザーには、ログイン後に空のマウントされたドライブが表示されます。 これは予期される動作です。

プロジェクト アクセスの管理について詳しくは、[ プロジェクトの管理](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-overview.md)および[ プロジェクトの共有](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

## ネットワーク要件

Adobe Cloud Driveでは、Adobe エンドポイントのセットへのアウトバウンド HTTPS （ポート 443）アクセスが必要です。 インバウンドファイアウォールルールは必要ありません。 エンドポイントの一覧については、[Adobe ネットワークエンドポイント ](https://helpx.adobe.com/in/enterprise/kb/network-endpoints.html)を参照してください。

Adobe Cloud Driveは、macOSとWindowsの両方でシステムレベルのプロキシ設定を読み取ります。 認証済みプロキシはサポートされています。

## セキュリティに関する検討事項

### 認証

Adobe Cloud Driveは、Adobe IMS（Identity Management System）を介してユーザーを認証します。 Enterprise IDまたはFederated IDを使用してログインします。 組織がAdobe Admin Consoleで設定されたSSOを使用する場合、ユーザーはID プロバイダーを通じて認証を行い、Adobeの資格情報を個別に入力する必要はありません。

>[!NOTE]
>
>Adobe Cloud Driveは、エンタープライズ版デプロイメントで個人のAdobe ID （個別に作成され、管理されていないアカウント）をサポートしていません。 ユーザーは、組織のディレクトリでEnterprise IDまたはFederated IDを使用してログインする必要があります。

### 転送中および保存中のデータ

* Adobe Cloud DriveとAdobe サービス間のすべての通信では、TLS 1.2以降が使用されます。
* Adobe クラウドストレージに保存されたファイルは、保存時に暗号化されます。
* ローカルにキャッシュされたファイルは、デバイスでFileVault （macOS）またはBitLocker （Windows）が有効になっている場合に、OS レベルのディスク暗号化を使用します。

### ファイルアクセス制御

ファイルへのアクセスは、Workfront プロジェクトのアクセス許可に従います。 Workfrontのアクセスレベルでは許可されているので、ユーザーは権限を持つプロジェクトのみを表示および操作できます。

各Workfront プロジェクトのルートフォルダーは、デスクトップビューでは読み取り専用です。 ユーザーは、Finderまたはファイルエクスプローラーからプロジェクトのルートフォルダーの名前を変更、移動、または削除することはできません。 Workfrontの権限に応じて、プロジェクトフォルダー内の任意の深さでフォルダー、サブフォルダー、ファイルを作成できます。

## 一般的な問題のトラブルシューティング

エンドユーザーのトラブルシューティング手順については、[Adobe Cloud Driveのトラブルシューティング ](/help/quicksilver/documents/adobe-cloud-drive/troubleshoot-adobe-cloud-drive.md)を参照してください。 以下に示す問題は、管理者に固有のものです。

### ソフトウェア配布でAdobe Cloud Drive インストーラーが見つかりません

**原因：** Adobe Admin Consoleのユーザーに対して、Adobe Cloud Drive アクセスが有効になっていません。

**解決策：**

1. [adminconsole.adobe.com](https://adminconsole.adobe.com/)にログインし、**Users**&#x200B;をクリックします。
1. ユーザーを検索し、名前をクリックします。
1. 「**役割**」タブをクリックし、Adobe Cloud Driveが有効になっているかどうかを確認します。

**原因：** Creative Cloud コンプリートプランは、Workfrontとは異なるIMS組織でプロビジョニングされています。

**解決策：**&#x200B;現在利用できる解決策はありません。

### ユーザーはアプリケーションをインストールしてサインインしましたが、ドライブにフォルダーが表示されません

**原因：** Workfront プロジェクトに対する権限がありません。

**解決策：**

1. Workfrontで、少なくとも1つのプロジェクトに対する権限をユーザーが持っていることを確認します。
1. そうでない場合は、ユーザーとプロジェクトを共有します。
1. プロジェクトフォルダーが表示されるまで、最大5分待つようにユーザーに依頼します。
1. 5分経ってもフォルダーが表示されない場合は、Adobe Cloud Driveを終了して再起動するようにユーザーに依頼します。

### Adobe Cloud Driveにログインできない

**原因：** ユーザーのAdobe Admin Console アカウントが非アクティブであるか、IDが正しく設定されていません。

**解決策：**

1. Adobe Admin Consoleで、**Users**&#x200B;をクリックし、ユーザーを検索します。
1. ユーザーのアカウントステータスが&#x200B;**アクティブ**&#x200B;であることを確認します。
1. ユーザーのメールドメインがAdmin Console ディレクトリ内のクレームされたドメインであることを確認します。
1. 組織でSSOを使用している場合は、ID プロバイダーでユーザーのアカウントがアクティブであることを確認します。
1. ユーザーに再度ログインを試すように依頼します。

### ユーザーの保存後にファイルが同期されない

**原因：** ファイルが明示的に保存されていないか、ネットワーク接続に問題があります。

**解決策：**

1. アプリケーションで&#x200B;**ファイル** > **保存**&#x200B;を使用してファイルを保存したことをユーザーに確認します。 アプリケーションを閉じたり、自動保存を利用したりしても、Syncはトリガーしません。
1. ユーザーがインターネットにアクセスしており、`*.adobe.com`と`*.workfront.com`にアクセスできることを確認してください。
1. エラーインジケーターについては、メニューバー（macOS）またはシステムトレイ（Windows）のAdobe Cloud Drive アイコンを確認するようにユーザーに依頼します。
1. エラーが発生した場合は、Adobe Cloud Driveを終了して再起動し、ファイルを再度保存するようにユーザーに依頼します。
1. 問題が解決しない場合は、アプリケーションログを収集します。

   * **macOS:** `~/Library/Logs/Adobe/AdobeCloudDrive/`
   * **Windows:** `C:\Users\<username>\AppData\Local\Temp\Adobe\AdobeCloudDrive\`

### プロジェクトフォルダーにファイルの競合コピーが表示されました

**原因：** 2人のユーザーが、いずれかのバージョンがクラウドに同期される前に、同じファイルに変更を保存しました。 Adobe Cloud Driveは、両方のバージョンを自動的に保存しました。

競合するコピーでは、次の命名形式が使用されます。 `filename (Conflicted copy from device_name on date_time).extension`
例：`project_brief (Conflicted copy from jsmith's MacBook Pro on 2026-06-15-10-45-19).docx`

**解決策：**

1. 両方のユーザーに、どのバージョンが権限を持つかを尋ねます。
1. 競合したコピーからプライマリファイルに必要なコンテンツをコピーします。
1. 2つのバージョンを調整した後、競合したコピーを削除します。

   >[!NOTE]
   >
   >Adobe Cloud Driveでは、ファイルロックは使用されません。 複数のユーザーが同じファイルを編集する際の競合を防ぐには、複数のユーザーがデスクトップから同じファイルにアクセスする前に、Workfront タスクの割り当てまたは承認ワークフローを通じて編集を調整します。

### ユーザーは、プロジェクトにフォルダーまたはファイルを作成できません

**原因A:** ユーザーがプロジェクトのルート レベルでフォルダーまたはファイルを作成しようとしています。 プロジェクトのルートフォルダーは現在、Adobe Cloud Driveで読み取り専用です。 ルートレベルのフォルダーは、Workfrontで作成および管理されるWorkfront プロジェクトを表します。

**解決策：**

1. プロジェクト内の既存のサブフォルダーに移動して、そこにファイルまたはフォルダーを作成するようにユーザーに依頼します。
1. プロジェクト内に新しいトップレベルフォルダーが必要な場合は、最初にWorkfrontで作成するように依頼します。 その後、Adobe Cloud Driveに表示されます。

**原因B:** Workfront プロジェクトに対する編集権限がありません。

**解決策：**

1. Workfrontで、プロジェクトに対するユーザーの権限を確認します（**ビュー**、**投稿**、または&#x200B;**管理**）。
1. ユーザーがファイルを作成または編集する必要がある場合は、ユーザーの権限を&#x200B;**Contribute**&#x200B;または&#x200B;**Manage**&#x200B;に更新します。
