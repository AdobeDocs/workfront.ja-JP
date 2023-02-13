---
content-type: release-notes
keywords: メモ，四半期，更新
navigation-topic: product-releases
title: 21.1 リリースの概要
description: 21.1 リリースは、の週に実稼動環境で利用できるようになりました。
author: Luke
feature: Product Announcements
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '3635'
ht-degree: 0%

---

# 21.1 リリースの概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

このページでは、Adobe Workfront Classic と、21.1 リリースに含まれる新しいAdobe Workfrontエクスペリエンスの両方の機能について説明します。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

今回のリリースでは、適応可能な戦略、自動化された作業プロセス、企業全体での成功を可能にする接続されたデジタルインフラストラクチャを活用して、2021 年に復帰を支援する新機能と機能強化をリリースします。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

これらの機能強化は現在利用可能です

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

実稼動環境で使用できます。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

2021 年 2 月 15 日にリリースされました。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfrontの機能強化

* [管理者の機能強化](#administrator-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [プロジェクト管理の強化](#project-management-enhancements)
* [分析の強化](#enhanced-analytics-improvements)
* [統合の強化](#integration-enhancements)
* [モバイル機能の強化](#mobile-enhancements)
* [その他の機能強化](#other-enhancements)

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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">プロジェクトをコピーするための新しいアクセスレベル設定を導入しました</a> </p> <p>システム管理者は、プロジェクトでプランナが実行できる操作をより詳細に制御できるように、新しい設定を導入して、プロジェクトのコピー機能を有効または無効にすることで、アクセスレベルでプロジェクトの編集アクセスをより詳細にしました。 この変更がおこなわれる前は、ユーザーのプロジェクト編集へのアクセスを有効にした場合、ユーザーは自動的にそれらのプロジェクトをコピーするためのアクセス権を持っていました。 新しい機能を使用すると、新しい [ コピー ] 設定を無効にして、必ずしもプロジェクトをコピーするアクセス権を持たずに、他のユーザーに編集プロジェクトへのアクセス権を付与できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">オブジェクトのカスタムフォームで、複数選択ドロップダウンフィールドのすべての項目を選択します</a> </p> <p>オブジェクトの詳細ページで、カスタムフォームの複数選択ドロップダウンフィールドに入力する際に、使用可能なすべてのオプションを選択する必要がある場合は、「すべて選択」をクリックします。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">（新しいリクエストを送信する際は、現在利用できません）。</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">オブジェクトのすべてのカスタムフォームフィールドを再計算する</a> </p> <p>オブジェクトの計算カスタムフィールドのすべてのデータを最新の状態に保つのが簡単になりました。 新しい [ 式を再計算 ] メニューオプションを使用すると、これらのフィールド内のすべてのデータをすばやく再計算できます。</p> <p>これは、オブジェクト内の計算カスタムフィールドで参照される別のオブジェクト内のデータを編集した後に特に便利です。</p> <p>以前は、計算されたカスタムフィールド内のすべてのデータが最新であることを確認するために、回避策を使用する必要がありました。 例えば、オブジェクトを他のオブジェクトと共に編集し、一括編集が可能な再計算オプションを使用しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 10 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">グループ管理者のタスクと問題の環境設定をロック解除</a> </p> <p>Workfrontの管理者は、個々のタスクと問題の環境設定をロック解除することで、グループ管理者にさらに自律性を与えることができるようになりました。 グループ管理者は、環境設定のロックが解除されると、各グループの固有のニーズと内部プロセスに対応するように、グループ用に環境設定を構成できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 3 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">(2021 年 6 月 24 日以前は、クラスター 4 および 6 のお客様およびその他のお客様に対してのみ、段階的なロールアウトの一環として使用できました。 現在は、すべてのお客様が実稼動環境で利用できます。)</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">ポートフォリオとプログラムのアクセスレベルを個別に設定する</a> </p> <p>ポートフォリオとプログラムへのユーザーアクセスを管理しやすくなりました。ポートフォリオとプログラムのアクセスレベルを個別に設定できるからです。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 3 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">カスタムフォームで情報を編集する際に、一連のすべてのチェックボックスをオンにする</a> </p> <p>オブジェクトの詳細ページで、チェックボックスを含むカスタムフォームフィールドに入力する際に、使用可能なすべてのチェックボックスをオンにする必要がある場合は、「すべて選択」をクリックします。</p> <p>このオプションは、フィールドに 2 つ以上のチェックボックスが含まれている場合にのみ表示されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 3 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">（リクエストの送信時は現在利用できません）。</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Workfront E メールの設定を許可リスト行う</a> </p> <p>データのセキュリティを強化するために、電子メールドメインドメインを使用して次のこ許可リストとをおこなうことができます。</p> 
    <ul> 
     <li> <p>Workfrontに保存されたレポートやドキュメントがWorkfront電子メールに含まれる場合の移動先を制御</p> </li> 
     <li> <p>ユーザープロファイルでユーザーが指定できる電子メールアドレスに、制御電子メールドメインを含めることができます</p> </li> 
    </ul> <p>例えば、アットリスクを伴う顧客を一覧表示するレポートなど、機密データを保護する場合は、E メールドメインに社内 E メールドメインまたはドメインのみを含めることができ許可リストます。 この方法では、ユーザーは、そのレポート ( またはその他のWorkfrontレポート ) を外部の電子メールアドレスに送信できません。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 21 日</p> <p>実稼動版リリース： 21.1 リリースを使用 </p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">サブグループのグループ管理者を割り当てる</a> </p> <p>組織のレベルが個別に操作しやすくなるように、グループ管理者をサブグループに割り当てる機能を追加しました。 これで、適切な担当者にサブグループ管理を委任していることを確認できます。</p> <p>以前は、最上位グループのみがグループ管理者を持つことができ、その管理者は最上位グループの下にあるすべてのサブグループを管理していました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 21 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">「グループ」領域でのグループプロジェクトと承認プロセスの操作</a> </p> <p>グループ管理者は、グループのプロジェクトや承認プロセスが「グループ」領域に一覧表示されるので、簡単にグループのプロジェクトや承認プロセスを表示および操作できます。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 21 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">グループのイベント通知の設定</a> <span style="color: #dc143c; font-weight: bold;">プレビューの新機能</span></p> <p>Workfrontの管理者は、最上位のグループに対するイベント通知を設定できるようになり、グループ管理者にさらに自律性を与えることができるようになりました。 サブグループは、最上位の親グループからイベント通知設定を継承します。</p> <p>以前は、Workfrontの管理者がシステムレベルでのみイベント通知を設定できていました。つまり、すべてのグループが同じイベント通知のセットを使用する必要がありました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 23 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">( 最初は実稼動環境で使用できるのは、段階的なロールアウトの一環として、クラスター 4 のお客様のみです。その後すぐに他のクラスターで使用可能</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">グループ内で使用および割り当てられたライセンス数の表示</a> </p> <p>ライセンスの配布状況を判断するために、1 つのグループとその下のサブグループで使用されているライセンスの数を表示できます。</p> <p>最上位グループを管理する場合は、グループで使用されるライセンスの数（およびそのサブグループ）と、グループに割り当てられるライセンスの最大数の両方を表示できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 21 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">プロジェクト用ワークロードバランサー</a> </p> <p>これで、ワークロードバランサーがプロジェクト内で使用できるようになりました。 これで、ワークロードバランサーまたはスケジューリングツールを使用してプロジェクトリソースを管理するかを選択できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 18 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">チームで利用可能なWorkfrontバランサー</a> </p> <p>ワークロードバランサーをチーム内で使用できるようになりました。 これで、ワークロードバランサーを使用するか、スケジューリングツールを使用してチームリソースを管理するかを選択できます。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 21 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### プロジェクト管理の強化 {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">プロジェクトの指標セクションでエクスポートが利用できるようになりました</a> </p> <p>プロジェクトのステータスと進行状況をより簡単に共有できるように、プロジェクトの「指標」セクションにあるダッシュボード全体を.png ファイルにエクスポートできるようになりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 16 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">問題の更新から変換されたプロジェクトまたはタスクで、問題の完了率を更新します</a> </p> <p>プロジェクトまたはタスクに変換された問題に対する、問題の完了率の仕組みを更新しました。 新機能では、問題がタスクまたはプロジェクトに変換されると、[ 解決可能な問題の状態が変更された場合に自動的に解決可能な問題の状態を更新する ] 設定が設定から有効になると、問題の完了率が解決タスクまたはプロジェクトの完了率と同期して更新されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">新しいリクエストページから削除されたフィールド</a> </p> <p>新しいリクエストページの再設計の一環として、プロジェクトのキュー設定セクションで設定された新しい問題フィールドを更新しました。</p> <p>様々な「新しい問題」フィールドは、プロジェクトの「問題」セクションからイシューを作成する場合にのみ表示されます。 「リクエスト」領域のリクエストキューを使用して問題を送信する際に、これらは表示されません。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">（リリースから削除）</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">リクエスト領域でリクエストを送信する際の新しいエクスペリエンス</a> </p> <p>新しいWorkfrontエクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエスト領域の新しいリクエストボックスのデザインを変更しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">( リリースから削除済み、はプレビューのままとなり、21.2 で実稼動環境にリリースされます )</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">リクエスト送信時のリクエストキューへのリンクの共有</a> </p> <p>リクエストの作成時に、リクエストキュー、トピックグループ、またはキュートピックへのリンクを共有できるようになりました。</p> <p>新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループまたはキュートピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 14 日</p> <p>実稼動版リリース： 21.1 リリースを使用 <span style="color: #dc143c; font-weight: bold;">( リリースから削除済み、はプレビューのままとなり、21.2 で実稼動環境にリリースされます )</span></p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">新しく送信されたリクエストリスト</a> </p> <p>より一貫性の高い簡単な方法で送信済みリクエストを管理できるように、「リクエスト」領域の「送信済みリクエスト」と「すべてのリクエスト」セクションを削除し、新しい送信済みリストに置き換えました。 リストは、システム内の他のすべてのリストと一致する使い慣れたルックアンドフィールを持ち、送信されたリクエストの様々なカテゴリをフィルタリングし、見つけにくいリクエストをすばやく検索できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 3 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">プロジェクトに割り当てるグループを検索し、その詳細を表示します</a> </p> <p>プロジェクトにグループを割り当てる際に、適切なグループを識別しやすくなりました。 「グループ」ボックスに表示されるグループ名の上にマウスポインターを置き、名前の横に表示される情報アイコンをクリックして、グループの詳細のツールチップを表示します。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 18 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">新しいユーザーの委任レポート</a> </p> <p>以前は、タスク、問題、プロジェクトの承認の委任に関する情報は、委任者のホーム領域にのみ表示されていました。 他のユーザーにこの情報の表示を許可するために、プランユーザーはユーザー委任レポートを作成できます。このレポートは次の内容を示します。</p> 
    <ul> 
     <li> <p>他のユーザーにこれらの承認を委任したユーザー</p> </li> 
     <li> <p>これらの承認が委任されたユーザー</p> </li> 
     <li> <p>これらの委任の開始日と終了日</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 18 日</p> <p>実稼動リリース： 2021 年 1 月 22 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 分析の強化 {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">すべてのクラスターでユーザーページを利用できるようになりました</a> </p> <p>Cluster 4 のWorkfront Classic で、People ページが使用できるようになりました。 このページには、チーム別のアクティビティ、リソース容量、チーム容量のグラフが含まれます。</p> <p>このページは、以前、Workfront Classic の 20.3 リリースと、その他すべてのクラスター向けの新しいWorkfrontエクスペリエンスで使用できました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 29 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス（以前利用可能）</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">拡張された分析がデフォルトで表示されるようになりました</a> </p> <p>注意：この変更は、レイアウトテンプレートに新しく追加されたユーザーにのみ適用されます。 カスタムレイアウトテンプレートに割り当てられたユーザーも、この変更による影響を受けません。</p> <p>デフォルトのレイアウトテンプレートでは、分析領域がデフォルトで有効になりました。つまり、このレイアウトテンプレートに割り当てられたユーザーは、Workfront Classic のグローバルナビゲーションバーに分析領域、新しいWorkfrontエクスペリエンスのメインメニューに表示されます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 7 日</p> <p>実稼動リリース： 2020 年 12 月 4 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">すべてのクラスターで利用可能な拡張分析</a> </p> <p>Cluster 6 のお客様を含む、すべてのWorkfrontクラスターで拡張分析を利用できます。</p> <p>以前は、Google Cloud Platform で拡張分析が使用できず、クラスター 6 のお客様が Analytics 領域にアクセスできなくなっていました。 現在は、Cluster 6 の Business および Enterprise のお客様は、Analytics 領域にアクセスできます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 11 月 21 日</p> <p>実稼動リリース： 2020 年 12 月 4 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Adobe Workfront通知のMicrosoft Teamsの強化</a> </p> <p>Microsoft Teamsを通じてWorkfrontを簡単に使用できるように、Workfrontから送信されるMicrosoft Teams通知に様々な機能強化が加えられました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：なし</p> <p>実稼動リリース： 2021 年 1 月 13 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Adobe Workfrontアプリの新しいナビゲーションパンくずリスト</a> </p> <p>Workfrontモバイルアプリにパンくずリストナビゲーションを追加しました。 これで、この機能を使用して、プロジェクト内の親作業項目に移動できます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：なし</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Workfrontアプリ上のカスタムフォームでサポートされるリッチテキスト</a> </p> <p>Workfrontモバイルアプリのカスタムフォームテキストフィールドでリッチテキストの書式設定を使用できるようになりました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：なし</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO ユーザーは、 Face ID またはフィンガープリントテクノロジーを使用して、Workfrontアプリに再ログインできるようになりました</a> </p> <p>組織が SSO を使用している場合、 Face ID またはフィンガープリントを使用して、セッションの後、タイムアウトしたときにWorkfrontモバイルアプリにログインできるようになりました。 最初に SSO 資格情報を使用してログインする必要があります。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：なし</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
—&gt;

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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">イベント購読失敗の要件の更新</a> </p> <p>イベント購読エラーのソフトディセーブル要件を更新しています。 既存の要件に加え、2000 回以内に正常な配信に失敗した場合、イベント購読はソフトディセーブルになります。 これは、ある条件下で過剰な失敗を引き起こす可能性のある、既存の 70%失敗ルールを強化するためです。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：なし</p> <p>実稼動リリース： 2021 年 1 月 12 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Daily Digest で使用できる新しいチームフィールド</a> </p> <p>チームの承認フィールドと割り当てフィールドを、「日々のダイジェストで必要なアクション」電子メールに追加しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 18 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">リクエストキューの POP 電子メールオプションの置き換え</a> </p> <p>リクエストキューの POP 電子メールオプションを、新しいWorkfront管理システムに置き換えます。 引き続き電子メールでリクエストを送信できますが、代わりに、リクエストキュー領域でWorkfrontが管理する新しい電子メールアドレスを設定する必要があります。 </p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 18 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">タイムシートの時間編集を制限する</a> </p> <p>タイムシートと時間の編集をより詳細に制御するために、時間の編集をタイムシートの所有者とシステム管理者に制限する設定を追加しました。</p> <p>以前は、アクセスレベルで [ タイムシートと時間 ] オプションが有効になっているユーザーは、任意のタイムシートの時間を編集できました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2021 年 1 月 22 日</p> <p>実稼動版リリース： 21.1 リリースを使用</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">[ タイムシート ] 領域のフィルタとビューを改善しました</a> </p> <p>プロジェクトとイシューのフィルターを追加し、検索ページに表示およびグループ化オプションを追加しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 3 日</p> <p>実稼動リリース： 2021 年 1 月 22 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">タイムシートの時間枠を非表示にする</a> </p> <p>Workfrontで時間外を追跡しない場合に、時間外ボックスを非表示にして、ユーザーの混乱を和らげることができるようになりました。 単一使用のタイムシートまたはタイムシートプロファイルで、超過作業時間ボックスを非表示にすることができます。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 3 日</p> <p>実稼動リリース： 2020 年 12 月 16 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">パンくずナビゲーションで項目を展開または折りたたむ</a> </p> <p>パンくずパス全体を容易に表示できるように、展開および折りたたみ機能が追加されました。</p> <p>現在は、切り捨てられた項目は、プロジェクトの前に「その他」というテキストでグループ化されます。 例えば、「さらに 3 つ」は、表示されていない 3 つのオブジェクトがあることを示します。</p> <p>以前は、省略記号をクリックして、切り捨てられたオブジェクトをドロップダウンメニューに表示する必要がありました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 1 月 8 日</p> <p>実稼動リリース： 2021 年 1 月 22 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">パンくずナビゲーションの新しいルックアンドフィール</a> </p> <p>ユーザーがWorkfront内の場所をより正確に識別し、オブジェクト間をより簡単に移動できるように、パンくずリストのナビゲーションをいくつか改善しました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> <p>ベータプレビューリリース：2020 年 12 月 10 日</p> <p>実稼動リリース： 2021 年 1 月 22 日</p> <p><strong>次の環境で使用できます。</strong> </p> <p>新しいAdobe Workfrontエクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront目標の強化

21.1 リリースでのWorkfront Goals リリースに向けての最新機能。 プレビューで利用できる新機能について詳しくは、 [Adobe Workfront 21.1 リリースでの目標](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Workfront Scenario Planner の機能強化

21.1 リリースでのWorkfront Scenario Planner リリースに加わる新機能です。 プレビューで利用できる新機能について詳しくは、 [21.1 リリースのAdobe Workfrontシナリオプランナー](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境では 21.1 リリーススケジュール以外のサイクルで使用できます。 最新の機能について詳しくは、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API の機能強化

API バージョン 12 が 20.4 リリースで利用できるようになりました。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

の新機能と更新点について詳しくは、 [API バージョン 12 の新機能](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

API バージョンについて詳しくは、 [API のバージョン管理とサポートのスケジュール](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

。

## Workfront のメンテナンス更新

21.1 リリースでおこなわれたメンテナンスアップデートについて詳しくは、 [Workfrontメンテナンスの更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## お知らせ

* [21.1 リリースでのWorkfront E メールの新しい IP アドレス](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [イベ許可リストント購読用の追加の IP アドレスの](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Workfrontにア許可リストクセスするために必要な追加ドメインの](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Flashの廃止](#flash-deprecation)
* [21.1 リリースウェビナー](#21-1-release-webinar)
* [プレビューのリリースケイデンスの変更](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### 21.1 リリースでのWorkfront E メールの新しい IP アドレス {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

E メールの配信を成功に導くために、クラスター 1、2、3、4、5 の 21.1 実稼動リリースで新しい IP アドレスを追加しています。

クラスターに追加する必要がある IP アドレスの詳細については、 [21.1 リリースでのAdobe Workfront E メールの新しい IP アドレス](../../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md).

インスタンスが存在するクラスタを確認するには、 Setup / System / Customer Info に移動します。

### イベ許可リストント購読用の追加の IP アドレスの {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

イベント購読の配信を成功に導くために、2021 年第 1 四半期に 21.1 実稼動版リリースを含む 4 つの新しい IP アドレスを追加します。 ユーザーが引き続きイベント購読を受け取るようにするに許可リストは、2021 年 2 月より前に、これらの IP アドレスをお客様のに追加する必要があります。

記事にある新しい IP の追加に関してサポートが必要な場合は、社内の IT 部門やセキュリティ部門に問い合わせてください。 [イベント購読 API](../../../wf-api/general/event-subs-api.md).

### Workfrontにア許可リストクセスするために必要な追加ドメインの {#allowlist-of-additional-domains-required-for-accessing-workfront}

組織でファイアウォールを使用している場合、Workfrontへの妨げられることのないアクセスを確保するため許可リストに、次のドメインを追加する必要があります。

* event.split.io
* sdk.split.io

詳しくは、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Flashの廃止 {#flash-deprecation}

2020 年 11 月 19 日に、すべてのFlashベースのツールがすべての製品から削除されました。

特定のFlash・ベースの各ツールの代替ソリューションの詳細については、次の記事を参照してください。 [Adobe WorkfrontのFlashベースのツールの代わり](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### 21.1 リリースウェビナー {#21-1-release-webinar}

Workfront 21.1 リリースウェビナーは、2 月 3 日 (PT) 午前 11 時/午後 4 時 (BST) に発表されます。 ウェビナーに登録 [ここ](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### プレビューのリリースケイデンスの変更 {#change-in-preview-release-cadence}

2020 年 5 月 20 日より、Workfrontは、プレビュー環境で毎週の機能の使用を開始しました。 この変更がおこなわれる前は、通常、機能は 2 週間ごとにプレビュー環境にリリースされていました。

詳しくは、 [Workfrontプレビューリリースケイデンスの変更に関する FAQ](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

Workfront One を使用すれば、Workfrontの最も重要なコンテンツ、リソースおよびニュースを 1 か所で 1 回のログインで確認できます。 エクスペリエンス、コミュニティ、トレーニングの各サイトを統合し、探しているものを見つけやすくしました。

[Workfront One の詳細](https://www.workfront.com/campaigns/workfront-one).
