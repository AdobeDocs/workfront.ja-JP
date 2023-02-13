---
content-type: release-notes
keywords: メモ，四半期，更新
navigation-topic: product-releases
title: 21.2 リリースの概要
description: 21.2 リリースは、2021 年 5 月 10 日の週に実稼動環境で公開されました。
author: Luke
feature: Product Announcements
exl-id: 1affe1ae-571e-4026-8ba7-8ce7104e1b89
source-git-commit: ab523ea5136b11a3ee1b6fa5746a1165f4b9d397
workflow-type: tm+mt
source-wordcount: '5474'
ht-degree: 0%

---

# 21.2 リリースの概要

21.2 リリースは、2021 年 5 月 10 日の週に実稼動環境で公開されました。

このページでは、Adobe Workfront Classic と、21.2 リリースに含まれる新しいAdobe Workfrontエクスペリエンスの両方の機能に関する情報を提供し、生産性とコラボレーションの解消に役立ちます。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.2 release nears its planned Production release the week of May 10, 2021, this page will be updated with all functionality included with 21.2.</p>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
the week of May 10, 2021.
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfrontの機能強化

* [ブランディングの変更 — Adobe Workfront](#branding-changes-adobe-workfront)
* [管理者の機能強化](#administrator-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [リクエストの強化](#requests-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [レポートの機能強化](#reporting-enhancements)
* [校正機能の強化](#proofing-enhancements)
* [統合の強化](#integration-enhancements)
* [その他の機能強化](#other-enhancements)
* [モバイル機能の強化](#mobile-enhancements)

### ブランディングの変更 — Adobe Workfront {#branding-changes-adobe-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#we" class="MCXref xref" xrefformat="{para}">我々は今正式にAdobe Workfront</a> </p> <p>WorkfrontはAdobe Workfrontに商標変更されました。 Adobe Workfrontアプリケーションおよびお客様向け Web サイトで最も重要な領域が更新されました。</p> <p>今後数週間で、この新しいブランディングが他の場所（モバイル用校正アプリやブラウザータブの favicon など）にも反映されます。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 28 日<br></p> <p>実稼動リリース： 2021 年 4 月 28 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for3" class="MCXref xref" xrefformat="{para}">管理者向け：Workfrontのその他の多くの領域に関する監査ログ情報の表示</a> </p> <p>「監査ログ」領域で、Workfront全体の様々な領域で変更を追跡し、トラブルシューティングできるようになりました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for4" class="MCXref xref" xrefformat="{para}">グループ管理者の場合：サブグループと更新されたツールバーを移動するためのコントロールを改善</a> </p> <p>セットアップのサブグループ領域で次の改善を行いました。</p> 
    <ul> 
     <li> <p>管理するグループを簡単に整理するために、「サブグループを追加」ツールバーボタンを追加し、新しいサブグループを作成して既存のサブグループを移動できます。</p> </li> 
     <li> <p>サブグループ領域のツールバーで、新しいWorkfrontエクスペリエンスで、リストが他の最新化されたリストと一致するようになりました。 グループを選択すると、ツールバーで使用可能な機能がアイコンで表されます。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">管理者向けの新機能：タイムシートと時間の環境設定ページのルックアンドフィールを更新しました</a> </p> <p>タイムシートと時間の環境設定ページの操作性を向上させるために、ユーザーインターフェイスを更新し、Workfrontの他の場所で見つかる最新の外観と操作性に合わせました。</p> <p>セクションと個々のオプションは、より縦のスペースで区切られているので、読みやすくなります。</p> <p>2 つのラジオボタンオプションのラベルは、それほど長くはないように分割されます。各ラベルの 2 番目の部分は、別々の行の情報メッセージになります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">グループ管理者の場合：グループ領域のリストの改善</a> </p> <p>セットアップのグループ領域で次の 2 つの機能が強化され、新しいWorkfrontエクスペリエンスの他の最新化されたリストと一致するリストが作成されました。</p> 
    <ul> 
     <li> <p>グループを選択すると、ツールバーで使用可能な機能がアイコンで表されます。</p> </li> 
     <li> <p>グループ、列、並べ替え、階層のリストでは、他のリストに慣れている方が新しい外観と操作性を持ちます。 また、デフォルトでは、1 つのページに最大 2,000 個の項目が表示され、100 個の項目は表示されません。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for2" class="MCXref xref" xrefformat="{para}">グループ管理者の場合：セットアップのグループ領域からプログラムを作成および編集する</a> </p> <p>アドビでは、グループとその関連オブジェクトを 1 か所で容易に管理できるようにし続けています。 これで、セットアップの [ グループ ] 領域で、グループのプログラムを表示して操作できるようになりました。 これにより、グループのプログラムを管理するために [ プログラム ] 領域に移動する必要がなくなります。 また、使用しているグループプログラムのリストを、システム内の他のプログラムとは別に保持します。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for5" class="MCXref xref" xrefformat="{para}">管理者向け：セットアップ領域の更新されたヘッダー</a> </p> <p>設定領域の管理者の向きを向上し、Workfront全体の一貫性を維持するために、設定ヘッダーを更新し、各設定ページとサブページを示す大きなカラフルなバッジ、フォントのスタイルとサイズを含む様々な更新をおこないました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 2 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for6" class="MCXref xref" xrefformat="{para}">グループ管理者の場合：グループページで追加のグループオブジェクトを表示および管理します</a> </p> <p>アドビでは、グループとその関連オブジェクトを 1 か所で容易に管理できるようにし続けています。 これで、セットアップのグループ領域で、グループの会社、チームおよびポートフォリオを表示および操作できます。 これにより、これらのオブジェクトの様々なセットアップページに移動して、グループの管理を行う必要がなくなります。 見ているグループオブジェクトのリストをシステム内の他のグループのリストとは別に保持します</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">グループ管理者向けの新機能：グループタイムシートプロファイルを割り当て</a> </p> <p>管理するグループのタイムシートプロファイルを管理しやすくなりました。 タイムシートプロファイルを作成できるだけでなく、自分のグループに割り当てたり、自分のグループの個々のメンバに割り当てたりすることもできます。 これは、アクセスレベルで [ タイムシートと時間 ] オプションが有効になっていない場合でも当てはまります。</p> <p>これまで、タイムシートプロファイルを割り当てるには、[ タイムシートと時間 ] オプションを有効にする必要がありました。 ただし、システム内のすべてのタイムシートと時間情報に対する表示と編集のアクセス権を付与するので、グループ管理者全員にとっては理想的ではない場合があります。 このレベルのアクセス権が必要ない場合は、グループのタイムシートプロファイルを管理できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 12 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for7" class="MCXref xref" xrefformat="{para}">管理者向け：ユーザーがオブジェクトリストに表示するフィルター、表示、グループ化を設定します</a><span class="uitext" style="color: #dc143c;"></span> </p> <p>新しいWorkfrontエクスペリエンスのレイアウトテンプレートを使用すると、Workfront全体のオブジェクトリストにユーザーが表示するデフォルトのフィルター、表示、グループ化を設定できるようになりました。</p> <p>たとえば、[ フィルタ一覧 ] のコントロールを [ すべて ] に設定したままにする代わりに、[ ホームチーム ] に変更することができます。 この方法では、ユーザーがオブジェクトのリストを表示すると、ユーザーのチームに関連付けられたオブジェクトのみが含まれます。</p> <p>以前は、これらのデフォルトはカスタマイズできなかったので、フィルターの場合は常に「すべて」、ビューの場合は「標準」、グループの場合は「なし」に設定されていました。 新しい機能に加えて、これら 3 つの設定が不要な場合に、ユーザーに対して非表示にできる点が特に重要です。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 12 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">管理者向けの新機能：現在カスタムフィールドを使用しているレポートを簡単にリスト</a> </p> <p>一部のWorkfrontレポートに既に実装されているカスタムフィールドを編集または削除する必要がある場合は、変更後も正しく動作するために、それらのレポートに調整が必要かどうかを評価することが重要です。 現在は、セットアップのカスタムForms領域に新しいカスタムフィールドの影響ビューが追加され、このフィールドを使用するレポートを簡単に見つけることができます。</p> <p>このビューがない場合、レポートを実行して、レポートでどのカスタムフィールドが使用されているかを調べる必要がありました。 組織で多くのカスタムフィールドを使用する場合は、これは困難で面倒です。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 19 日<br></p> <p>実稼動版リリース： 2021 年 3 月 5 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for8" class="MCXref xref" xrefformat="{para}">グループ管理者の場合：1 か所でグループとそのオブジェクトを表示、管理する</a> </p> <p>セットアップの [ グループ ] 領域でグループを表示すると、グループを管理しやすくなりました。 新しい「その他」メニューを使用すると、グループページに戻ることなく、グループの編集、コピー、削除をすばやくおこなうことができます。</p> <p>また、グループのページから、グループのレイアウトテンプレート、集計表、タイムシートプロファイル、サブグループメンバを表示し、操作することもできます。 これにより、これらのオブジェクトの様々なセットアップページに移動して、グループの管理を行う必要がなくなります。 また、グループのオブジェクトのリストは、システム内の他のグループのリストとは別に保持されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 19 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">管理者向けの新機能：カスタムフォームフィールドで使用可能なその他のテキスト書式設定オプション</a> </p> <p>書式設定が可能なカスタムフォームフィールドに入力すると、太字、斜体、下線に加えて、箇条書き、段落番号、ハイパーリンク、ブロック引用符を使用してテキストを整理できるようになりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 19 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">プロジェクトヘッダーで使用できる新しいボタン</a> </p> <p>[ プロジェクト ] ページのプロジェクトの一覧をすばやくフィルターできるように、ヘッダーに 2 つの新しいボタンが追加され、[ 自分が所有するプロジェクト ] または [ 自分が所有するプロジェクト ] フィルターをすばやく適用できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 30 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">新しい「イシューの編集」ボックス</a> </p> <p>新しいWorkfrontエクスペリエンスのルックアンドフィールを更新する際に、「問題を編集」ボックスのデザインを変更しました。 個々のイシューから、またはリストから単一のイシューを編集する際に、新しいイシューの編集ボックスにアクセスできます。</p> <p>その他、様々な変更を加え、外観と操作性を更新しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">繰り返しタスクを作成および編集するための新しいインターフェイス</a> </p> <p>「新規タスク」ボックスと「タスクを編集」ボックスの再設計の一環として、新しいタスクを繰り返しタスクにする機能と、繰り返しタスクの親を編集する機能を追加しました。 この機能は、以前にリリースした「新規タスク」(New and Edit Task) ボックスの再設計には含まれていませんでした。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#move" class="MCXref xref" xrefformat="{para}">スクラムボードからストーリーやイシューを移動または削除する</a> </p> <p>ストーリーまたはイシューカードの「その他」アイコンをクリックし、「移動先」を選択して、スクラムボードからストーリーまたはイシューを移動できるようになりました。 以降のイテレーションが定義されている場合は、アイテムを別のイテレーションに移動できます。 また、アイテムをチームのバックログに移動することもできます。</p> <p>また、カードの「その他」アイコンをクリックし、「削除」を選択して、ストーリーやイシューをスクラムボードから直接削除することもできます。 ストーリーまたはイシューを削除すると、30 日間ごみ箱に移動され、システム管理者のみが復元できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#relocate" class="MCXref xref" xrefformat="{para}">「編集」ボックスと「新規オブジェクト」ボックスの「保存」ボタンと「キャンセル」ボタンの位置を変更しました。</a> </p> <p>ユーザーのフィードバックに基づいて、プロジェクトとタスクの「オブジェクトを編集」ボックスと「新しいオブジェクト」ボックスの左下隅に「保存」ボタンと「キャンセル」ボタンを移動しました。 </p> <p>この機能強化の前は、これらのボタンはこれらのボックスの右上隅に配置されていました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">カスタムフォームの機能強化</a> </p> <p>カスタムフォームの入力時の操作性を向上させるため、長いカスタムフィールドラベルの表示方法を改善しました。 全体を表示するのに十分な水平方向のスペースがある場合、これらのラベルは切り捨てられなくなります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 19 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#the" class="MCXref xref" xrefformat="{para}">問題のプライマリ連絡先が「プロジェクトの詳細」領域に表示されるようになりました</a> </p> <p>イシューをプロジェクトに変換すると、そのイシューのリクエスターがプロジェクトに転送され、「変換されたイシュー作成者」フィールドに表示されます。 このフィールドは、プロジェクトの詳細領域、およびプロジェクトのレポートとリストで表示できます。 この情報は、レポートおよびリストでのみ、タスクに対しても表示されます。</p> <p>プロジェクトの新しいWorkfrontエクスペリエンスでこのフィールドを表示するには、レイアウトテンプレートでこのフィールドを有効にする必要があります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 2021 年 3 月 10 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#view" class="MCXref xref" xrefformat="{para}">ポートフォリオ、プログラム、またはチームに割り当てるグループに関する情報を表示します</a> </p> <p>グループをポートフォリオ、プログラム、チームに割り当てる際に、適切なグループを確実に作成できるようになりました。グループ名の横の情報アイコンをクリックすると、グループの上にグループの階層を含むツールチップが表示されます。 グループに設定された詳細に応じて、グループのビジネスリーダーと説明も表示されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#text" class="MCXref xref" xrefformat="{para}">カスタムフィールドのテキスト書式が、すべてのWorkfront Classic リストとレポートに表示されるようになりました</a> </p> <p>Workfront Classic のリストで、リストやレポートを表示する際に、カスタムフィールド内の太字、箇条書き、ハイパーリンクなどのテキスト書式を表示できるようになりました。</p> <p>以前は、Workfront Classic では、テキストの書式設定はプロジェクト、タスク、時間の各リストにのみ表示されていました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">新しい「タスクの編集」ボックス </a> </p> <p>新しいWorkfrontエクスペリエンスのルックアンドフィールを更新する際に、「タスクを編集」ボックスのデザインを変更しました。 個々のタスクから、またはリストから 1 つのタスクを編集する際に、新しい「タスクを編集」ボックスにアクセスできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 2 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">新規タスクボックス</a> </p> <p>新しいWorkfrontエクスペリエンスのルックアンドフィールを更新する際に、新しいタスクボックスのデザインを変更しました。 プロジェクトにタスクを追加する場合は、タスク一覧の上部にある [ 新しいタスク ] をクリックして、[ 新しいタスク ] ボックスにアクセスできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 2 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">使用されなくなったチームのアクティベートを解除</a> </p> <p>使用しなくなったチームを非アクティブ化できるようになりました。 チームを非アクティブ化すると、Workfront内のほとんどの typeahead、検索フィールドまたは共通メニューにそのチームが表示されなくなります。 ただし、チームに関連付けられた履歴データは保持されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 2 日<br></p> <p>実稼動リリース： 2021 年 4 月 16 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#update" class="MCXref xref" xrefformat="{para}">ユーザーがログに記録された時間のタスクと問題を削除できる設定に更新します</a> </p> <p>すべてのオブジェクトにまたがって統一されたエクスペリエンスを提供するために、Workfrontでの「ユーザーによるタスクおよび問題の削除を許可」設定の動作方法を変更しました。 現在は、Workfrontまたはグループ管理者がタスクと問題設定を無効にした場合、ログに記録された時間に関するタスクや問題を含むプロジェクトを削除できなくなりました。 </p> <p>この変更がおこなわれる前に、設定を無効にすると、ユーザーはプロジェクトではなくタスクやイシューを削除するだけでなくなりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 2 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#control" class="MCXref xref" xrefformat="{para}">新しいリクエストに対して実行する割り当てのタイプを制御する</a> </p> <p>一貫性を保つために新しいリクエストを作成する際の「割り当て」フィールドの機能を変更し、ユーザーが入力できる割り当ての種類に関係なく、常に同じフィールドを表示するようにしました。</p> <p>リクエストキューの設定時に、「割り当て先」、「ジョブロール」、または「チーム」の各フィールドを表示すると、リクエスターには、これら 3 つの割り当てタイプのすべてまたはいずれかに対応する同じ「割り当て」フィールドが表示されます。</p> <p>[ 割り当て ] フィールドには、許可される割り当ての種類を示すメッセージが表示されます。 例えば、リクエストキューを設定する際に「割り当て先」フィールドと「チーム」フィールドを有効にすると、「担当者、役割またはチームを検索」ではなく「担当者またはチームを検索」するよう求められます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">リクエストの作成とドラフトの管理の改善</a> </p> <p>新しいWorkfrontエクスペリエンスにリクエストの作成に関するフィードバックを取り入れ続ける中で、新しいリクエストワークフローに対していくつかの改善を行いました。 これには、新しいリクエストを作成する際に「閉じる」ボタンが含まれ、ドラフトやその他の機能強化が失われずにリクエストを終了できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#improvem2" class="MCXref xref" xrefformat="{para}">リクエストワークフローの改善</a> </p> <p>アドビでは、お客様のフィードバックを引き続き聞き、取り込む際に、新しいリクエストワークフローにいくつかの改善を加え、Workfrontとのインタラクションをより簡単かつ直感的にできるようにしました。 リクエストキューの作成時に、ファイルのアップロード用に「ドキュメント」セクションを配置する場所を選択できるようになりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#open" class="MCXref xref" xrefformat="{para}">リクエスト領域の「Submitted」セクションで Summary パネルを開きます。</a> </p> <p>Workfrontのすべての領域でエクスペリエンスの一貫性を保つために、リクエスト領域の「送信済み」セクションに概要を開くアイコンを追加しました。 送信された問題の概要パネルを開き、問題に関する詳細を表示したり、問題を割り当てたり、ドキュメントやコメントを追加したりできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 19 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#bring" class="MCXref xref" xrefformat="{para}">削除した新しい問題フィールドを新しいリクエストフォームに戻す</a> </p> <p>以前のリリースで開始した新しいリクエストフォームのデザインを変更した際に、新しいリクエストを送信する際に、プロジェクトの「Queue Details」セクションの「New Issue Fields」領域に表示される複数のフィールドを非表示にしました。 フィードバックを取り込んだ後、フィールドを取り戻し、すべてのフィールドを新しいリクエストフォームに表示できるようにすることにしました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">リクエスト領域でリクエストを送信する際の新しいエクスペリエンス</a> </p> <p>新しいWorkfrontエクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエスト領域の新しいリクエストボックスのデザインを変更しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日 </p> <p>実稼動版リリース： 21.2 リリースを使用 <span class="uitext" style="color: #dc143c;">（元々は 21.1 リリースに予定されていましたが、21.2 に移行しました）</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#share" class="MCXref xref" xrefformat="{para}">リクエスト送信時のリクエストキューへのリンクの共有</a> </p> <p>リクエストの作成時に、リクエストキュー、トピックグループ、またはキュートピックへのリンクを共有できるようになりました。</p> <p>新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループまたはキュートピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.2 リリースを使用 <span class="uitext" style="color: #dc143c;">（元々は 21.1 リリースに予定されていましたが、21.2 に移行しました）</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#month-le" class="MCXref xref" xrefformat="{para}">ワークロードバランサーの月レベルの表示</a> </p> <p>リソースの割り当てをより長期間管理できるよう、ワークロードバランサーの月レベルの表示を実装しました。 一度に 3 ヶ月まで表示し、月別のリソース割り当てを更新できます。 この変更が行われる前は、1 日または 1 週間のみでワークロード・バランサを表示できました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#connecti" class="MCXref xref" xrefformat="{para}">シナリオ・プランナ、ワークロード・バランサ、タスク・リスト間の接続</a> </p> <p>プロジェクトの戦略的計画に役立ち、シナリオプランナーの大きな構想に合わせるために、プロジェクトに新しい領域を作成しました。プロジェクトには、取り組みからの求人ロール要件と、プロジェクトの作業項目に対する予定時間が表示されます。 この領域は、プロジェクトレベルのワークロードバランサーとタスクリストに使用できます。 この新しい機能をサポートするには、既存の日別および週別オプションに加えて、月別のワークロードバランサーも表示できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#use" class="MCXref xref" xrefformat="{para}">生産資源プランナの正味値を計算する際に計画時間を使用 </a> </p> <p>リソース・プランナの新しい設定では、正味値の計算に計画時間を使用できます。 </p> <p>この機能強化の前は、Workfrontは予算時間のみを使用して正味値を計算しました。 正味値には、「使用可能」と「予算」、「計画時間」、「工数」、「原価」の差が表示されます。 [ 予算時間 ] は、[ 正味値 ] の計算時の既定の設定です。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 12 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#12-week" class="MCXref xref" xrefformat="{para}">ワークロード・バランサの 12 週間表示</a> </p> <p>ワークロードバランサーで最大 12 週間分の情報を表示できるようになりました。 この機能強化がおこなわれる前は、2 週間、4 週間、6 週間の情報を表示できました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 12 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#change" class="MCXref xref" xrefformat="{para}">ワークロードバランサーの未割り当て領域でのジョブロールフィルタの動作方法の変更</a> </p> <p>ワークロードバランサーでのジョブの役割フィルターの動作を改善し、ユーザーの期待に応えるために、未割り当て領域でのフィルターの機能を変更しました。 フィルタで指定したジョブの役割に割り当てられた時間のみを表示できるようになりました。 </p> <p>この強化がおこなわれる前は、「未割り当て」領域に「ジョブの役割」フィルターを適用すると、ワークロードバランサーは、ジョブの役割に割り当てられた作業項目に関連するすべての時間を表示していました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### レポートの機能強化 {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">プロジェクトとレポートでの時間の編集を制限する</a> </p> <p>プロジェクトおよび時間レポートの「時間」タブで時間の編集をより細かく制御できるように、Workfront管理者が時間の編集を時間の所有者およびシステム管理者に制限できる設定を追加しました。</p> <p>以前は、タイムシートと時間がアクセスレベルで有効になっているユーザーが時間を編集する場合がありました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 16 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">更新されたリストおよびレポートの「割り当て」フィールドの新しいルックアンドフィール</a> </p> <p>新しいWorkfrontエクスペリエンスの他の領域の最新の外観に合わせて、更新されたリストとレポートの「割り当て」フィールドのスタイル設定が変更されました。 再設計には、新しいジョブロールアイコン、高度な割り当て用の新しい人物アイコン、新しい制限付きアクセスアイコンなどが含まれます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">更新されたリストおよびレポートの先読みフィールドの新しいルックアンドフィール</a> </p> <p>新しいWorkfrontエクスペリエンスの他の領域の最新の外観に合わせて、更新されたリストとレポートの typeahead フィールドのスタイル設定が変更されました。 これらの変更には、様々な機能強化が含まれます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 9 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用 <span class="uitext" style="color: #dc143c;">（2021 年 5 月 20 日に本番から一時的に削除）</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#report" class="MCXref xref" xrefformat="{para}">システム更新のレポート</a> </p> <p>新しいジャーナルエントリレポートでは、次のようなシステム更新を詳細に調べることで、監査性を高めることができます。プロジェクト、タスク、またはタスクのステータス変更削除されたタスクと問題カスタムフィールドの値；その他</p> <p>以前は、Workfront API を使用してのみ、システムの更新をレポートできました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 19 日<br></p> <p>実稼動版リリース： 2021 年 3 月 5 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-proofing-enhancements.md#proof" class="MCXref xref" xrefformat="{para}">配達確認の決定がドキュメントリストに表示されるようになりました</a> </p> <p>配達確認の全体的な決定が、デフォルトのドキュメントリストビューに表示されるようになりました。</p> <p>この機能強化により、全体的な決定を持つすべての配達確認を、デフォルトのリストビュー内で直接簡単に確認できます。 これにより、別のページに移動する必要なく、配達確認の進行状況を簡単に見つけることができます。</p> <p>以前は、配達確認の決定全体を表示するには、ドキュメントの詳細と配達確認のワークフローに移動する必要がありました（複数回のクリックが必要）。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 16 日<br></p> <p>実稼動リリース： 2021 年 5 月 7 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-proofing-enhancements.md#new" class="MCXref xref" xrefformat="{para}">配達確認の承認レポートの新しいフィールド</a> </p> <p>役に立つ情報を表面的に検証できるように、配達確認の承認レポートに新しいフィールドを追加しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-proofing-enhancements.md#carry" class="MCXref xref" xrefformat="{para}">新しいバージョンを生成する際に既存の配達確認ワークフローを引き継ぐ</a> </p> <p>これで、既存の配達確認ワークフローは、生成方法に関係なく、作成した新しいバージョンに引き継がれます。</p> <p>以前は、Workfrontでの生成場所に応じて、配達確認のワークフローの実行方法に若干の違いがありました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 12 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用<span class="uitext" style="color: #dc143c;"> （プレビューおよび実稼動環境から削除）。この機能は、21.2 リリースではリリースされません )</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 統合の強化 {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p style="color: #dc143c;"><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-integration-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Adobe Workfront for XDの概要</a> </p> <p>新しいプラグインのローンチがお知らせします。Adobe Workfront for XD このプラグインを使用すると、作業項目の詳細にアクセスしたり、更新領域で同僚と共同作業したり、レビュー用に配達確認を送信したりできます。すべてXDを終了する必要はありません。 Adobe XD Marketplace にアクセスし、今すぐプラグインをダウンロードしてください。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 28 日<br></p> <p>実稼動リリース： 2021 年 4 月 28 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-integration-enhancements.md#search" class="MCXref xref" xrefformat="{para}">ドキュメントの統合でフォルダを検索する</a> </p> <p>ドキュメントの統合内容を簡単にナビゲートできるように、フォルダーを検索できるようになりました。 検索バーにキーワードを入力すると、Workfrontは検索語句を名前に含むドキュメント、フォルダ、およびサブフォルダを返すようになりました。</p> <p>以前は、サブフォルダーは親フォルダーを開くことによってのみ配置できました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-integration-enhancements.md#enhanced" class="MCXref xref" xrefformat="{para}">ファイルをGoogle Drive にアップロードする際のセキュリティの強化</a> </p> <p>Google Drive の統合で、新しいGoogleセキュリティプロトコルがサポートされるようになりました。 </p> <p>Workfrontオブジェクトの「ドキュメント」セクションからGoogle Drive にリンク、アップロード、またはファイルを作成する際に、Googleのファイルピッカーを使用してGoogleファイルにアクセスできるようになりました。 これにより、Workfrontのアクセスと表示は、WorkfrontにリンクしたGoogleファイルに限定されます。</p> <p>以前は、Workfrontをベースとするファイルダイアログを通じてファイルにアクセスしていました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 12 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#email" class="MCXref xref" xrefformat="{para}">E メール許可リストの検証</a> </p> <p>E メールアドレスを使用する場合許可リスト、新規および更新されたユーザー E メールアドレスは、に対して検証さ許可リストれます。 新しいユーザーを追加したり、既存のユーザーを編集したりする際に、上にない E メールドメインを入力する許可リストと、E メールメッセージがユーザーに送信されないことを示すメッセージが表示されます。 ユーザープロファイルは保存できますが、ユーザーが E メールを受信するにはドメ許可リストインをドメインに追加する必要があります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">ブループリントベータ版をプレビューで利用できるようになりました</a> </p> <p>ブループリントは、成長する作業管理システムの作成に役立つ基本的な構成要素を提供します。 システム管理者は、ブループリントカタログを参照して、すぐに使用できるプロジェクトテンプレートをインストールできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 4 月 23 日<br></p> <p>実稼動版リリース： 21.3 リリースで一般に入手可能です</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">オブジェクトヘッダーの新しいルックアンドフィール</a> </p> <p>情報の階層をさらに強化し、ユーザーがどのページにあるかをより明確に理解できるように、各オブジェクトヘッダーには次の機能が追加されました。</p> 
    <ul> 
     <li> <p>各オブジェクトタイプのカラフルで最新のアイコン</p> </li> 
     <li> <p>オブジェクトの名前の上にリストされるオブジェクトタイプ</p> </li> 
     <li> <p>更新されたフォントスタイルとテキストサイズ</p> </li> 
     <li> <p>その他の小規模なスタイルの変更</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動版リリース： 2021 年 3 月 10 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">オブジェクトステータスの検索応答の更新</a> </p> <p>Workfrontでは、オブジェクトのステータスが新しい方法で保存されるようになりました。 </p> <p>これらの変更は、ステータス検索リクエストの実行方法には影響しません。 ただし、オブジェクトのステータス検索を含む API リクエストでは、不完全なグループステータスのリストが返されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 26 日<br></p> <p>実稼動版リリース：未定</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#event" class="MCXref xref" xrefformat="{para}">ID で終わるすべてのフィールドが含まれるように更新されたイベント購読ペイロード</a> </p> <p> </p> <p>すべてのイベント購読ペイロードに、「ID」で終わるすべてのフィールドが含まれるようになりました。 </p> <p>各オブジェクトには、ID で終わる一意の関連フィールドのセットが含まれる、独自の関連フィールドのセットが存在することに注意する必要があります。 つまり、各ペイロードには、ID で終わる、そのオブジェクトに関連するすべてのフィールドが含まれますが、各オブジェクトには、ID で終わる異なるフィールドセットがあります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 3 月 26 日<br></p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-mobile-enhancements.md#timeshee" class="MCXref xref" xrefformat="{para}">タイムシートコメント</a> </p> <p>モバイルアプリで、タイムシートにコメントを入力できるようになりました。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：なし</p> <p>実稼動版リリース： 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-mobile-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">typeahead でサポートされる追加のオブジェクト — iOSユーザーのみ</a> </p> <p>カスタムフォームの typeahead フィールドで、より多くのオブジェクトがモバイルアプリでサポートされるようになりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動リリース： 2021 年 4 月 28 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>iOSモバイルアプリ</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-mobile-enhancements.md#save" class="MCXref xref" xrefformat="{para}">Workfrontモバイルアプリで要求をドラフトとして保存する</a> </p> <p>一部入力済みの要求をモバイルアプリでドラフトとして保存できるようになりました。 リクエスト領域に新しい「ドラフト」セクションが追加され、任意のドラフトを簡単に検索できるようになりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 2 月 26 日<br></p> <p>実稼動リリース：iOS:2021 年 4 月 27 日；Android: 21.2 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>iOSモバイルアプリ</p> <p>Android モバイルアプリ</p> </td> 
  </tr> 
 </tbody> 
</table>

 

## Workfront目標の強化

21.2 リリースでのWorkfront Goals リリースに向けての最新機能。 プレビューで利用できる新機能について詳しくは、 [Adobe Workfront 21.2 リリースでの目標](../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md).

## Workfront Scenario Planner の機能強化

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

21.2 リリースでのWorkfront Scenario Planner リリースに加わる新機能です。 プレビューで利用できる新機能について詳しくは、 [21.2 リリースのAdobe Workfrontシナリオプランナー](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-2.md).

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境では 21.2 リリーススケジュール以外のサイクルで使用できます。 最新の機能について詳しくは、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API バージョン 13

API バージョン 13 では、様々なリソースとエンドポイントを変更しました。 一部の変更は新しい機能をサポートし、他の変更では、API を通じて入手可能な情報を使いやすくします。

の新機能と更新点について詳しくは、 [API バージョン 13 の新機能](../../../wf-api/api/new-api-version-13.md).

## 実稼動から削除される機能

### 機能のロールバック：新しいバージョンを生成する際に既存の配達確認ワークフローを引き継ぐ

お客様のご意見により、 **Workfrontは、2021 年 3 月 30 日のプレビュー環境から、2021 年 3 月 31 日の実稼動環境から、この変更を削除します。**.

2021 年 3 月 12 日に、Workfrontは、Workfront Classic と新しいWorkfrontエクスペリエンスの両方の既存の配達確認ワークフローに対する変更をリリースしました。 既存のワークフローで、ユーザーが作成した新しい配達確認バージョンに引き継ぐことができる変更（その方法は関係ありません）。

この変更が削除された後の新しいWorkfrontエクスペリエンスでは、シンプルな配達確認の選択で作成された配達確認に、事前設定済みの校正設定が含まれず、新しいバージョンでは既存のワークフローや配達確認設定は引き継がれません。 ユーザーは、配達確認の生成後に設定を調整できます。

この変更が削除された後、Workfront Classic では、「配達確認を生成」オプションに事前設定済みの校正設定が含まれず、新しいバージョンでは既存のワークフローや配達確認設定が引き継がれません。 ユーザーは、配達確認の生成後に設定を調整できます。

既存のワークフローを簡単にコピーするのと同様の機能が、将来実稼動環境に追加される可能性があります。

## サポートされなくなった機能

### Internet Explorer 11

Internet Explorer のサポートが削除され、WorkfrontはMicrosoft Edge を正式にサポートするようになりました。

サポートされているブラウザーについて詳しくは、 [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

 
