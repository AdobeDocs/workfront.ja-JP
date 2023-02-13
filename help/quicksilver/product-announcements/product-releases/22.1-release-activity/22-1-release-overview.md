---
title: 22.1 リリースの概要
description: 22.1 リリースの概要
author: Luke
draft: Probably
feature: Product Announcements
exl-id: daf977fe-957a-40ad-a37f-1c164cb4ada3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '4721'
ht-degree: 0%

---

# 22.1 リリースの概要

このページでは、22.1 リリースに含まれる機能について説明します。 新しいAdobe Workfrontエクスペリエンスでは、すべての機能を使用できます。 一部の機能は、Adobe Workfront Classic でも使用できます。しかしながら [Workfront Classic は 2022 年 3 月に廃止されます](https://one.workfront.com/s/new-workfront-experience)。その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.1 release nears its planned Production release the week of January 17, 2022
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.1. </p>
-->

これらの機能強化は、2022 年 1 月 18 日の週に実稼動環境で利用できるようになりました。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of January 17, 2022, unless otherwise specifiedthe week of May 10, 2021
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on
<a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times
</MadCap:conditionalText>
-->

。

## Adobe Workfrontの機能強化

* [管理者の機能強化](#administrator-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [リクエストの強化](#requests-enhancements)
* [校正機能の強化](#proofing-enhancements)
* [その他の機能強化](#other-enhancements)
* [モバイル機能の強化](#mobile-enhancements)

### 管理者の機能強化 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#document" class="MCXref xref" xrefformat="{para}">「更新」領域にログインしたドキュメントのダウンロード</a> </p> <p>ユーザーがWorkfrontに保存しているドキュメントのダウンロード数を追跡できるように、ユーザーがドキュメントをダウンロードしたときに、そのドキュメントの更新領域にエントリが記録されるようになりました。</p> <p>この機能は、新しくアップロードしたドキュメントのプレビューでテストすることをお勧めします。</p> </td> 
   <td> <p>プレビューリリース：2021 年 12 月 16 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#create" class="MCXref xref" xrefformat="{para}">OAuth2 アプリを作成してアプリケーションをWorkfrontと統合する</a> </p> <p>Workfrontを、Workfrontに組み込み統合を提供していない他のアプリケーションと統合できるようになりました。 統合するアプリケーションの OAuth2 アプリを作成すると、データが安全な業界標準の OAuth2 認証プロトコルで保護されていることを知りながら、そのアプリケーションがWorkfrontにアクセスできるようになります。</p> <p>以前は、組み込みの統合、Workfront Fusion、Workfront API を使用して、他のアプリケーションとのみ統合できました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#interfac" class="MCXref xref" xrefformat="{para}">会社領域のインターフェイステキストの改善</a> </p> <p>「設定」の「会社」領域で、新しい確認メッセージと若干の変更により、会社のメンバーシップを管理しやすくなります。 例えば、左側のパネルのセクション名「People」は、「会社メンバー」になりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">カスタムフォームをグループに追加する</a> </p> <p>Group オブジェクトでカスタムフォームがサポートされるようになりました。 これにより、組織内のグループが、特定のニーズやワークフローを満たす情報を容易に取得および共有できます。 ユーザーは、カスタムフォームの作成、カスタムフォームの添付、カスタムフォームの保存など、他のWorkfrontオブジェクトに対して実行できる操作と同じ操作をグループに対しても実行できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#styling" class="MCXref xref" xrefformat="{para}">カスタムForms領域でのスタイル設定の更新</a> </p> <p>カスタムForms領域は、新しいWorkfrontエクスペリエンスの他の多くの領域と最新の状態にするための新しいルックアンドフィールを備えています。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 2 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#many" class="MCXref xref" xrefformat="{para}">計算カスタムフィールドを作成するための多くの機能強化</a> </p> <p>新しい計算エディタで、次の追加を使用すると、計算カスタムフィールドをより簡単に作成できるようになりました。</p> 
    <ul> 
     <li> <p>計算の式の上にマウスポインターを置くと、説明、使用例、ヘルプ記事の詳細情報へのリンクなど、式に関する情報が表示されます。</p> </li> 
     <li> <p>追加する各式は、タイプに応じて色分けされます。 これにより、式を見つけやすくなり、式の種類をすぐに認識できます。</p> </li> 
     <li> <p> 行番号は、長い計算で関数を識別し、参照するのに役立ちます。</p> </li> 
     <li> <p>式またはフィールド名の入力を開始すると、使用可能な項目のリストが表示され、必要な項目を選択できます。 また、開き丸括弧を入力すると、閉じ丸括弧が自動的に追加されます。</p> </li> 
     <li> <p>計算エディターを離れることなく、既存のオブジェクトを使用して計算結果をプレビューできます。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 4 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">新しい計算フィールドウィンドウで式とフィールドを選択する</a> </p> <p>カスタムフォームでの計算フィールドの作成が、引き続き容易になります。 次に、[ 最大化 ] をクリックして新しい計算エディタを開くと、必要な式やフィールドを検索して選択できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 10 月 22 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#larger" class="MCXref xref" xrefformat="{para}">集計フィールドを作成する領域が大きい</a> </p> <p>これで、カスタムフォームで複雑な計算フィールドを簡単に作成できます。 新しい「最大化」ボタンをクリックして、計算を作成するための大きな編集ウィンドウを開きます。 完了したら、「最小化」をクリックして、カスタムフォームの作業を続行します。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 10 月 14 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#grant" class="MCXref xref" xrefformat="{para}">アクセスレベルを使用したチームへのアクセス権の付与</a> </p> <p>「アクセスレベル」領域の新しいセクションでは、チームに対するユーザーのアクセスを管理するためのより詳細なコントロールを提供します。 チームを作成、編集および表示できるユーザーを決定できます。</p> <p>これによって、ユーザのチームへの既存のアクセスが変更されることはありません。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 2 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#group" class="MCXref xref" xrefformat="{para}">グループマッピングがブループリントで使用できるようになりました</a> </p> <p>一部のブループリントにグループが含まれるようになり、ブループリントをインストールする前にカスタマイズできます。 ブループリント内のグループをWorkfrontインスタンス内の既存のグループにマッピングしたり、必要に応じて新しいグループを作成したりできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 2 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">ブループリント会社のマッピングおよびその他の機能強化</a> </p> <p>一部のブループリントに会社が含まれるようになり、ブループリントをインストールする前にカスタマイズできます。 ブループリント内の会社をWorkfrontインスタンス内の既存の会社にマッピングしたり、必要に応じて新しい会社を作成したりできます。</p> <p>ブループリントのその他の機能強化も利用できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 12 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">ステータスと会社に関する監査ログ情報の表示</a> </p> <p>設定の監査ログ領域でステータスや会社に関するインシデントの情報を表示すると、それらのインシデントのトラブルシューティングをより簡単におこなうことができます。</p> <p>例：</p> 
    <ul> 
     <li> <p>ステータスの名前変更、ロック、非表示のユーザー、および変更日時を確認できます。</p> </li> 
     <li> <p>会社から一部のメンバーやジョブの役割を削除したユーザーと削除したタイミングを確認できます。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 4 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#manage" class="MCXref xref" xrefformat="{para}">会社メンバーシップをより簡単に管理</a> </p> <p>会社領域では、更新されたツールバーを使用すると、既存のWorkfrontユーザーを会社に簡単に追加したり、会社メンバーを削除したりできます。 </p> <p>以前は、これらの操作は「会社を編集」ボックスでのみ使用できました。</p> <p>更新されたツールバーには、メンバーのユーザープロファイル情報の編集やシステムでの非アクティブ化など、前のツールバーで使用できたすべてのアクションも含まれています。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 5 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#groups" class="MCXref xref" xrefformat="{para}">グループは、独自のタイムシートと時間の基本設定を構成できます</a> </p> <p>大規模な組織では、管理者がシステムレベルで設定した基本設定を継承するのではなく、固有のワークフローに合わせてタイムシートと時間の基本設定を個別に構成する必要がある場合があります。 Workfrontの管理者は、システム内のすべてのグループのタイムシートと時間の優先順位をロック解除して、自分で構成できるようになりました。</p> <p>この機能は、最近、プロジェクトの環境設定や、タスクおよび問題の環境設定に追加されました。 </p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> <p>プレビューリリース： 2021 年 9 月 10 日<br></p> <p>実稼動リリース： 2021 年 11 月 9 日 <span style="color: #ff0000;">( この機能は、実稼動環境では、21.4 リリースのクラスター 4 のお客様のみが使用できるようになりました。2021 年 11 月 8 日に、実稼動環境の他のすべてのクラスターで使用可能になりました )。</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#select2" class="MCXref xref" xrefformat="{para}">グループのロックを解除または再ロックする複数の通知を選択します</a> </p> <p>グループの電子メール通知のロック解除や再ロックがより速く、簡単になりました。 複数の通知を選択し、選択内容が正しいことを確認した後、ツールバーに表示される新しい「ロック解除」または「ロック」ボタンをクリックします。</p> <p>以前は、通知のロックを解除し、一度に 1 つずつ再ロックする必要がありました。 Workfrontには現在 95 の通知があるので、すべてまたは多くの通知に対しておこなう必要がある場合は時間がかかりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 10 月 14 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">グループ管理者の場合：グループの削除時に置き換えグループを簡単に選択できる</a> </p> <p>グループを削除する場合は、[ グループの削除 ] ボックスに 2 つの改善点があり、削除したグループのユーザー、作業項目、サブグループを保持する置換グループを簡単に選択できます。</p> 
    <ul> 
     <li> <p>グループの名前を入力すると、すばやく見つけることができます。 </p> </li> 
     <li> <p>新しい情報アイコンを使用して、必要な置換グループを選択していることを確認できます。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 10 月 14 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

### プロジェクトの強化 {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">ドキュメントフォルダーの共有</a> </p> <p>「ドキュメント」領域で、ドキュメントフォルダとそのコンテンツを共有できるようになりました。 以前は、これは不可能でした。1 つのフォルダー内の各ドキュメントを別々に共有する必要がありました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 16 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#limit" class="MCXref xref" xrefformat="{para}">共有しているテンプレートにドキュメントを追加する機能を制限</a> </p> <p>プロジェクトテンプレートにドキュメントを追加する人が、プロジェクトにドキュメントを追加すると考える場合があります。 これを防ぐには、ビューアクセスでテンプレートを共有する際に、新しい詳細設定「ドキュメントを追加」を無効にできます。 これにより、受信者はテンプレートにドキュメントを追加できなくなります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 10 月 14 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#update" class="MCXref xref" xrefformat="{para}">ダッシュボードのダッシュボードリストとレポートのツールバーを更新しました</a> </p> <p>4 つのダッシュボードページ上のツールバーは、プロジェクト、タスク、問題などの他のWorkfrontリストと一致する最新のルックアンドフィールになりました。 この直感的なツールバーにより、ダッシュボードの追加、編集、共有、コピー、削除が簡単になりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#add" class="MCXref xref" xrefformat="{para}">ドキュメント用のカスタムフォーム概要パネルの追加と編集</a> </p> <p>ドキュメントの概要パネルで、カスタムフォームを直接追加および編集できるようになりました。</p> <p>この変更により、ドキュメントの「概要」に新しい外観と操作性が表示されます。 新しい「概要」セクションが追加されました。このセクションには、画像のサムネールとドキュメントの詳細が含まれています。 ドキュメントの詳細セクションで、ドキュメントのチェックインとチェックアウトを行うこともできます。</p> <p>以前は、ドキュメントの詳細の「カスタムフォーム」タブに移動して、編集やカスタムフォームの追加をおこなう必要がありました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 19 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#filter" class="MCXref xref" xrefformat="{para}">アジャイルボードのユーザーリストでフィルターすると、ほとんどの割り当てを最初に行ったユーザーが表示されます</a> </p> <p>現在は、最初に最も多くの割り当てを持つユーザーがフィルターに表示され、リストをスクロールせずに見つけやすくなります。</p> <p>以前は、かんばんボードとスクラムボードの両方で、ユーザーリストによるフィルターがアルファベット順に表示されていました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 12 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 <b style="color: #ff0000;">(22.1 リリースから削除されました。 プレビューでは使用できなくなりました。)</b></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#change" class="MCXref xref" xrefformat="{para}">タスクのコピーまたは移動時に、先行タスクの既定のオプションを変更する</a> </p> <p>タスクをコピーまたは移動する際の手動ステップ数を最小限に抑えるために、デフォルトでタスクと共にコピーまたは移動される情報を更新しました。 これで、すべての先行タスクは、既定では [ すべての先行タスク ] オプションが選択されているので、既定ではタスクと共にコピーまたは移動されます。 </p> <p>この機能強化以前は、タスクをコピーまたは移動する際に、既定で [ すべての先行タスク ] オプションが選択解除されていました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">1 つまたは複数のタスクをコピーする際の新しいエクスペリエンス</a> </p> <p>Workfrontの使用を新しいAdobe Workfrontエクスペリエンスと一貫させるために、タスクをコピーする際にインターフェイスのデザインを変更しました。 現在、タスクレベルでタスクをコピーする場合や、リスト内の 1 つ以上のタスクをコピーする場合に使用できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 19 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">1 つまたは複数のタスクをリストから移動する際の新しいエクスペリエンス</a> </p> <p>同じタスクを実行する際に一貫したエクスペリエンスを提供するために、1 つまたは複数のタスクをリストから移動し、タスクレベルでタスクを移動する際のエクスペリエンスに合わせてインターフェイスを更新しました。 （以前のプレビューリリースで、タスクレベルでタスクを移動するエクスペリエンスを更新しました）。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 5 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">タスクレベルでタスクを移動する際の新しいエクスペリエンス</a> </p> <p>Workfrontを新しいWorkfrontエクスペリエンスと一貫して使用するため、タスクを移動するためのインターフェイスのデザインを変更しました。 これは、現在、タスクレベルでタスクを移動する場合に使用できます。 次のリリースでは、この再設計を拡張して、タスクをリストから移動させます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 10 月 22 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">イシューレベルでテンプレートを使用してイシューをプロジェクトに変換する際の新しいエクスペリエンス</a> </p> <p>Workfrontを新しいWorkfrontエクスペリエンスと一貫して使用できるように、イシューページから変換する際に、テンプレートを使用してイシューをプロジェクトに変換する際のインターフェイスを再設計しました。</p> <p>イシューを変換するために選択した後、すぐにお気に入りのリストに簡単にアクセスできるようになりました。</p> <p>再設計されたインターフェイスは、最近更新したテンプレートからプロジェクトを作成する場合のエクスペリエンスと一致します。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 <span style="color: #ff0000; font-weight: bold;">( この機能は、2022 年 3 月 4 日に実稼動環境から一時的に削除されました。 その後、2022 年 4 月 28 日より段階的に公開されました。 公開日は 2022 年 5 月 5 日。 これは、すべての顧客がプレビューと実稼動で使用できるようになりました )。</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">リスト、レポート、ダッシュボードのテンプレートを使用して、問題をプロジェクトに変換する</a> </p> <p>作業の効率を高め、ペースの速い環境で問題を簡単に変換できるように、リスト、レポート、ダッシュボードのテンプレートを使用して問題をプロジェクトに変換する機能が追加されました。</p> <p>この機能強化がおこなわれるまでは、この機能は、イシューページからイシューを変換した場合にのみ存在していました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 <span style="color: #ff0000; font-weight: bold;">( この機能は、2022 年 3 月 4 日に実稼動環境から一時的に削除されました。 その後、2022 年 4 月 28 日より段階的に公開されました。 公開日は 2022 年 5 月 5 日。 これは、すべての顧客がプレビューと実稼動で使用できるようになりました )。</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

### リソース管理の強化 {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">設定パネルの改善と、ワークロードバランサーでのプロジェクトとタスクのカラーコード機能の改善</a> </p> <p>ワークロードバランサーを使用する際のエクスペリエンスを向上させるために、次の機能強化が導入されました。</p> 
    <ul> 
     <li> <p>設定パネルのデザインが一新され、以前ツールバーにあったオプションが含まれるようになりました。 これにより、ツールバーのスペースが使いやすくなります。</p> </li> 
     <li> <p>プロジェクトごとにカラーテーマをカスタマイズする機能が追加されました。 プロジェクトで色分けを選択すると、各プロジェクトとその作業項目が同じ色で表示されます。 色は各プロジェクトに固有です。 この機能強化の前は、プロジェクトステータス別のカラーコードのみを表示できました。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">ワークロードバランサーを使用して作業を一括で割り当て</a> </p> <p>スケジューリングツールを廃止し、ワークロードバランサーに置き換える取り組みを続ける中で、割り当てを一括で管理する機能を追加しました。 複数の作業項目を一度に複数のユーザーに割り当てたり、複数の作業項目のユーザーを他のユーザーに置き換えたり、複数の項目のユーザーを一度に割り当て解除したりできるようになりました。 ワークロードバランサーの新しい一括割り当て機能を使用すると、これらすべてを 1 回のアクションで実行できます。</p> <p>この機能強化がおこなわれるまでは、手動またはドラッグ&amp;ドロップで 1 人のユーザーを 1 つの作業項目に割り当てることができました。</p> <p>新しい一括割り当てには、名前に加えて、プロジェクトステータスとタスクステータス別の新しいフィルタリング機能も含まれます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 2 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#override" class="MCXref xref" xrefformat="{para}">ジョブの役割を管理する際の通貨の上書き</a> </p> <p>グローバル組織全体のコストと請求率を簡単に管理できるように、ジョブロールの通貨の上書きを実装しました。 この機能を使用して、ジョブロールの場所に一致する通貨でジョブロールのコストと請求率を設定できるようになりました。 これにより、ジョブロールのすべての財務計算でシステム通貨が上書きされます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
 </tbody> 
</table>

### リクエストの強化 {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#interfac" class="MCXref xref" xrefformat="{para}">リクエストを作成するためのアクセス権を持たないユーザーのインターフェイスが改善されました</a> </p> <p>リクエストを処理する際のユーザーエクスペリエンスを向上させるために、リクエストを作成するアクセス権がないことをログインユーザーに示すインターフェイスが改善されました。 この改善により、イシューを作成するアクセス権を持たないユーザーに対しては、「新しいリクエスト」ボタンが淡色表示になります。 淡色表示のボタンにカーソルを合わせると、Workfront管理者が現在のユーザーのリクエスト作成へのアクセスを制限したことを示すツールヒントが表示されます。 </p> <p>この機能強化以前は、これらのユーザーの「リクエスト」領域に「新しいリクエスト」ボタンが表示されていませんでした。 リクエストを新規としてコピーして送信することも制限されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：2021 年 12 月 2 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#copy" class="MCXref xref" xrefformat="{para}">リクエストのコピーと送信</a> </p> <p>リクエストの送信プロセスを最適化するために、既存のリクエストをコピーして新しいリクエストとして送信できる新しい機能が追加されました。 これは、類似したリクエストを頻繁に送信する場合に役立ちます。 この場合、既存のリクエストを再利用し、いくつか変更を加えて、新しいリクエストとして送信できます。</p> <p>この変更により、他のユーザーが送信したリクエストを表示できるユーザーも、そのリクエストをコピーして新規として送信できます。 リクエストキュープロジェクトの次の設定を更新すると、この処理を防ぐことができます。同じ会社のユーザーは、すべてのリクエストに対して同じ権限を継承します。</p> <p>この機能がリリースされる前に、キュートピックのない要求キューに送信された問題をコピーして再送信することはできません。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 19 日 <br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">リクエスト領域の「Submitted」セクションの Summary パネルエクスペリエンスを更新しました</a> </p> <p>Summary パネルとの表示やインタラクションを改善するために、「Requests」領域の「Submitted」セクションにある「Open Summary」アイコンにラベルを追加しました。 ラベルは動的になり、パネルが開いているか閉じているかに応じて更新されます。 </p> <p>要求を選択せずに Summary パネルを開くと、より使いやすい画像が表示され、パネルを開く前に項目を選択するようにユーザーに明確に指示できるようになりました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 11 月 5 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

### 校正機能の強化 {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">レビュー担当者およびリクエスト担当者向けの校正機能の改善</a> </p> <p>Workfrontと配達確認を統合し、レビュー担当者とリクエスターの校正機能に関していくつかの改善を行いました。</p> 
    <ul> 
     <li> <p>Workfrontのユーザーには、校正ライセンスを持っているかどうかに関係なく、アクションの適用やコメントの解決などの追加の権限を付与することができます。</p> </li> 
     <li> <p>ログインが必要な配達確認や、電子署名が必要な配達確認に、レビュー担当者とリクエスターを追加できます。</p> </li> 
     <li> <p>また、Workfrontと配達確認の接続性を向上させることで、すべてのユーザーにメリットがもたらされます。 これで、ユーザーを非アクティブ化したり、ユーザーの E メールアドレスを更新したりする際に、Workfrontで変更した場合の校正に更新が正しく反映されるようになりました。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日 <b style="color: #ff0000;">（統合校正をおこなった EMEA のお客様のみ利用可能）（2022 年 1 月 18 日に残りのすべてのお客様が利用できます）</b><br></p> <p>実稼動リリース： 2021 年 12 月 21 日 <b style="color: #ff0000;">（統合校正をおこなった EMEA のお客様のみ利用可能）（2022 年 2 月 3 日の残りのお客様）</b><br></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#electron" class="MCXref xref" xrefformat="{para}">配達確認のための電子署名の強化</a> </p> <p>ユーザーが電子的に配達確認に署名するのを容易にしました。 これで、ユーザーは、Workfront資格情報を使用して、配達確認に関する決定に署名できます。</p> <p>SSO 資格情報を使用して配達確認に電子署名を行うには、Workfront Proof で SSO を設定する必要があります。 </p> <p>以前は、ユーザーはWorkfront Proof の資格情報を使用する必要がありましたが、これはWorkfrontの資格情報とは異なります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日 <b style="color: #ff0000;">（EMEA と米国の両方のお客様が利用可能）</b><br></p> <p>実稼動版リリース：未定 <b style="color: #ff0000;">（2021 年 12 月 21 日、EMEA のお客様が利用可能）（2022 年 2 月 4 日）残りのすべてのお客様に対して利用可能</b></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#desktop" class="MCXref xref" xrefformat="{para}">デスクトップビューアのアップグレード</a> </p> <p>Chrome バージョン 91 までをサポートするよう、デスクトップ校正ビューアをアップグレードし、インタラクティブな配達確認との互換性を高めました。</p> <p>Windows ユーザーは、最新バージョンにアップグレードするには、デスクトップビューアを手動で再インストールする必要があります。 その後、今後のデスクトップ校正ビューアの更新は自動的に行われます。</p> <p>Macユーザーは、自動的に最新バージョンにアップグレードされます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：なし<br></p> <p>実稼動リリース： 2021 年 12 月 2 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他の機能強化 {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">ユーザーリスト用の新しいツールバー</a> </p> <p>より新しく直感的なツールバーにより、ユーザーリストでのユーザーの管理が容易になります。 ツールバーのボタンを使用すると、Workfrontにユーザーをすばやく追加したり、ユーザーに登録を促したり、ユーザーのプロファイルを管理したりできます。 また、ユーザーリストを書き出すこともできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 8 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#default" class="MCXref xref" xrefformat="{para}">計画完了日のデフォルトの昇順です。また、ホーム作業リストの計画開始日でグループ化できます。</a> </p> <p>注意が必要な項目を簡単かつ迅速に見つけられるように、2 つの機能強化を追加しました。これにより、最も早い期限の項目がデフォルトで作業リストの上部に表示され、タスクと問題を計画開始日別にグループ化できます。 </p> <p>これらの機能強化がおこなわれる前は、項目を計画完了日およびコミット日のみでグループ化できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#add" class="MCXref xref" xrefformat="{para}">すべてのライセンスユーザーの更新情報領域を追加します</a> </p> <p>Workfront Classic と新しいWorkfrontエクスペリエンスとの同等性を創出するための取り組みの一環として、すべてのユーザーに対してマイアップデート領域を再導入しました。</p> <p>この更新の結果、レビューユーザーは、レイアウトテンプレートに割り当てられていない限り、この領域をデフォルトのランディングページとして見つけることができます。</p> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートを使用して、この領域をすべてのユーザーのメインメニューおよびトップナビゲーションに追加できます。</p> <p>[ マイアップデート ] 領域を開くと、次の情報がすぐに見つかります。</p> 
    <ul> 
     <li> <p>決定を待機している承認は、マイアップデートページの前半に表示されます。 承認、拒否、変更の提案、アクセス権の付与または他のユーザーへの承認の委任をおこなうことができます。</p> </li> 
     <li> <p>追加したコメントは、[ マイ更新 ] ページの下半分の [ メンション ] セクションに表示されます。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">タイムシートの改善</a> </p> <p>Workfrontで時間を管理するすべてのユーザーのエクスペリエンスを向上させるために、タイムシートに様々な更新を導入しています。</p> <p>更新の一部を次に示します。</p> 
    <ul> 
     <li> <p>ユーザーが現在のタイムシートを持っている場合、[ タイムシート ] 領域が現在のタイムシートに開き、現在のタイムシートで検索およびクリックする時間を節約できます。 現在のタイムシートがない場合、[ タイムシート ] 領域には、現在の [ マイタイムシート ] セクションが表示されます。</p> </li> 
     <li> <p>カーソルを合わせるか、時間を入力するためにクリックした行がハイライト表示され、可視性が向上します。</p> </li> 
     <li> <p>タイムシートボタンを含むフッターが固定され、ページの下部にスクロールせずに常に保存およびキャンセルできるようになりました。 また、この領域に新しい「トップに戻る」ボタンを追加し、ページのトップにすばやく戻ることができます。</p> </li> 
     <li> <p>新しい警告通知で、未保存の変更に関する警告が表示され、タイムシートから移動する際に情報が失われないようになりました。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース： 2021 年 12 月 3 日<br></p> <p>実稼動版リリース： 22.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">ヘルプメニューの更新</a> </p> <p>上部ナビゲーションバーのヘルプリンクをクリックすると、より効率的なメニューが表示されるようになりました。 新しいメニューでは同じ情報を提供しますが、ナビゲーションのレベルが少なくなり、関連するコンテンツを表示するためのクリック数が少なくなります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：なし<br></p> <p>実稼動版リリース： 22.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

### モバイル機能の強化 {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">モバイルアプリでの配達確認機能の強化</a> </p> <p>Adobe Workfrontモバイルアプリで、次の操作を実行できるようになりました。</p> 
    <ul> 
     <li> <p>内部および外部の受信者との配達確認の共有</p> </li> 
     <li> <p>配達確認コメントを表示</p> </li> 
     <li> <p>配達確認をダウンロード</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>プレビューリリース：なし<br></p> <p>実稼動版リリース：2022 年 2 月初旬</p> <p><strong>次の環境で使用できます。</strong> </p> <p>iOSモバイルアプリ</p> <p>Android モバイルアプリ</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境では 22.1 リリーススケジュール以外のサイクルで使用できます。 最新の機能について詳しくは、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Workfront Scenario Planner の機能強化

リリースのこの時点では、シナリオプランナーの更新はありません。 この領域は、更新が利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof の強化

Workfront Proof の新機能が使用できるようになりました。 詳しくは、 [Workfront Proof リリースアクティビティ：2021 年 11 月 29 日の週](../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md).

## Workfront目標の強化

このリリースでは、現時点でWorkfront Goals の更新はありません。 この領域は、更新が利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API バージョン 14

API バージョン 14 では、いくつかのリソースとエンドポイントを変更しました。 一部の変更は新しい機能をサポートし、他の変更では、API を通じて入手可能な情報を使いやすくします。

の新機能と更新点について詳しくは、 [API バージョン 14 の新機能](../../../wf-api/api/new-api-version-14.md).

API バージョンについて詳しくは、 [API のバージョン管理とサポートのスケジュール](../../../wf-api/api/api-version-support-schedule.md).

## Workfront のメンテナンス更新

22.1 リリースでおこなわれたメンテナンスアップデートについて詳しくは、 [Workfrontメンテナンスの更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## 22.1 リリースウェビナー

Workfront 22.1 リリースウェビナーは 2022 年 1 月 12 日に発表されました。 オンラインセミナの録画は、 [Workfront One のイベントページ](https://one.workfront.com/s/event).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## トレーニングの更新

各Adobe Workfront製品リリースの学習プログラム、学習パス、ビデオ、ガイドに対しておこなわれた最新のアップデートを確認します。 詳しくは、 [トレーニングリリースの更新ページ](https://one.workfront.com/s/training-release-updates).

## サポートされなくなった機能

### Internet Explorer 11

Internet Explorer のサポートが削除され、WorkfrontはMicrosoft Edge を正式にサポートするようになりました。

サポートされているブラウザーについて詳しくは、 [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).
