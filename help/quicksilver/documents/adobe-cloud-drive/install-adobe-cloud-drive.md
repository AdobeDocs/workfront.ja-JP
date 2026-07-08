---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Adobe Cloud Driveのインストール
description: Adobe Cloud DriveをMacまたはWindows コンピューターにインストールして、Finderまたはファイルエクスプローラーで直接Adobe クラウドストレージプロジェクトを操作できるようにします。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 44bf6f571c35bd9a2f44fc23b2a5eaa3eb2d763b
workflow-type: tm+mt
source-wordcount: 532
ht-degree: 6%

---

# Adobe Cloud Driveのインストール

デスクトップでAdobe クラウドストレージプロジェクトを操作するには、Adobe Cloud DriveをMacまたはWindows コンピューターにインストールします。

Adobe Cloud Driveとは何か、またその機能について詳しくは、[Adobe Cloud Driveの概要](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront版</td> 
   <td><p>Adobe クラウドストレージをサポートするWorkfrontのバージョンを使用している必要があります。 お客様の組織がまだサポートされているバージョンを使用していない場合は、Adobe アカウント担当者にお問い合わせください。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">その他の製品</td> 
   <td><p>Adobe Cloud DriveにログインするためのAdobe ID</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

Adobe Cloud Driveをインストールする前に、次の点を確認してください。

* お使いのデバイスは、この記事の「[必要システム構成](#system-requirements)」セクションに記載されている必要システム構成に適合しています。
* お客様の組織は、Adobe クラウドストレージをサポートするWorkfrontのバージョンを使用しています。

お客様の組織がアプリケーションのインストールを管理しており、ダウンロード可能なAdobe Cloud Driveが表示されない場合は、Workfront管理者にお問い合わせください。

## 必要システム構成

**オペレーティングシステム：**

* macOS 13.5以降（IntelおよびApple Silicon）
* Windows 11 22H2 （22621.6060）以降（x64）
* Windows 11 23H2 （22631.6199）以降（ARM）

**ハードウェア：**

* 最小4 GB RAM
* アプリケーション用の空きディスク容量が500 MB
* キャッシュされたファイル用の追加スペース（使用状況によって異なります）

**ネットワーク：**

* 初期設定と同期のためのインターネット接続
* パフォーマンスに推奨される安定した接続

Adobe Cloud Driveが依存するサービスに確実にアクセスできるようにするには、[Adobe ネットワークエンドポイント ](https://helpx.adobe.com/in/enterprise/kb/network-endpoints.html)にリストされているネットワークエンドポイントを許可します。

## インストーラーのダウンロード

1. [Adobe Software Distribution](https://experience.adobe.com/#/downloads)に移動します。

1. Adobe ID を使用してログインします。
1. **一般** ダウンロード リストで、**Adobe Cloud Drive**&#x200B;を見つけます。
1. オペレーティングシステムのインストーラーを選択します。

   * **macOS:** Adobe Cloud Drive for Mac （ARM64またはIntel）
   * **Windows:** Windows用Adobe Cloud Drive （x64またはARM64）

1. 「**ダウンロード**」をクリックします。

   >[!IMPORTANT]
   >
   >Adobe Cloud Drive インストーラーが表示されない場合、組織がAdobe クラウドストレージをサポートするWorkfrontのバージョンを使用していない可能性があります。 Workfront管理者にお問い合わせください。

## Adobe Cloud Driveのインストール

オペレーティングシステムの手順を使用します。

### MacOSへのインストール

1. ダウンロードした`.dmg` ファイルを開きます。
1. 表示されるインストールアイコンをダブルクリックします。
1. 画面のセットアップウィザードに従います。

1. プロンプトが表示されたら、Adobe IDでログインします。

   別のAdobe デスクトップアプリケーションが既に実行中で、ログインしている場合、Adobe Cloud Driveはそのアクティブセッションを自動的に使用します。

### Windowsでのインストール

1. ダウンロードした`.exe` インストーラーを実行します。

1. インストールウィザードのプロンプトに従います。
1. プロンプトが表示されたら、**Install**&#x200B;をクリックします。
1. スタートメニューから&#x200B;**Adobe Cloud Drive**&#x200B;を起動します。
1. プロンプトが表示されたら、Adobe IDでログインします。

## インストールの確認

インストール後、Adobe Cloud Driveはコンピューター上にマウントされたドライブとして表示されます。

* **macOS:** **場所**&#x200B;の下のFinder サイドバーに、**Adobe Cloud Drive**&#x200B;として表示されます。
* **Windows:** In File Explorer under **このPC**, as **Adobe Cloud Drive**.

Adobe クラウドストレージプロジェクトがドライブ内にフォルダーとして表示されます。

ドライブでのプロジェクトの操作について詳しくは、[Adobe Cloud Driveの使用](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)を参照してください。
