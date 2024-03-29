---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 削除した項目を復元
description: Workfront の管理者は、過去 30 日間に削除されているプロジェクト、タスク、イシュー、ドキュメントおよびテンプレートを Adobe Workfront で復元できます。30 日が経過すると、これらの項目は完全に削除され、復元できなくなります。オブジェクトを復元すると、その子オブジェクトとフィールドもすべて復元されます。例えば、プロジェクトを復元すると、そのプロジェクト内のすべてのタスク、イシュー、ドキュメント、時間、メモ、割り当て、カスタムデータも復元されます。
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 82%

---

# 削除した項目を復元

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront の管理者は、過去 30 日間に削除されているプロジェクト、タスク、イシュー、ドキュメントおよびテンプレートを Adobe Workfront で復元できます。30 日が経過すると、これらの項目は完全に削除され、復元できなくなります。

オブジェクトを復元すると、その子オブジェクトとフィールドもすべて復元されます。例えば、プロジェクトを復元すると、そのプロジェクト内のすべてのタスク、イシュー、ドキュメント、時間、メモ、割り当て、カスタムデータも復元されます。

また、グループ管理者は、管理するグループにあるこれらのオブジェクトを復元することができます。

>[!IMPORTANT]
>
>* レポート、ダッシュボード、ユーザー、グループ、チーム、またはイテレーションを削除した場合、復元することはできません。
>* グループで、グループ管理者以外のユーザーがドキュメントをオブジェクトのドキュメントエリアに直接アップロードした場合、そのドキュメントを復元できるのは Workfront 管理者だけです。
>
>* タスクまたはイシューを移動し、そのタスクまたはイシューに添付されたドキュメントも移動しないように選択した場合、そのドキュメントは削除され、30 日間ごみ箱に入れられます。管理者はそれらを復元し、移動したタスクまたはイシューに再び関連付けることができます。 タスクまたはイシューが移動後に削除された場合、ドキュメントを復元する管理者のユーザーページの「ドキュメント」領域にドキュメントが復元されます。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td><p>新規：標準</p>
   または
   <p>現在：プラン</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;現在のプランまたはライセンスの種類を確認するには、Workfront 管理者に問い合わせてください。

## プロジェクト、タスク、またはイシューを復元する際に復元される情報

プロジェクト、タスク、またはイシューを復元すると、次の関連情報も同時に復元されます。

* 「アップデート」エリアのコメントおよび返信
* 承認
* 割り当て
* カスタムフォーム
* キューの設定
* スコアカード、目標、リスクなどのビジネスケース
* プロジェクトチーム
* 日付
* イシュー
* タスク
* サブタスク
* ステータス
* 財務情報：

   * 請求記録
   * 請求レート
   * 費用

* タイムライン情報：

   * 先行タスク
   * タスクの制約
   * 期間タイプ

* ベースライン

  タスクのベースラインは、親プロジェクトまたはタスクの復元時には復元されますが、個別に削除したタスクの復元時には復元されません。

* 時間（および時間 ID）

  削除されたアイテムに時間が復元されるかどうかは、タイムシートと時間の環境設定を構成する際に選択した設定によって異なります。詳しくは、[オブジェクトが削除および復元される時間への影響の設定](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md)を参照してください。

* 項目の URL

  復元後も、項目の URL は同じままです。ユーザーが項目のブラウザーブックマークを作成した場合、そのブックマークは引き続き有効です。

* アクセスと権限

  項目を削除する前にその項目へのアクセス権があったユーザーは、復元後に再びアクセスできるようになります。

* ドキュメント（プルーフ済みドキュメントを含む）

  ドキュメントとドキュメントのバージョンを復元する際は、次の点を考慮してください。

   * 個別に削除したドキュメントは、個別に復元できます。

     親プロジェクト、タスク、またはイシューと共に削除されたドキュメントは、親を復元すると復元されますが、個別に復元することはできません。

   * ドキュメントの復元時に、ドキュメントまたはドキュメントプルーフのすべてのバージョンが復元されます。\
     個別に削除したドキュメントやドキュメントプルーフの個々のバージョンは復元できません。

## プロジェクト、タスク、イシューの復元時に復元されない情報

プロジェクト、タスク、またはイシューの復元時に、次の関連情報は一緒に復元されません。

* いいね
* 推薦
* リクエストキュー内の取り込みメールアドレス
* お気に入り

  お気に入りメニューを削除する前にこのメニューに追加したプロジェクト、タスク、またはイシューは、お気に入りメニューを復元しても表示されません。

* 解決オブジェクト

  解決プロジェクトは、「**元のイシューを保持し、その解決策を次の&lt;**&#x200B;プロジェクト&#x200B;**または**&#x200B;タスク&#x200B;**>に関連付けます**」オプションで設定された変換済みイシューです。親プロジェクトまたはタスクを削除すると、イシューはそのプロジェクトまたはタスクにリンクされなくなるので、解決オブジェクトとして識別されなくなります。親を復元しても、リンクは復元されません。

  Workfront 管理者またはグループ管理者が、変換時に解決オブジェクトに一致するようにイシューを設定する方法に関して詳しくは、[システム全体のタスクとイシューの環境設定を行う](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)および[グループのタスクとイシューの環境設定を行う](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

  問題の変換について詳しくは、 [Adobe Workfrontでの変換の問題の概要](../../../manage-work/issues/convert-issues/convert-issues.md).

## 項目を復元

{{step-1-to-setup}}

1. **ごみ箱**／**最近削除された項目**&#x200B;をクリックします。
1. 次をクリック： **プロジェクト**, **タスク**, **問題**, **テンプレート**&#x200B;または **ドキュメント** タブに表示されます。

   デフォルトでは、項目が&#x200B;**削除日**&#x200B;列で並べ替えられます。

1. 復元する項目を最大 10 個選択します。

   子タスクを削除すると、そのタスクがリストに表示されます。

   親タスクを削除すると、親タスクのみがリストに表示されます。ただし、親タスクを復元すると、すべての子タスクが復元されます。

1. 「**復元**」をクリックして、選択した項目を元の場所に復元します。
1. （オプション）復元された項目をすばやく表示するには、[復元された項目を表示](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md)に記された手順に従います。

   項目を復元した後の動作の詳細については、「 [項目を復元した後の動作](#what-happens-after-you-restore-items) 」を参照してください。

## 項目を復元した後の動作 {#what-happens-after-you-restore-items}

* タスクとサブタスクを復元すると、削除前の順に表示されます。

  ただし、タスクを削除している間に他のタスクの順序が変更された場合は、タスクまたはサブタスクのリストの下部に復元される可能性があります。

* 項目を復元した後の動作は、以下のようになります。

   * 成功したかどうかを知らせるメッセージが表示されます。

     また、メール通知も受け取ります。複数の項目を復元した場合は、メールにリストが表示されます。

   * コメントは、プロジェクト、タスク、またはイシューのアップデートエリアと、親オブジェクトのアップデートエリアに表示されます。

     これは、ドキュメントまたはテンプレートを復元する場合には発生しません。

## プルーフ復元済み

配達確認のあるドキュメントを復元すると、配達確認の検証アクティビティページに、実際に配達確認を復元した実際のユーザーではなく、組織のインスタンスにリストされた最初のアクティブなWorkfront管理者の名前が（プロファイル ID の順に）表示されます。
