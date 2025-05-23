---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 リソース管理の機能強化：ワークロードバランサー
description: このページでは、実稼動環境に対する 2020.2 リリースで行われた、リソース管理のすべての機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 99%

---

# 2020.2 リソース管理の機能強化：ワークロードバランサー

このページでは、実稼動環境に対する 2020.2 リリースで行われた、リソース管理のすべての機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。

2020.2 リリースで利用可能なすべての変更点の一覧については、[2020.2 リリースの概要](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)を参照してください。

担当者は第 1 階層のアセットです。ワークロードバランサーを使用すると、担当者を極度の疲労から守り、主要な企業戦略に沿って最高の成果を生み出せるように支援することができます。同じビューで担当者のワークロードと要求レベルを視覚化し管理できる、新しいスケジュールエクスペリエンスを導入します。ユーザーインターフェイスは、過稼動および低稼働状況の明確なビジュアルマッピングを提供し、すべての関係者に対して透明性が高くなっています。管理職は、その情報を入力として使用し、同じ画面からタイムライン全体で労力のバランスを取り直すことができます。これがその後、Workfront プラットフォームの残りの部分に反映されます。

>[!NOTE]
>
>ワークロードバランサーは、2019.4 リリースでベータ版としてリリースされ始めました。2020.2 リリースでは、ワークロードバランサーのすべての機能強化が一般に提供されます。このページで説明している機能強化は、2020.2 リリースで追加されました。ワークロードバランサーの概要については、[ワークロードバランサーの概要](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

## ワークロードバランサーでの日次および週次の配分の調整

リソースのバーンアウトを避けるために、ワークロードバランサーを使用して、ユーザーの日次および週次の作業の配分が調整できるようになりました。

この機能強化以前は、この調整はリソーススケジュールツールを使用した場合にのみ可能でした。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## ワークロードバランサーフィルター

ワークロードバランサーの情報を自分にとって関連性の高いものにするために、ワークロードバランサーの未割り当て作業エリアと割り当てられた作業エリアの両方に対するフィルターを作成して、今後の使用のために保存できるようになりました。その場合、新しいフィルターを使用してゼロから始めるのではなく、保存したバージョンを編集して、小さな変更を加えることができます。

ワークロードバランサーでのフィルタリングについては、[ワークロードバランサーでのフィルターの管理](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## ワークロードバランサーでの残存時間数の表示

正しい割り当てを決定できるように、新しい設定では、ユーザーが自分のスケジュールに従って稼動できる時間数と既に作業に割り当てられている時間数の差（残存時間数）を表示できるようになりました。新しい設定がワークロードバランサーで使用できるようになりました。

ワークロードバランサーでの情報の表示については、[ワークロードバランサーの操作](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)（Adobe Workfront Classic を使用している場合は[ワークロードバランサーの操作](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

**利用可能な環境：**

* 新しい Adobe Workfront エクスペリエンス

## ワークロードバランサーの未割り当て作業エリアでのタスクとプロジェクトの日次予定時間数の表示

割り当てをする前にタスクがユーザーのワークロードに与える影響を理解するうえで役に立つように、「割り当てを表示する」設定で、ワークロードバランサーの未割り当て作業エリアに表示される情報を管理するようになりました。この設定を有効にすると、タスクとプロジェクトの両方の予定時間数がワークロードバランサーの未割り当て作業エリアに表示されます。

この変更以前は、バランサーの割り当てられた作業エリアの情報のみがこの設定で更新されていました。

ワークロードバランサーの操作について詳しくは、[ワークロードバランサーの操作](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)（Adobe Workfront Classic を使用している場合は[ワークロードバランサーの操作](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新バージョンの Adobe Workfront（以前はタスクでのみ使用可能）

## ワークロードバランサーに対する新しい「設定」ボックス

エクスペリエンスを合理化するために、ワークロードバランサーでビューを更新するための追加のツールが表示される「設定」ボックスが使用可能になりました。このボックスには、次の設定が含まれます。

* プロジェクトでグループ化
* タスクおよびプロジェクトの割り当て済み時間または残り時間を表示

ワークロードバランサーでの情報の表示について詳しくは、[ワークロードバランサーの操作](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)（Adobe Workfront Classic を使用している場合は[ワークロードバランサーの操作](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## リンクによるワークロードバランサーの共有

従業員のワークロードを幹部と共有して、スタッフ配置のニーズに関するコンテキストを把握できるようになります。そのためには、ワークロードバランサーに対して一意の URL を他のユーザーと共有することで、ワークロードバランサーを共有することができます。

ワークロードバランサーの操作について詳しくは、[ワークロードバランサーの操作](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)（Adobe Workfront Classic を使用している場合は[ワークロードバランサーの操作](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## ワークロードバランサーでの日付範囲を変更

ワークロードバランサーのタイムライン期間をカスタマイズしてニーズに合わせられるように、一度に 2 週間、4 週間、6 週間のカスタム期間を選択して表示できるようになりました。

この機能強化が行われる前は、ワークロードバランサーには常に現在の週を始点として情報が表示されていました。

ワークロードバランサーの操作について詳しくは、[ワークロードバランサーの操作](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)（Adobe Workfront Classic を使用している場合は[ワークロードバランサーの操作](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス（以前利用可能）

## タスクを別のプロジェクトに移動したりコピーしたりすると、タスクがプロジェクトのタイムライン内に収まる場合、タスクの制約が維持されます

タスクをコピーしたり、別のプロジェクトに移動したりする際に、Workfront が日付特有のタスクの制約を処理する方法を向上しました。日付固有のタスクの制約の例としては、必須開始日、必須終了日、固定日、遅くとも開始する日があります。

例えば、必須開始日の制約があるタスクを、予定開始日がそのタスクの開始日より早い別のプロジェクトに移動またはコピーすると、そのタスクはコピーまたは移動後も制約を保持します。必須開始日の制約があるタスクを、予定開始日がそのタスクの開始日より遅い別のプロジェクトに移動またはコピーすると、そのタスクの制約は「できるだけ早く」に変わります。

この変更を行う前は、タスクの制約は常に「できるだけ早く」に変わります。

タスクの移動については、[タスクを移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)（Adobe Workfront Classic を使用している場合は、[タスクを移動](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

タスクのコピーについては、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)（Adobe Workfront Classic を使用している場合は、[タスクのコピーと複製](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

すべてのタスクの制約の概要については、[タスクの制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)（Adobe Workfront Classic を使用している場合は、[タスクの制約の概要](https://experienceleague.adobe.com/ja/docs/workfront/using/home)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## 詳細タブまたはタスクリストで変更を加える際にデータが失われるのを防ぐ

プロジェクトレベルのタスクリストにあるオブジェクトやタスクの詳細ページの情報を更新して、変更を手動で保存する際、未保存の変更があることを知らせる警告メッセージを表示して、データが失われるのを防ぎます。変更を保存する前に実行できるアクションは、お気に入りにオブジェクトをサブスクライブまたは追加するだけです。

リスト内のタスクの編集について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

**利用可能な環境：**

* 新しい Adobe Workfront エクスペリエンス

## カスタムステータスを使用したグループの承認プロセスの作成

グループで独自のワークフローを容易に管理できるように、承認プロセスでグループ固有のカスタムステータスを使用できるようになりました。

以前は、グループ固有の承認プロセスで、グループ独自のカスタムステータスを使用することはできませんでした。システム全体のステータスのみが使用可能で、これらが常にグループ承認プロセスに適合しているとは限りませんでした。

カスタムステータスは、1 回限りの承認プロセスおよびシステム全体の承認プロセスの両方で使用できるようになりました。

* オブジェクト（プロジェクト、タスクまたはイシュー）に対して1 回限りの承認プロセスを作成し、そのオブジェクトの作業グループに関連するステータスのベースにします。グループに関連付けられているカスタムステータスも含まれます。
* グローバル承認プロセスを作成し、そのグループのみ、またはシステム内の全員が利用できるようにします。

承認プロセスへの管理者アクセス権を持つユーザーの場合、承認プロセスの設定に関する情報は、[作業アイテムの承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)にあります（Adobe Workfront Classic を使用している場合は、[承認プロセスの作成](https://experienceleague.adobe.com/ja/docs/workfront/using/home)を参照してください）。

ユーザーの場合、承認プロセスと作業アイテムの関連付けに関する情報は、[新規または既存の承認プロセスを作業に関連付ける](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)にあります（Adobe Workfront Classic を使用している場合は、[新規または既存の承認プロセスと作業の関連付け](https://experienceleague.adobe.com/ja/docs/workfront/using/home)を参照してください）。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## ワークロードバランサーで割り当てを更新するためのより便利な方法

ワークロードバランサー内の作業アイテムに対するユーザーの割り当てを管理しやすくするために、作業アイテムをダブルクリックできるようになりました。既存の「割り当てを編集」メニューオプションも引き続き使用できます。また、割り当てを更新するために、割り当ての表示を有効にする必要もなくなりました。

ワークロードバランサーでの割り当ての管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

## ワークロードバランサーでのタスクの予定時間数の更新

>[!NOTE]
>
>この機能強化は、2020.2 リリース後間もなく実稼動環境で利用できるようになります。

アクセスレベルのリソース管理エリアに新しいオプションが追加され、このアクセス権を持つユーザーが、ワークロードバランサーから予定時間数を編集できるようになりました。ワークロードバランサーで割り当てを調整する場合、1 日の割り当ての合計は、タスクの予定時間数と一致する必要はありません。割り当てを保存すると、割り当て時間の合計がタスクの予定時間数になります。これは、シンプルな期間タイプを持つタスクでのみ可能です。

ワークロードバランサーでの割り当て管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

リソース管理へのアクセス権の付与について詳しくは、[リソース管理へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)を参照してください。

## ワークロードバランサーからの「ベータ版」ラベルの削除

2020.2 リリースでは、ワークロードバランサーは、ベータ状態ではなくなり、リソースの割り当てと配分の確認と管理にリソースバランサーを使用できるようになります。プレビュー環境で「ベータ版」ラベルが削除されました。同じ変更は、20.2 実稼動リリースでも行われます。ワークロードバランサーについて詳しくは、[ワークロードバランサーの概要](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。
