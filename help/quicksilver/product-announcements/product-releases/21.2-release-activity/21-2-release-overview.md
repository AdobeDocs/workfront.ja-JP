---
content-type: release-notes
keywords: メモ、四半期、更新
navigation-topic: product-releases
title: 21.2 リリースの概要
description: 21.2 リリースは、2021年5月10日（PT）の週に、実稼動環境で使用可能になりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1affe1ae-571e-4026-8ba7-8ce7104e1b89
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '5544'
ht-degree: 100%

---

# 21.2 リリースの概要

21.2 リリースは、2021年5月10日（PT）の週に、実稼動環境で使用可能になりました。

このページには、Adobe Workfront Classic と、21.2 リリースに含まれる新しい Adobe Workfront エクスペリエンスの両方の機能に関する情報が提供されており、生産性とコラボレーションの実現に役立ちます。

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

## Adobe Workfront の機能強化

* [ブランディングの変更 - Adobe Workfront](#branding-changes-adobe-workfront)
* [管理者の機能強化](#administrator-enhancements)
* [プロジェクトの機能強化](#project-enhancements)
* [リクエストの機能強化](#requests-enhancements)
* [リソース管理の機能強化](#resource-management-enhancements)
* [レポートの機能強化](#reporting-enhancements)
* [プルーフの機能強化](#proofing-enhancements)
* [統合の機能強化](#integration-enhancements)
* [その他の機能強化](#other-enhancements)
* [モバイルの機能強化](#mobile-enhancements)

### ブランディングの変更 - Adobe Workfront {#branding-changes-adobe-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#we" class="MCXref xref" xrefformat="{para}">正式に Adobe Workfront になりました</a> </p> <p>Workfront は Adobe Workfront としてブランド変更されました。Adobe Workfront アプリケーションと、お客様向け web サイトの最も重要な部分が新しくなりました。</p> <p>今後数週間で、この新しいブランディングが他の場所（モバイルのプルーフアプリやブラウザータブのお気に入りなど）にも反映されます。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月27日（PT）<br></p> <p>実稼動リリース：2021年4月27日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 管理者機能の強化 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for3" class="MCXref xref" xrefformat="{para}">管理者向け：Workfront のその他の多くのエリアに関する監査ログ情報の表示</a> </p> <p>監査ログエリアで、Workfront 全体の様々なエリアで変更を追跡し、トラブルシューティングができるようになりました。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for4" class="MCXref xref" xrefformat="{para}">グループ管理者向け：サブグループを移動するためのコントロールの改善およびツールバーの更新</a> </p> <p>設定の「サブグループ」エリアで、次の改善を行いました。</p> 
    <ul> 
     <li> <p>管理するグループを簡単に整理するために、「サブグループを追加」ツールバーボタンを追加し、新しいサブグループの作成や既存のサブグループの移動ができるようになりました。</p> </li> 
     <li> <p>「サブグループ」エリアのツールバーのリストが、新しい Workfront エクスペリエンスの他の最新化されたリストと統一されました。グループを選択すると、ツールバーで使用可能な機能がアイコンで表されます。</p> </li> 
    </ul> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">管理者向けの新機能：タイムシートと時間の環境設定ページのルックアンドフィールを更新</a> </p> <p>タイムシート設定と時間設定ページのエクスペリエンスを向上させるために、ユーザーインターフェイスを更新し、Workfront 全体でより最新のルックアンドフィールに合わせました。</p> <p>セクションと個々のオプションは、より縦のスペースで区切られているので、読みやすくなります。</p> <p>2 つのラジオボタンオプションのラベルは、それほど長くはないように分割されます。各ラベルの 2 番目の部分は、別々の行の情報メッセージになります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">グループ管理者向け：グループエリアでの改善リストの表示</a> </p> <p>設定のグループエリアで次の 2 つの機能が強化され、新しい Workfront エクスペリエンスの他の最新のリストと一貫性のあるリストが作成されました。</p> 
    <ul> 
     <li> <p>グループを選択すると、ツールバーで使用可能な機能がアイコンで表されます。</p> </li> 
     <li> <p>グループ、列、並べ替えおよび階層のリストでは、他のリストで慣れ親しんだ新しいルックアンドフィールとなりました。また、デフォルトでは、1 つのページに、100 個ではなく、最大 2,000 個の項目が表示されます。</p> </li> 
    </ul> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for2" class="MCXref xref" xrefformat="{para}">グループ管理者向け：設定のグループエリアでプログラムを作成および編集</a> </p> <p>アドビでは、グループとその関連オブジェクトを 1 か所で容易に管理できるように引き続き取り組んでいます。設定のグループエリアから、グループのプログラムを表示して操作できるようになりました。これにより、グループのプログラムを管理するためにプログラムエリアに移動する必要がなくなります。また、作業中のグループプログラムのリストを、システム内の他のプログラムとは別に保持します。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for5" class="MCXref xref" xrefformat="{para}">管理者向け：設定エリアの更新されたヘッダー</a> </p> <p>管理者のために設定エリアの使いやすさを向上し、Workfront 全体の一貫性を維持するために、各設定ページとサブページを示す大きなカラフルなバッジ、フォントのスタイルとサイズの最新化など、様々なアップデートを加えて設定ヘッダーを更新しました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月1日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for6" class="MCXref xref" xrefformat="{para}">グループ管理者向け：グループページでより多くのグループオブジェクトを表示および管理</a> </p> <p>アドビでは、グループとその関連オブジェクトを 1 か所で容易に管理できるように引き続き取り組んでいます。設定のグループエリアから、グループの会社、チームおよびポートフォリオを表示および操作できるようになりました。これにより、これらのオブジェクトの様々な設定ページに移動して、グループの管理を行う必要がなくなります。表示するグループオブジェクトのリストをシステム内の他のグループのリストとは別に保持します。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">グループ管理者向けの新機能：グループタイムシートプロファイルの割り当て</a> </p> <p>管理するグループのタイムシートプロファイルを管理しやすくなりました。タイムシートプロファイルを作成できるだけでなく、自分のグループに割り当てたり、自分のグループの個々のメンバーに割り当てたりすることもできます。これは、アクセスレベルでタイムシートと時間オプションが有効になっていない場合でも当てはまります。</p> <p>これまで、タイムシートプロファイルを割り当てるには、「タイムシートと時間」オプションを有効にする必要がありました。ただし、システム内のすべてのタイムシートと時間情報に対する表示と編集のアクセス権を付与することになるため、すべてのグループ管理者にとっては理想的ではない場合がありました。このレベルのアクセス権が必要ない場合、グループのタイムシートプロファイルを管理できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月11日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for7" class="MCXref xref" xrefformat="{para}">管理者向け：オブジェクトリストでユーザーに表示するフィルター、ビューおよびグループ化の設定</a><span class="uitext" style="color: #dc143c;"></span> </p> <p>新しい Workfront エクスペリエンスのレイアウトテンプレートを使用すると、Workfront 全体のオブジェクトリストでユーザーに表示されるデフォルトのフィルター、ビューおよびグループ化を設定できるようになりました。</p> <p>例えば、フィルターのリスト制御の設定を「すべて」のままにせず、「ホームチーム」に変更できます。この方法では、ユーザーがオブジェクトのリストを表示すると、ユーザーのチームに関連付けられたオブジェクトのみが含められます。</p> <p>以前は、これらのデフォルトはカスタマイズできなかったので、フィルターの場合は常に「すべて」、ビューの場合は「標準」、グループ化の場合は「なし」に設定されていました。新しい機能に加えて、これら 3 つの設定が不要な場合に、ユーザーに対して非表示にできる点が特に重要です。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月11日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">管理者向けの新機能：現在カスタムフィールドを使用しているレポートを簡単にリスト</a> </p> <p>一部の Workfront レポートに既に実装されているカスタムフィールドを編集または削除する必要がある場合は、変更後も正常に機能し続けるために、それらのレポートに調整が必要かどうかを評価することが重要です。現在は、設定のカスタムフォームエリアに新しいカスタムフィールドの影響ビューが追加され、このフィールドを使用するレポートを簡単に見つけることができます。</p> <p>このビューがない場合では、レポートを実行して、レポートでどのカスタムフィールドが使用されているかを調べる必要がありました。組織で多くのカスタムフィールドを使用する場合は、これは困難で面倒な作業でした。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年2月18日（PT）<br></p> <p>実稼動版リリース：2021年3月4日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#for8" class="MCXref xref" xrefformat="{para}">グループ管理者向け：グループとそのオブジェクトを 1 か所で表示および管理</a> </p> <p>設定のグループエリアでグループを表示すると、グループを管理しやすくなりました。新しいその他メニューを使用すると、グループページに戻ることなく、グループの編集、コピーまたは削除をすばやく行うことができます。</p> <p>また、グループのページから、グループのレイアウトテンプレート、スケジュール、タイムシートプロファイルおよびサブグループメンバーを表示し、操作することもできます。これにより、これらのオブジェクトの様々な設定ページに移動して、グループの管理を行う必要がなくなります。また、グループのオブジェクトのリストは、システム内の他のグループのリストとは別に保持されます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年2月18日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-admin-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">管理者向けの新機能：カスタムフォームフィールドで使用できるその他のテキスト形式オプション</a> </p> <p>形式設定が可能なカスタムフォームフィールドに入力すると、太字、斜体、下線に加えて、箇条書き、段落番号、ハイパーリンク、ブロック引用符を使用してテキストを整理できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年2月18日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">プロジェクトヘッダーで使用できる新しいボタン</a> </p> <p>プロジェクトページのプロジェクトのリストをすばやくフィルターできるように、ヘッダーに 2 つの新しいボタンが追加され、担当プロジェクトフィルターまたは所有プロジェクトフィルターをすばやく適用できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月29日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">新しい「イシューを編集」ボックス</a> </p> <p>新しい Workfront エクスペリエンスのルックアンドフィール更新の一環として、「イシューを編集」ボックスのデザインを変更しました。個々のイシューからまたはリストから個々のイシューを編集する際に、新しい「イシューを編集」ボックスにアクセスできます。</p> <p>その他、様々な変更を加え、ルックアンドフィールを更新しました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">繰り返しタスクを作成および編集するための新しいインターフェイス</a> </p> <p>「新規」ボックスと「タスクの編集」ボックスのデザイン変更の一環として、新規タスクを繰り返しタスクにする機能と、繰り返しタスクの親を編集する機能を追加しました。この機能は、以前にリリースした「新規」ボックスおよび「タスクの編集」ボックスのデザイン変更には含まれていませんでした。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#move" class="MCXref xref" xrefformat="{para}">スクラムボードからストーリーやイシューを移動または削除する</a> </p> <p>ストーリーまたはイシューカードのその他アイコンをクリックし、「指定の場所に移動」を選択して、スクラムボードからストーリーまたはイシューを移動できるようになりました。以降のイテレーションが定義されている場合は、項目を別のイテレーションに移動できます。また、項目をチームのバックログに移動することもできます。</p> <p>また、カードのその他アイコンをクリックし、「削除」を選択して、ストーリーやイシューをスクラムボードから直接削除することもできます。ストーリーやイシューを削除すると、30 日間ごみ箱に移動され、システム管理者のみが復元できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#relocate" class="MCXref xref" xrefformat="{para}">「編集」ボックスと「新規オブジェクト」ボックスの「保存」ボタンと「キャンセル」ボタンの位置変更</a> </p> <p>ユーザーのフィードバックに基づいて、「保存」ボタンと「キャンセル」ボタンを、プロジェクトとタスクの「オブジェクトを編集」ボックスと「新しいオブジェクト」ボックスの左下隅に移動しました。 </p> <p>この機能強化の前は、これらのボタンはこれらのボックスの右上隅に配置されていました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#custom" class="MCXref xref" xrefformat="{para}">カスタムフォームの機能強化</a> </p> <p>カスタムフォームの入力時の操作性を向上させるために、長いカスタムフィールドラベルの表示方法を改善しました。全体を表示するのに十分な水平方向のスペースがある場合、これらのラベルは切り詰められなくなります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月18日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#the" class="MCXref xref" xrefformat="{para}">イシューのプライマリ連絡先がプロジェクトの詳細エリアに表示されるようになりました</a> </p> <p>イシューをプロジェクトに変換すると、そのイシューのリクエスターがプロジェクトに転送され、変換済みイシューの発信元フィールドに表示されます。このフィールドは、プロジェクトの詳細エリア、およびプロジェクトのレポートとリストで表示できます。この情報は、レポートおよびリストでのみ、タスクに対しても表示されます。</p> <p>プロジェクトの新バージョンの Workfront でこのフィールドを表示するには、レイアウトテンプレートでこのフィールドを有効にする必要があります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：2021年3月10日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#view" class="MCXref xref" xrefformat="{para}">ポートフォリオ、プログラム、またはチームに割り当てるグループに関する情報を表示</a> </p> <p>グループをポートフォリオ、プログラム、またはチームに割り当てるときに、適切なグループがあることをより簡単に確認できるようになりました。グループ名の横にある「情報」アイコンをクリックすると、その上位のグループの階層とそのグループの管理者を含むツールチップが表示されます。グループに設定された詳細に応じて、グループのビジネスリーダーと説明も表示されます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#text" class="MCXref xref" xrefformat="{para}">カスタムフィールドのテキスト書式が、すべての Workfront Classic リストとレポートに表示されるようになりました</a> </p> <p>Workfront Classic のリストで、リストやレポートを表示する際に、カスタムフィールド内の太字、箇条書き、ハイパーリンクなどのテキスト書式を表示できるようになりました。</p> <p>Workfront Classic で以前は、テキストの書式設定はプロジェクト、タスク、時間数の各リストにのみ表示されていました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">新しいタスクを編集ボックス</a> </p> <p>新しいバージョンの Workfront のルックアンドフィールをアップデートする際に、イシューを編集ボックスのデザインを変更しました。個々のタスクから、またはリストから 1 つのタスクを編集する際に、新しい「タスクを編集」ボックスにアクセスできます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月1日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">新しいタスクボックス</a> </p> <p>新しいバージョンの Workfront のルックアンドフィールをアップデートする際に、新しいタスクボックスのデザインを変更しました。プロジェクトにタスクを追加する場合は、タスクリストの上部にある「新規タスク」をクリックして、「新規タスク」ボックスにアクセスできます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月1日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">使用されなくなったチームの非アクティブ化</a> </p> <p>使用しなくなったチームを非アクティブ化できるようになりました。チームを非アクティブ化すると、Workfront 内のほとんどの typeahead、検索フィールドまたは共通メニューにそのチームが表示されなくなります。ただし、チームに関連付けられた履歴データは保持されます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月1日（PT）<br></p> <p>実稼動版リリース：2021年4月15日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-project-enhancements.md#update" class="MCXref xref" xrefformat="{para}">ユーザーがログに記録された時間のタスクとイシューを削除できる設定に更新</a> </p> <p>すべてのオブジェクトにまたがって統一されたエクスペリエンスを提供するために、Workfront での「ユーザーに対して、時間が記録されたタスクとイシューの削除を許可する」設定の動作方法を変更しました。現在は、Workfront 管理者またはグループ管理者がタスクおよびイシュー設定を無効にした場合、ログに記録された時間に関するタスクやイシューを含むプロジェクトを削除できなくなりました。 </p> <p>この変更以前は、設定を無効にすると、ユーザーは、プロジェクトではなく、タスクやイシューを削除できなくなっていました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月1日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

### リクエストの機能強化 {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#control" class="MCXref xref" xrefformat="{para}">新しいリクエストに対して実行する割り当てのタイプを制御</a> </p> <p>一貫性を保ち、ユーザーが入力できる割り当ての種類に関係なく、常に同じフィールドを表示するために、新しいリクエストを作成する際の「割り当て」フィールドの機能を変更しました。</p> <p>リクエストキューの設定時に「割り当て先」、「担当業務」または「チーム」の各フィールドを有効にすると、要求者には、これら 3 つの割り当てタイプのすべてまたはいずれかに対応する同じ「割り当て」フィールドが表示されます。</p> <p>「割り当て」フィールドには、許可される割り当ての種類が表示されます。例えば、リクエストキューを設定する際に「割り当て先」フィールドと「チーム」フィールドを有効にすると、「担当者、役割またはチームを検索」ではなく「担当者またはチームを検索」するよう求められます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">リクエストの作成とドラフトの管理の改善</a> </p> <p>新しい Workfront エクスペリエンスにおいて、リクエストの作成に関するフィードバックを取り入れ続ける中で、新しいリクエストワークフローに対していくつかの改善を行いました。これには、新しいリクエストを作成する際に「閉じる」ボタンが含まれ、ドラフトやその他の機能強化が失われずにリクエストを終了できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#improvem2" class="MCXref xref" xrefformat="{para}">リクエストワークフローの改善</a> </p> <p>アドビでは、お客様のフィードバックを大切に受け止め、新しいリクエストワークフローにいくつかの改善を加え、Workfront とのインタラクションをより簡単かつ直感的にできるようにしました。リクエストキューの作成時に、ファイルのアップロード用に「ドキュメント」セクションを配置する場所を選択できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#open" class="MCXref xref" xrefformat="{para}">リクエストエリアの「送信済み」セクションで概要パネルを開く</a> </p> <p>Workfront のすべてのエリアでのエクスペリエンスの一貫性を保つために、リクエストエリアの「送信済み」セクションに概要を開くアイコンを追加しました。送信済みのイシューの概要パネルを開き、イシューに関する詳細を表示したり、イシューを割り当てたり、ドキュメントやコメントを追加したりできます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月18日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#bring" class="MCXref xref" xrefformat="{para}">新規リクエストフォームで削除された「新規イシュー」フィールドの復活</a> </p> <p>以前のリリースの新規リクエストフォームのデザイン変更で、新規リクエストの送信時に、プロジェクトの「キューの詳細」セクションの「新規イシュー」フィールド領域に表示される複数のフィールドを非表示にしました。お客様のフィードバックを考慮した上で、フィールドの復活を決定し、すべてのフィールドを新規リクエストフォームに表示できるようにしました。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#new" class="MCXref xref" xrefformat="{para}">リクエスト領域でリクエストを送信する際の新しいエクスペリエンス</a> </p> <p>新しい Workfront エクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエストエリアの「新規リクエスト」ボックスのデザインを変更しました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月13日 </p> <p>実稼動版リリース：21.2 リリースを使用<span class="uitext" style="color: #dc143c;">（元々は 21.1 リリースに予定されていましたが、21.2 に移行しました）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-requests-enhancements.md#share" class="MCXref xref" xrefformat="{para}">リクエスト送信時のリクエストキューへのリンクを共有</a> </p> <p>リクエストの作成時に、リクエストキュー、トピックグループ、またはキューのトピックへのリンクを共有できるようになりました。</p> <p>新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループ、またはキューのトピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース：21.2 リリースを使用<span class="uitext" style="color: #dc143c;">（元々は 21.1 リリースに予定されていましたが、21.2 に移行しました）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#month-le" class="MCXref xref" xrefformat="{para}">ワークロードバランサーの月レベルの表示</a> </p> <p>リソースの割り当てをより長期間管理できるよう、ワークロードバランサーの月レベルの表示を実装しました。一度に 3 か月まで表示し、月別のリソース割り当てをアップデートできます。この変更以前は、1 日または 1 週間のみでワークロードバランサーを表示できました。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#connecti" class="MCXref xref" xrefformat="{para}">シナリオプランナー、ワークロードバランサー、タスクリスト間の接続</a> </p> <p>プロジェクトの戦略的計画に役立ち、シナリオプランナーの大きな構想に合わせるために、プロジェクトに新しいエリアを作成しました。その領域には、イニチアチブからの担当業務要件と、プロジェクト作業アイテムで予測される予定時間数が表示されます。このエリアは、プロジェクトレベルのワークロードバランサーとタスクリストに使用できます。この新しい機能をサポートするには、既存の日別および週別オプションに加えて、月別のワークロードバランサーも表示できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#use" class="MCXref xref" xrefformat="{para}">リソースプランナーの正味価値を計算する際に予定時間数を使用</a> </p> <p>リソースプランナーの新しい設定を使用すると、正味価値の計算に予定時間数を使用できます。 </p> <p>この機能強化の前は、Workfront は予算計上時間数のみを使用して正味価値を計算しました。正味価値には、利用可能時間数と予算計上時間数または予定時間数、FTE、コストとの差が表示されます。正味価値を計算する場合、予算計上時間数は依然としてデフォルト設定です。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月11日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#12-week" class="MCXref xref" xrefformat="{para}">ワークロードバランサーの 12 週間表示</a> </p> <p>ワークロードバランサーで最大 12 週間分の情報を表示できるようになりました。この機能強化がおこなわれる前は、2 週間、4 週間、6 週間の情報を表示できました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月11日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-resource-management-enhancements.md#change" class="MCXref xref" xrefformat="{para}">ワークロードバランサーの未割り当てエリアでの担当業務フィルターの動作方法の変更</a> </p> <p>ワークロードバランサーでの担当業務フィルターの動作を改善し、ユーザーの期待に応えるために、未割り当てエリアでのフィルターの機能を変更しました。フィルターで指定した担当業務に割り当てられた時間のみを表示できるようになりました。 </p> <p>この強化が行われる前は、未割り当てエリアに担当業務フィルターを適用すると、ワークロードバランサーは、担当業務に割り当てられた作業アイテムに関連するすべての時間数を表示していました。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">プロジェクトとレポートでの時間の編集を制限</a> </p> <p>プロジェクトおよび時間レポートの「時間」タブで時間編集をより詳細に制御できるようにするために、Workfront 管理者が時間の編集を、時間の所有者およびシステム管理者に制限できる設定を追加しました。</p> <p>以前は、タイムシートと時間がアクセスレベルで有効になっているユーザーが時間を編集する場合がありました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月15日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">アップデートされたリストおよびレポートの「割り当て」フィールドの新しいルックアンドフィール</a> </p> <p>新しい Workfront エクスペリエンスの他のエリアの最新のルックに合わせて、更新されたリストとレポートの「割り当て」フィールドのスタイル設定が変更されました。再設計には、新しい「担当業務」アイコン、詳細な割り当て用の新しい「ユーザー」アイコン、新しい制限付き「アクセス」アイコンなどが含まれます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用 </p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">アップデートされたリストおよびレポートの先行入力フィールドの新しいルックアンドフィール</a> </p> <p>新しい Workfront エクスペリエンスの他のエリアの最新のルックに合わせて、更新されたリストとレポートの先行入力フィールドのスタイル設定が変更されました。これらの変更には、様々な機能強化が含まれます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月8日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用<span class="uitext" style="color: #dc143c;">（2021年5月20日（PT）に実稼動版から一時的に削除）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-reporting-management-enhancements.md#report" class="MCXref xref" xrefformat="{para}">システムのアップデートに関するレポート</a> </p> <p>新しいジャーナルエントリレポートでは、プロジェクト、タスクまたはイシューのステータス変更、削除されたタスクおよびイシュー、カスタムフィールドの値など、システムアップデートを詳細に調べることにより、監査性を高めることができます。</p> <p>以前は、Workfront API を使用してのみ、システムのアップデートをレポートできました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年2月18日（PT）<br></p> <p>実稼動版リリース：2021年3月4日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### プルーフ機能の強化 {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-proofing-enhancements.md#proof" class="MCXref xref" xrefformat="{para}">プルーフ決定をドキュメントリストに表示</a> </p> <p>全体的なプルーフ決定が、デフォルトのドキュメントリストビューに表示されるようになりました。</p> <p>この機能強化により、全体的な決定を持つすべてのプルーフを、デフォルトのリストビュー内で直接簡単に確認できます。これにより、別のページに移動する必要なく、プルーフの進捗状態を簡単に見つけることができます。</p> <p>以前は、プルーフ決定の全体を表示するには、ドキュメント詳細とプルーフワークフローに移動する必要がありました（複数回のクリックが必要）。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年4月15日（PT）<br></p> <p>実稼動版リリース：2021年5月6日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-proofing-enhancements.md#new" class="MCXref xref" xrefformat="{para}">プルーフ承認レポートの新しいフィールド</a> </p> <p>役に立つ情報を表面的に検証できるように、プルーフ承認レポートに新しいフィールドを追加しました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-proofing-enhancements.md#carry" class="MCXref xref" xrefformat="{para}">新しいバージョンの生成時に既存プルーフワークフローを継承</a> </p> <p>これで、既存のプルーフワークフローは、生成方法に関係なく、作成した新しいバージョンに引き継がれます。</p> <p>以前は、Workfront での生成場所に応じて、プルーフワークフローの引き継ぎ方法に若干の違いがありました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月11日（PT）<br></p> <p>実稼動版リリース：21.2 リリース<span class="uitext" style="color: #dc143c;">（プレビューおよび実稼動環境から削除されました。この機能は 21.2 リリースではリリースされません）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 統合の機能強化 {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p style="color: #dc143c;"><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-integration-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Adobe Workfront for XD の概要</a> </p> <p>新しいプラグインである Adobe Workfront for XD がリリースされました。このプラグインを使用すると、作業アイテムの詳細にアクセスしたり、更新エリアで同僚と共同作業したり、レビュー用にプルーフを送信したりできます。すべて XD を終了する必要はありません。Adobe XD Marketplace にアクセスし、今すぐプラグインをダウンロードしてください。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月27日（PT）<br></p> <p>実稼動リリース：2021年4月27日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-integration-enhancements.md#search" class="MCXref xref" xrefformat="{para}">ドキュメントの統合でフォルダーを検索する</a> </p> <p>ドキュメントの統合を簡単にナビゲートできるように、フォルダーを検索できるようになりました。検索バーにキーワードを入力すると、Workfront は検索語句を名前に含むドキュメント、フォルダーおよびサブフォルダーを返すようになりました。</p> <p>以前は、サブフォルダーは親フォルダーを開かない限り見つけることはできませんでした。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-integration-enhancements.md#enhanced" class="MCXref xref" xrefformat="{para}">ファイルを Google Drive にアップロードする際のセキュリティの強化</a> </p> <p>Google Drive の統合で、新しい Google セキュリティプロトコルがサポートされるようになりました。 </p> <p>Workfront オブジェクトの「ドキュメント」セクションから Google Drive にファイルをリンク、アップロードまたは作成する際に、Google のファイルピッカーを使用して Google ファイルにアクセスできるようになりました。これによって、Workfront のアクセスと表示は、Workfront にリンクした Google ファイルに対してのみ制限されます。</p> <p>以前は、Workfront をベースとするファイルダイアログを通じてファイルにアクセスしていました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月11日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#email" class="MCXref xref" xrefformat="{para}">メール許可リスト検証</a> </p> <p>メールの許可リストを使用する場合、新規および更新されたユーザーのメールアドレスが許可リストに対して検証されるようになりました。ユーザーを新しく追加したり、既存のユーザーを編集したりする際に、許可リストにないメールドメインを入力すると、そのユーザーにはメールが送信されないことを通知するメッセージが表示されます。そのユーザーのプロファイルは保存できますが、ユーザーがメールを受信できるようにするには、そのドメインを許可リストに追加する必要があります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">ブループリントベータ版をプレビュー環境で利用可能</a> </p> <p>ブループリントは、ユーザーとともに成長する作業管理システムを作成するのに役立つ基本的な構成要素を提供します。システム管理者は、ブループリントカタログを参照して、すぐに使えるプロジェクトテンプレートをインストールできます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年4月22日（PT）<br></p> <p>実稼動版リリース：21.3 リリースで一般に利用可能</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">オブジェクトヘッダーの新しいルックアンドフィール</a> </p> <p>情報の階層をさらに強化し、ユーザーがどのページにいるかをより明確に理解できるように、各オブジェクトヘッダーに以下が追加されました。</p> 
    <ul> 
     <li> <p>各オブジェクトタイプのカラフルで最新のアイコン</p> </li> 
     <li> <p>オブジェクト名の上に表示されるオブジェクトタイプ</p> </li> 
     <li> <p>新しくなったフォントスタイルとテキストサイズ</p> </li> 
     <li> <p>その他の小規模なスタイル変更</p> </li> 
    </ul> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動版リリース：2021年3月10日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">オブジェクトステータス検索の応答の更新</a> </p> <p>Workfront でオブジェクトステータスが新しい方法で保存されるようになりました。 </p> <p>これらの変更は、ステータス検索リクエストの実行方法には影響しません。ただし、オブジェクトステータスの検索を含む API リクエストでは、不完全なグループステータスのリストが返されます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月25日（PT）<br></p> <p>実稼動リリース：未定</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-other-enhancements.md#event" class="MCXref xref" xrefformat="{para}">ID で終わるすべてのフィールドが含まれるようにイベントサブスクリプションのペイロードを更新</a> </p> <p> </p> <p>すべてのイベントサブスクリプションのペイロードに、「ID」で終わるすべてのフィールドが含まれるようになりました。 </p> <p>各オブジェクトには、独自の一連の関連フィールドが存在することに注意する必要があります。これには、ID で終わる一連のユニークな関連フィールドが含まれます。つまり、各ペイロードには、ID で終わる、そのオブジェクトの関連フィールドがすべて含まれますが、各オブジェクトには、ID で終わる別の一連のフィールドがあります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年3月25日（PT）<br></p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### モバイルの機能強化 {#mobile-enhancements}

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
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：なし</p> <p>実稼動版リリース：21.2 リリースを使用</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-mobile-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">先行入力を使用できる追加のオブジェクト - iOS ユーザーのみ</a> </p> <p>モバイルアプリでは、カスタムフォームの先行入力フィールドで使用できるオブジェクトが増えました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動リリース：2021年4月27日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>iOS モバイルアプリ</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.2-release-activity/21-2-mobile-enhancements.md#save" class="MCXref xref" xrefformat="{para}">Workfront モバイルアプリでリクエストの下書きを保存する</a> </p> <p>途中まで入力したリクエストをモバイルアプリで下書きとして保存できるようになりました。リクエストエリアに新しく「下書き」セクションを追加し、下書きを簡単に検索できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年2月25日（PT）<br></p> <p>実稼動リリース：iOS：2021年4月27日（PT）、Android：21.2 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>iOS モバイルアプリ</p> <p>Android モバイルアプリ</p> </td> 
  </tr> 
 </tbody> 
</table>

 

## Workfront Goals の強化

21.2 リリースでの Workfront Goals リリースに向けての最新機能。プレビュー環境で利用できる新機能について詳しくは、[Adobe Workfront Goals 21.2 リリース](../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md)を参照してください。

## Workfront シナリオプランナーの機能強化

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are no Scenario Planner updates at this point in the release. This area will be updated when updates are available.</p>
-->

21.2 リリースでの Workfront Scenario Planner リリースに加わる新機能です。プレビュー環境で利用できる新機能について詳しくは、[Adobe Workfront Scenario Planner 21.2 リリース](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-2.md)を参照してください。

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、21.2 リリーススケジュール以外のタイミングで実稼動環境で利用可能になります。最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

## API バージョン 13

API バージョン 13 では、様々なリソースとエンドポイントを変更しました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

新機能と更新点について詳しくは、[API バージョン 13 の新機能](../../../wf-api/api/new-api-version-13.md)を参照してください。

## 実稼動環境から削除される機能

### ロールバックの機能：新しいバージョン生成時に既存のプルーフワークフローを継承

お客様からのフィードバックに基づき、**Workfront は、2021年3月30日（PT）にプレビュー環境から、2021年3月31日（PT）に実稼動環境から、この変更を削除します**。

2021年3月11日（PT）に、Workfront は、Workfront Classic と新しい Workfront エクスペリエンスの両方の既存のプルーフワークフローに対する変更をリリースしました。既存のワークフローにおける変更は、ユーザーが作成した新しいプルーフバージョンで、その作成方法にかかわらず、引き継ぐことができます。

この変更が削除された後の新しい Workfront エクスペリエンスでは、シンプルなプルーフの選択で作成されたプルーフに、事前設定済みのプルーフの設定が含まれず、新しいバージョンでは既存のワークフローやプルーフ設定は引き継がれません。ユーザーは、プルーフの生成後に設定を調整できます。

この変更が削除された後、Workfront Classic では、「プルーフを生成」オプションに事前設定されたプルーフの設定が含まれず、新しいバージョンでは既存のワークフローやプルーフの設定が引き継がれません。ユーザーは、プルーフの生成後に設定を調整できます。

既存のワークフローを簡単にコピーするのと同様の機能が、今後実稼動環境に追加される可能性があります。

## サポートされなくなった機能

### Internet Explorer 11

Internet Explorer のサポートが廃止され、Workfront は Microsoft Edge を正式にサポートするようになりました。

サポートされているブラウザーについて詳しくは、[Adobe Workfront のブラウザー要件](../../../workfront-basics/workfront-browser-requirements.md)を参照してください。

 
