---
content-type: release-notes
keywords: メモ、四半期、更新
navigation-topic: product-releases
title: 21.1 リリースの概要
description: 21.1 リリースは、実稼動環境で利用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '3658'
ht-degree: 100%

---

# 21.1 リリースの概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

このページでは、Adobe Workfront Classic と、21.1 リリースに含まれる新しい Adobe Workfront エクスペリエンスの両方の機能について説明します。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

今回のリリースでは、適応可能な戦略、自動化された作業プロセス、および企業全体での成功を可能にする接続されたデジタルインフラストラクチャを活用して、2021年の復帰をリードするための新機能と機能強化をリリースします。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

これらの機能強化は現在利用可能で、

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

2021年2月15日（PT）にリリースされました。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfront の機能強化

* [管理者機能の強化](#administrator-enhancements)
* [リソース管理機能の強化](#resource-management-enhancements)
* [プロジェクト管理機能の強化](#project-management-enhancements)
* [拡張分析の強化](#enhanced-analytics-improvements)
* [統合の機能強化](#integration-enhancements)
* [モバイル機能の強化](#mobile-enhancements)
* [その他の機能強化](#other-enhancements)

### 管理者機能の強化 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日および環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">プロジェクトをコピーするための新しいアクセスレベル設定を導入</a> </p> <p>システム管理者は、プロジェクトでプランナーが実行できる操作をより詳細に制御できるように、新しい設定を導入して、プロジェクトのコピー機能を有効または無効にすることで、アクセスレベルのプロジェクトへの編集アクセスをより詳細にしました。この変更以前は、ユーザーのプロジェクト編集へのアクセスを有効にした場合、ユーザーは自動的にそれらのプロジェクトをコピーするためのアクセス権を付与されました。新しい機能を使用すると、新しいコピー設定を無効にして、プロジェクトをコピーするアクセス権なしで、他のユーザーに編集プロジェクトへのアクセス権を付与できるようになります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">オブジェクトのカスタムフォームで、複数選択ドロップダウンフィールドのすべての項目を選択</a> </p> <p>オブジェクトの詳細ページで、カスタムフォームの複数選択ドロップダウンフィールドに入力する際に、使用可能なすべてのオプションを選択する必要がある場合は、「すべてを選択」をクリックします。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース：21.1 リリースを使用<span style="color: #dc143c; font-weight: bold;">（新しいリクエストを送信する際は、現在利用できません。）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">オブジェクトのすべてのカスタムフォームフィールドを再計算</a> </p> <p>オブジェクトの計算カスタムフィールドのすべてのデータを最新の状態に保つのが容易になりました。新しい式を再計算メニューオプションを使用すると、これらのフィールド内のすべてのデータをすばやく再計算できます。</p> <p>これは、オブジェクト内の計算カスタムフィールドで参照される別のオブジェクト内のデータを編集した後に特に便利です。</p> <p>以前は、計算されたカスタムフィールド内のすべてのデータが最新であることを確認するために、回避策を使用する必要がありました。例えば、オブジェクトを他のオブジェクトと共に編集し、一括編集が可能な再計算オプションを使用しました。</p> </td> 
   <td><strong>公開日：</strong> <p>Beta プレビューリリース：2020年12月10日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">グループ管理者のタスクとイシューの環境設定のロックを解除</a> </p> <p>Workfront の管理者は、個々のタスクとイシューの環境設定をロック解除することで、グループ管理者にさらに自律性を与えることが可能になりました。グループ管理者は、環境設定のロックが解除されると、各グループの一意なニーズと内部プロセスに対応するように、グループ用に環境設定を構成できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月2日（PT）</p> <p>実稼動版リリース：21.1 リリース<span style="color: #dc143c; font-weight: bold;">（2021年6月24日（PT）までは、段階的なロールアウトの一環として、クラスター 4 および 6 のお客様と、その他一部のお客様のみが使用できました。現在は、すべてのお客様が実稼動環境で利用できます。）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">ポートフォリオとプログラムのアクセスレベルを個別に設定</a> </p> <p>ポートフォリオとプログラムのアクセスレベルを個別に設定できるので、ポートフォリオとプログラムへのユーザーアクセスを管理しやすくなりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月2日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">カスタムフォームで情報を編集する際に、一連のすべてのチェックボックスをオンにする</a> </p> <p>オブジェクトの詳細ページで、カスタムフォームの複数選択ドロップダウンフィールドに入力する際に、使用可能なすべてのオプションを選択する必要がある場合は、「すべてを選択」をクリックします。</p> <p>このオプションは、フィールドにチェックボックスが 3 つ以上含まれている場合にのみ表示されます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月2日（PT）</p> <p>実稼動版リリース：21.1 リリース<span style="color: #dc143c; font-weight: bold;">（リクエストの送信時は現在利用できません。）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Workfront メール許可リストの設定</a> </p> <p>データのセキュリティを強化するために、メールドメインの許可リストを使用して以下を実行できます。</p> 
    <ul> 
     <li> <p>Workfront に保存されたレポートやドキュメントが Workfront メールに含まれる場合、メールの送信先を制御する</p> </li> 
     <li> <p>メールアドレスに含めることができるメールドメインを制御する（ユーザープロファイルでユーザーが指定できます）</p> </li> 
    </ul> <p>例えば、メールの許可リストに社内のメールドメインのみを含めると、リスクのある顧客をリストアップしたレポートなどの機密データを保護することができます。この場合、ユーザーは、そのレポートを（その他の Workfront レポートも）外部のメールアドレスに送信できません。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年11月20日（PT）</p> <p>実稼動版リリース：21.1 リリース </p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">サブグループのグループ管理者を割り当て</a> </p> <p>組織の各レベルで独立して運用しやすくなるように、サブグループにグループ管理者を割り当てる機能を追加しました。これにより、サブグループの管理を適切な担当者に委任することができます。</p> <p>以前は、トップレベルのグループにのみグループ管理者を置くことができ、その管理者がトップレベルのグループの下にあるすべてのサブグループを管理していました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年11月20日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">グループエリアでのグループプロジェクトと承認プロセスの操作</a> </p> <p>グループのプロジェクトや承認プロセスがグループエリアに一覧表示されるようになり、グループ管理者はそれらの表示と操作を簡単に行うことができます。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年11月20日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">グループのイベント通知の設定</a>（<span style="color: #dc143c; font-weight: bold;">プレビュー環境での新機能</span>）</p> <p>Workfront 管理者は、トップレベルのグループに対するイベント通知を設定できるようになり、グループ管理者にさらに自律性を持たせることができるようになりました。サブグループは、トップレベルの親グループから通知設定を継承します。</p> <p>以前は、Workfront 管理者がシステムレベルでしかイベント通知を設定できず、すべてのグループが同じ一連のイベント通知を使用する必要がありました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021年1月22日（PT）</p> <p>実稼動リリース：21.1 リリースと同時<span style="color: #dc143c; font-weight: bold;">（段階的ロールアウトの一環として、最初はクラスター 4 のお客様のみが実稼動環境で利用できますが、他のクラスターでもその後すぐに利用可能になります）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">グループ内の使用済みおよび割り当て済みライセンス数の表示</a> </p> <p>ライセンスの配布状況を判断するために、あるグループとその下のサブグループで使用されているライセンスの数を表示できます。</p> <p>トップレベルのグループを管理している場合は、あるグループ（およびそのサブグループ）で使用されているライセンス数と、そのグループに割り当てられているライセンスの最大数の両方を表示できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年11月20日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">プロジェクトのワークロードバランサー</a> </p> <p>プロジェクト内でワークロードバランサーを使用できるようになりました。プロジェクトリソースを管理するのに、ワークロードバランサーを使用するかスケジュールツールを使用するかを選択できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月17日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">ワークロードバランサーがチームで利用可能</a> </p> <p>チーム内でワークロードバランサーを使用できるようになりました。チームリソースを管理するのに、ワークロードバランサーを使用するかスケジュールツールを使用するかを選択できるようになりました。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年11月20日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### プロジェクト管理の機能強化 {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">プロジェクトの「指標」セクションで書き出しが利用可能</a> </p> <p>プロジェクトのステータスと進行状況をより簡単に共有できるように、プロジェクトの「指標」セクションにあるダッシュボード全体を .png ファイルに書き出しできるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2021 年 1 月 15 日</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">イシューの更新からプロジェクトまたはタスクに変換された際にイシューの完了率を更新</a> </p> <p>プロジェクトまたはタスクに変換されたイシューにおけるイシューの完了率の仕組みをアップデートしました。新しい機能では、イシューがタスクまたはプロジェクトに変換されると、「解決オブジェクトの状態が変わると、解決可能問題の状態を自動的に更新します」が設定で有効になっている場合、イシューの完了率が解決タスクまたは解決プロジェクトの完了率と同期して更新されます。</p> </td> 
   <td><strong>次の日程で利用可能：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">新しいリクエストページから削除されたフィールド</a> </p> <p>新しいリクエストページの再設計の一環として、プロジェクトの「キューの設定」セクションで設定された新しいイシューフィールドを更新しました。</p> <p>様々な新しいイシューフィールドは、プロジェクトのイシューセクションからイシューを作成する場合にのみ表示されます。リクエスト領域のリクエストキューを使用してイシューを送信する際には表示されません。</p> </td> 
   <td><strong>次の日程で利用可能：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース：21.1 リリース<span style="color: #dc143c; font-weight: bold;">（リリースから削除）</span></p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">リクエスト領域でリクエストを送信する際の新しいエクスペリエンス</a> </p> <p>新しい Workfront エクスペリエンスとの一貫性を保ち、リクエストの送信時の効率を高めるために、リクエストエリアの「新規リクエスト」ボックスのデザインを変更しました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース： 21.1 リリース<span style="color: #dc143c; font-weight: bold;">（リリースから削除。プレビューに残り、21.2 実稼動環境にリリースされます）</span></p> <p><strong>次の環境で利用可能：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">リクエスト送信時のリクエストキューへのリンクを共有</a> </p> <p>リクエストの作成時に、リクエストキュー、トピックグループ、またはキューのトピックへのリンクを共有できるようになりました。</p> <p>新しいリクエストを送信する前に、リクエストのリクエストキュー、トピックグループ、またはキューのトピックへのリンクをコピーして、他のユーザーと共有したり、ダッシュボードに埋め込んだりできます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月13日</p> <p>実稼動版リリース： 21.1 リリース<span style="color: #dc143c; font-weight: bold;">（リリースから削除。プレビューに残り、21.2 実稼動環境にリリースされます）</span></p> <p><strong>次の環境で利用可能：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">新しく送信されたリクエストのリスト</a> </p> <p>より簡単で一貫性の高い方法で送信済みリクエストを管理できるように、リクエストエリアの「送信済みの要求」セクションと「すべての要求」セクションを削除し、新しく「送信済み」リストに置き換えました。リストは、システムの他のリストとマッチする使い慣れたルックアンドフィールになっており、送信済みリクエストの様々なカテゴリをフィルタリングし、見つけにくいリクエストを素早く検索できます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月2日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">プロジェクトに割り当てるグループを検索し、その詳細を表示する</a> </p> <p>プロジェクトにグループを割り当てる際に、適切なグループを識別しやすくなりました。「グループ」ボックスに表示されるグループ名の上にポインタを合わせて、名前の横に表示される情報アイコンをクリックして、グループの詳細のツールチップを表示します。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月17日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">新規ユーザーのデリゲーションレポート</a> </p> <p>以前は、タスク、イシュー、プロジェクトの承認のデリゲーションに関する情報は、デリゲートのホームエリアにのみ表示されていました。他のユーザーにこの情報の表示を許可するために、プランユーザーはユーザーのデリゲーションレポートを作成できます。このレポートは、次の内容を示します。</p> 
    <ul> 
     <li> <p>他のユーザーにこれらの承認をデリゲートしたユーザー</p> </li> 
     <li> <p>これらの承認がデリゲートされたユーザー</p> </li> 
     <li> <p>これらのデリゲーションの開始日と終了日</p> </li> 
    </ul> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月17日（PT）</p> <p>実稼動版リリース：2021年1月21日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 拡張分析の強化 {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>機能</strong> </p> </td> 
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">すべてのクラスターでユーザーページを利用できるようになりました</a> </p> <p>クラスター 4 のWorkfront Classic で、ユーザーページが使用できるようになりました。このページには、チーム別のアクティビティ、リソースのキャパシティ、チームのキャパシティのグラフが含まれます。</p> <p>このページは、以前、Workfront Classic の 20.3 リリースと、その他すべてのクラスター向けの新しい Workfront エクスペリエンスで使用できました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2021年1月28日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス（以前利用可能）</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">拡張された分析がデフォルトで表示されるようになりました</a> </p> <p>メモ：この変更は、レイアウトテンプレートに新しく追加されたユーザーにのみ適用されます。カスタムレイアウトテンプレートに割り当てられたユーザーも、この変更による影響を受けません。</p> <p>デフォルトのレイアウトテンプレートでは、分析エリアがデフォルトで有効になりました。つまり、このレイアウトテンプレートに割り当てられたユーザーは、Workfront Classic のグローバルナビゲーションバーに分析エリア、新しい Workfront エクスペリエンスのメインメニューに表示されます。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータプレビューリリース：2020年11月6日（PT）</p> <p>実稼動版リリース：2020年12月3日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">すべてのクラスターで利用可能な拡張分析</a> </p> <p>クラスターのお客様を含む、すべての Workfront クラスターで拡張分析を利用できます。</p> <p>以前は、Google Cloud Platform で拡張分析が使用できず、クラスター 6 のお客様が Analytics エリアにアクセスできなくなっていました。クラスター 6 の Business および Enterprise のお客様が分析エリアにアクセスできるようになりました。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：2020年11月20日（PT）</p> <p>実稼動版リリース：2020年12月3日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Microsoft Teams での Adobe Workfront 通知の機能強化</a> </p> <p>Microsoft Teams を通じて Workfront を簡単に使用できるように、Workfront から送信される Microsoft Teams 通知に様々な機能強化が追加されました。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：なし</p> <p>実稼動版リリース：2021年1月13日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Adobe Workfront アプリの新しいナビゲーションパンくずリスト</a> </p> <p>Workfront モバイルアプリにパンくずリストナビゲーションが追加されました。この機能を使用して、プロジェクト内の親作業アイテムに移動できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：なし</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Workfront アプリ上のカスタムフォームでサポートされるリッチテキスト</a> </p> <p>Workfront モバイルアプリのカスタムフォームテキストフィールドでリッチテキスト書式を使用できるようになりました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：なし</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO ユーザーは、顔認識 ID またはフィンガープリントテクノロジーを使用して、Workfront アプリに再ログインできるようになりました</a> </p> <p>組織が SSO を使用している場合、セッションがタイムアウトになった後、顔認証またはフィンガープリントを使用して Workfront モバイルアプリにログインできるようになりました。ただし、最初は SSO 資格情報を使用してログインする必要があります。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：なし</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
--&gt;

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
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">イベントサブスクリプションエラーの要件の更新</a> </p> <p>イベントサブスクリプションエラーのソフトな無効化要件を更新しています。既存の要件に加え、2000 試行以内に正常な配信に失敗した場合、イベントサブスクリプションはソフトに無効化されます。これは、条件によっては過剰な失敗を引き起こす可能性のある、既存の 70％失敗ルールを強化するためです。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：なし</p> <p>実稼動版リリース：2021年1月11日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">日次ダイジェストで使用できる新しいチームフィールド</a> </p> <p>チームの承認フィールドと割り当てフィールドを、「必要なアクションの日刊ダイジェスト」メールに追加しました。</p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月17日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">リクエストキューの POP メールオプションを置き換え</a> </p> <p>リクエストキューの POP メールオプションを、Workfront 管理が管理する新しいシステムに置き換えます。引き続きメールでリクエストを送信できますが、Workfront が管理する新しいメールアドレスをリクエストキューのエリアで設定する必要があります。 </p> </td> 
   <td><strong>公開日：</strong> <p>ベータ版プレビューリリース：2020年12月17日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">タイムシートの時間編集を制限</a> </p> <p>タイムシートと時間の編集をより詳細に制御するために、タイムシートの所有者やシステム管理者が時間を編集することを制限できる設定を追加しました。</p> <p>以前は、アクセスレベルで「タイムシートと時間」オプションが有効になっているユーザーは、タイムシートの時間を編集できました。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：2021年1月21日（PT）</p> <p>実稼動版リリース：21.1 リリース</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">タイムシートエリアのフィルターとビューを改善</a> </p> <p>プロジェクトとイシューのフィルターを追加し、検索ページに表示オプションとグループ化オプションを追加しました。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：2020年12月2日（PT）</p> <p>実稼動版リリース：2021年1月21日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">タイムシートの超過時間ボックスを非表示にする</a> </p> <p>Workfront で残業時間を追跡しない場合、超過時間ボックスを非表示にして、ユーザーの混乱を和らげることができるようになりました。単一使用のタイムシートまたはタイムシートプロファイルで、超過時間ボックスを非表示にすることができます。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：2020年12月2日（PT）</p> <p>実稼動版リリース：2020年12月16日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">パンくずナビゲーションで項目を展開または折りたたむ</a> </p> <p>パンくず全体のパスを容易に表示できるように、展開と折りたたみの機能を追加しました。</p> <p>省略された項目は、プロジェクトの前に「その他」というテキストでグループ化されます。例えば、「その他 3 つ」は、表示されていない 3 つのオブジェクトがあることを示します。</p> <p>これまでは、切り詰められたオブジェクトをドロップダウンメニューで表示するには、省略記号アイコンをクリックする必要がありました。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>ベータ版プレビューリリース：2020年1月7日（PT）</p> <p>実稼動版リリース：2021年1月21日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">パンくずナビゲーションの新しいルックアンドフィール</a> </p> <p>ユーザーが Workfront の場所をより正確に識別し、オブジェクト間をより簡単に移動できるように、パンくずリストのナビゲーションにいくつかの改善を加えました。</p> </td> 
   <td><strong>利用可能になる日時：</strong> <p>Beta プレビューリリース：2020年12月10日（PT）</p> <p>実稼動版リリース：2021年1月21日（PT）</p> <p><strong>利用可能な環境：</strong> </p> <p>新しい Adobe Workfront エクスペリエンス </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Goals の強化

21.1 リリースでの Workfront Goals リリースに向けての最新機能。プレビュー環境で利用できる新機能について詳しくは、[Adobe Workfront Goals 21.1 リリース](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md)を参照してください。

## Workfront シナリオプランナーの機能強化

21.1 リリースで Workfront Scenario Planner リリースに加わる新機能です。プレビュー環境で利用できる新機能について詳しくは、[Adobe Workfront Scenario Planner 21.1 リリース](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md)を参照してください。

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境の 21.1 リリーススケジュール以外のサイクルで使用できます。最新の機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

## API の機能強化

API バージョン 12 が 20.4 リリースで利用できるようになりました。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

新機能と更新点について詳しくは、[API バージョン 12 の新機能](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm)を参照してください。

API のバージョンについて詳しくは、[API のバージョン管理とサポートのスケジュール](../../../wf-api/api/api-version-support-schedule.md)を参照してください。

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Workfront のメンテナンスアップデート

21.1 リリースで行われたメンテナンスアップデートについて詳しくは、[Workfront メンテナンスの更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350)を参照してください。

## お知らせ

* [21.1 リリースでの Workfront メールの新しい IP アドレス](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [イベントサブスクリプションの追加 IP アドレスの許可リスト](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Workfront へのアクセスに必要な追加ドメインの許可リスト](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Flash の廃止](#flash-deprecation)
* [21.1 リリースウェビナー](#21-1-release-webinar)
* [プレビューのリリース頻度を変更](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### 21.1 リリースでの Workfront メールの新しい IP アドレス {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

メールの配信を成功に導くために、21.1 実稼動版リリースでクラスター 1、2、3、4、5 に新しい IP アドレスを追加します。

クラスターに追加する必要がある IP アドレスについて詳しくは、[21.1 リリースでの Adobe Workfront メールの新しい IP アドレス](../../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)を参照してください。

インスタンスが存在するクラスターを確認するには、設定／システム／顧客情報の順に移動します。

### イベントサブスクリプションの追加 IP アドレスの許可リスト {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

イベントサブスクリプションの配信を成功に導くために、2021年第 1 四半期の 21.1 実稼動版リリースで 4 つの新しい IP アドレスを追加します。ユーザーが引き続きイベントサブスクリプションを受信できるようにするには、2021年2月（PT）までにこれらの IP アドレスを許可リストに追加する必要があります。

[イベントサブスクリプション API](../../../wf-api/general/event-subs-api.md)の記事にある新しい IP の追加についてサポートが必要な場合は、社内の IT 部門やセキュリティ部門にお問い合わせください。

### Workfront へのアクセスに必要なドメインを許可リストに追加 {#allowlist-of-additional-domains-required-for-accessing-workfront}

組織でファイアウォールを使用している場合、Workfront へのアクセスが遮断されないように、次のドメインを許可リストに追加してください。

* event.split.io
* sdk.split.io

詳しくは、[ファイアウォールの許可リストを設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

### Flash の廃止 {#flash-deprecation}

すべての Flash ベースのツールは、2020年11月19日（PT）にすべての製品から削除されました。

特定の Flash ベースの各ツールの代替ソリューションについて詳しくは、[Adobe Workfront における Flash ベースのツールの代替](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md)の記事を参照してください。

### 21.1 リリースウェビナー {#21-1-release-webinar}

Workfront 21.1 リリースウェビナーは、2月3日午前 11 時（EDT）／4 時（BST）に発表されます。ウェビナーへは[ここから](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register)登録してください。

### プレビューのリリース頻度の変更 {#change-in-preview-release-cadence}

2020年5月20日（PT）より、Workfront は、毎週プレビュー環境で機能を利用できるようになりました。この変更を行う前は、通常、2 週間ごとにプレビュー環境で機能をリリースしていました。

詳しくは、[Workfront プレビューリリース頻度の変更に関する FAQ](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence) を参照してください。

### Workfront One {#workfront-one}

Workfront One を使用すると、Workfront の重要なコンテンツ、リソース、ニュースをすべて 1 か所で、1 回のログインで見つけることができます。エクスペリエンス、コミュニティ、トレーニングの各サイトを統合し、探しているものを見つけやすくしました。

[Workfront One の詳細](https://www.workfront.com/campaigns/workfront-one)
