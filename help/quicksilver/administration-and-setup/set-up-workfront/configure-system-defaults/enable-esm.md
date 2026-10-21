---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Adobe クラウドストレージを有効にする
description: Adobe クラウドストレージを有効にすると、すべてのAdobe製品に対して統合ストレージソリューションを使用できるようになります。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 5d487a068f747eb538775846cca80ab5a3a612bf
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 6%

---
# Adobe クラウドストレージを有効にする

Adobe クラウドストレージは、Adobe エンタープライズ製品全体のアセットの中央リポジトリとして機能する、クラウドベースの統合ストレージソリューションです。 この記事では、組織全体または特定のグループのデフォルトのストレージオプションとしてAdobe クラウドストレージを有効にする方法について説明します。

>[!IMPORTANT]
>
>Adobe クラウドストレージをworkfrontの「設定」エリアで有効にするまで、環境に何も変わりません。<br>
>Adobe クラウドストレージを有効にすると、新しいプロジェクトのみがAdobe クラウドストレージを使用し、これにはFrame.io ビューアと統合承認が含まれます。 既存のプロジェクトでは、現在のストレージが引き続き使用され、変更はありません。

タイミングを制御することで、エクスペリエンスをテストし、Workfront Fusionのシナリオを更新し、誰かが作業する前に変更をレポートする計画を立てることができます。 何が異なるか、ロールアウトを計画する方法について詳しくは、[Adobe クラウドストレージ上のWorkfrontへの移行](/help/quicksilver/review-and-approve-work/workfront-storage.md)を参照してください。

## Adobe クラウドストレージでの承認機能

Adobe クラウドストレージは、プロジェクトが使用する承認サービスを決定します。 Adobe クラウドストレージをサポートするバージョンのWorkfrontに移行しても、組織全体が統合承認に自動的に切り替わることはありません。 承認サービスは、各プロジェクトのストレージモデルによって異なります。

* **Adobe クラウドストレージプロジェクト**&#x200B;では、Frame.io ビューアでレビューと承認が行われ、デフォルトで統合承認が使用されます。
* **従来のWorkfront ストレージプロジェクト**&#x200B;は、既に使用している承認サービスを維持します。 組織によっては、統合承認やレガシードキュメントの承認などが考えられます。

Adobe クラウドストレージでのレビューと承認のエクスペリエンスについて詳しくは、[Adobe クラウドストレージでのWorkfrontへの移行](/help/quicksilver/review-and-approve-work/workfront-storage.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意のワークフローパッケージ</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Adobe クラウドストレージを有効にする

Adobe クラウドストレージを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。
1. **ストレージの環境設定** セクションまでスクロールします。
1. デフォルト ドロップダウンメニューで、**Adobe クラウドストレージ**&#x200B;を選択します。
1. （オプション）Adobe クラウドストレージと従来のWorkfront ストレージを組み合わせて使用する場合は、「**ユーザーがストレージプロバイダーを選択することを許可する**」チェックボックスをオンにします。

   >[!NOTE]
   >
   >このオプションを有効にすると、ユーザーは新しいプロジェクトの作成時にストレージプロバイダーを選択できます。 Adobe クラウドストレージは、デフォルトのストレージプロバイダーであるため、「新しいプロジェクト」というラベルが付けられます。 従来のWorkfront ストレージは、「従来のプロジェクト」とラベル付けされます。
   >
   >![新しいプロジェクトと従来のプロジェクトのオプション ](assets/new-esm-project.png)

1. 「適用先」ドロップダウンメニューで、次のいずれかのオプションを選択します。

   * **組織全体**：このオプションは、デフォルトのストレージプロバイダーをWorkfront環境全体に適用します。 ユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます。
   * **特定のグループ**：このオプションは、組織内の特定のグループにのみデフォルトのストレージプロバイダーを適用します。 指定したグループのユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます。

     ![ ストレージ環境設定グループ ](assets/configure-storage-preference.png)

1. 「**保存**」をクリックします。

   >[!NOTE]
   >
   >既存のプロジェクトは、作成されたストレージモデルを保持します。 例えば、Adobe クラウドストレージを使用するプロジェクトでは、デフォルトのストレージ環境設定を変更した後も、引き続きAdobe クラウドストレージを使用します。



## サンドボックス環境でのAdobe クラウドストレージ

Adobe クラウドストレージは、[!DNL Workfront] サンドボックス環境で利用できます。本番環境でロールアウトする前に、この記事で説明した機能をテストできます。 ただし、Frame.io ビューアはサンドボックスでは利用できないため、統一されたレビューと承認のエクスペリエンスを本番環境で検証する必要があります。

カスタムリフレッシュサンドボックスがある場合は、Adobe クラウドストレージをサポートするWorkfrontのバージョンにアップグレードした後でリフレッシュする必要があります。 更新により、サンドボックスからAdobe クラウドストレージ機能にアクセスできるようになり、テストを開始できます。 詳しくは、[ カスタムリフレッシュサンドボックス環境 [!DNL Adobe Workfront] を参照してください。](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)
