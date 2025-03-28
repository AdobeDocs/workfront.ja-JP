---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: 新しいコメントエクスペリエンス
description: Adobe Workfront のコメント機能エクスペリエンスのアップデートは現在開発中です。この更新には、新しいインターフェイス、新機能、一部のオブジェクトの「更新」セクションのパフォーマンスの向上などが含まれています。
author: Alina
feature: Product Announcements
role: User
hide: true
hidefromtoc: true
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 62%

---

# 新しいコメントエクスペリエンス

<!--take out legacy, preview, prod references from below-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

-->

>[!IMPORTANT]
>
>この記事の情報では、新しいコメントエクスペリエンスにリリースされた機能について説明しています。
>
>新しいコメント機能のベータ版プログラムは 2023 年 4 月に開始し、2023 年 10 月に終了して、2023 年 10 月リリースを迎えました。
>
>2024 年 4 月 11 日（PT）以降、新しいコメント機能は、すべてのお客様の実稼動環境で利用できるようになりました。
>
> 以前のコメント機能がWorkfrontから削除されました。

## 機能

新しいコメントエクスペリエンスには、Adobe Workfront オブジェクトの「更新」セクションの改善と変更が含まれています。

新しいコメントエクスペリエンスの改善点には以下が含まれます。

* パフォーマンスとユーザーエクスペリエンスの向上
* システムアクティビティの更新からのユーザーコメントの分離
* オブジェクトに新しいコメントが追加されたときのリアルタイムインジケーター
* コメントの送信後の編集

次の機能が新しいエクスペリエンスから削除されました。

* システム更新に対するコメント。過去にシステム更新に追加されたコメントが、新しい「システムアクティビティ」タブに読み取り専用コメントとして読み込まれました。
* タスクとイシューに関するコメントを作成中に、ステータス、条件、コミット日、完了率を編集できる機能。

  代わりに、これらのフィールドをタスクとイシューの概要パネルに追加して、リスト、ホーム、Workfront バランサーまたはタイムシートから簡単にアクセスできるようにすることをお勧めします。
* カスタムフォームを編集する機能
* Workfront 管理者またはグループ管理者が別のユーザーとしてログインし、そのユーザーに代わってコメントを追加したときの「&lt; user name > の代理」情報は、当初は削除されましたが、2023年10月19日に復元しました。
* ドキュメントにコメントを追加する際に担当者にタグを付けるときの「承認を依頼する」オプション。
* ユーザーのプロファイルボックスを編集する際の「完了率を更新状態に表示」する設定は削除されました。タスクまたはイシューの完了率を更新する機能は削除されました。


<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

新しいコメントエクスペリエンスで使用できる機能と、それらがサポートされているエリアでの機能の使用可否を次の表に示します。

<table>
  <tr>
   <td><strong>機能</strong>
   </td>
   <td><strong> 古いコメント体験に存在する </strong>
   </td>
   <td><strong>新しいコメントエクスペリエンスに存在</strong>
   </td>

<td><strong> 新しいコメント体験 </strong> ージで導入
   </td>
   </tr>
  <tr>
   <td>コメントの作成／読み取り／返信／削除 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>

<td> 
   </td>

</tr>
  <tr>
   <td>リッチテキスト（引用と絵文字を除く）
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>

<td> 
   </td>
  </tr>

<tr>
   <td>リッチテキスト（絵文字）
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>

</tr>

<tr>
   <td>リッチテキスト（ブロック引用）
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
    <td> 2023年第 2 四半期
   </td>

</tr>
  <tr>
<tr>
   <td> コメントの引用
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 2023年第 2 四半期
   </td>

</tr>
  <tr>
   <td>コメントへの反応（「いいね！」） 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>

</tr>
  <tr>
   <td>コメントに画像を添付 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
      <td> 
   </td>

</tr>
  <tr>
   <td>コメント内で人物にタグ付け 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>

</tr>
  <tr>
   <td>スレッド参加者を削除
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>スレッドのすべての参加者に自動的にタグを付ける
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>会社の非公開のコメント 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>コメントの投稿を取り消す 
   </td>
   <td>✓ 
   </td>
   <td>編集コメントに置き換え 
   </td>
     <td> 
   </td>
  </tr>
  <tr>
   <td>システムの更新をオフにする 
   </td>
   <td>✓ 
   </td>
   <td>「アクティビティ」タブに置き換え 
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>コメントを編集 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>ページから移動する際にコメントのドラフトを保存 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>新しいコメントをリアルタイムで表示（コメントが削除された際の表示を含む）
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>時間のログ記録 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>スレッド リンクをコピー 
   </td>
   <td>✓ 
   </td>
   <td> 「リンクをコピー」に置き換え
   </td>
   <td>2023年第 2 四半期 
   </td>
  </tr>
  <tr>
   <td>コメントリンクをコピー 
   </td>
   <td>✓ 
   </td>
   <td> 「リンクをコピー」に置き換え
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>コメントテキストを引用 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
  <td>2023年第 2 四半期 
   </td>
   </tr>
  <tr>
   <td>本文をコピー 
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td>
   </td>
   </tr>
    <tr>
   <td>コメント内を検索 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td>2024年第 1 四半期 
   </td>

</tr>

<tr>
   <td>コメント内の画像をコピーして貼り付ける
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td>2024年第 1 四半期 
   </td>
     </tr>

<tr>
   <td>コメント内の画像をドラッグしてドロップする
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td>2024年第 1 四半期 
   </td>
    </tr>

<tr>
   <td>カスタムフォームを編集 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>コメント中にステータス、条件、コミット日を編集可能 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>システム更新に返信 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>別のユーザーとしてログインしコメントを追加する際に「代理」として表示
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td>
   </td>
  </tr>

<tr>
   <td>「更新」セクションでコミット日が変更された場合に、プロジェクト所有者がタスクの予定完了日を変更できる機能
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
</table>

## リリースタイムライン

>[!IMPORTANT]
>
>ベータ期間に新しいコメントエクスペリエンスにリリースされた機能について詳しくは、[新しいコメント機能のベータ版エクスペリエンスのリリースアクティビティ](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)を参照してください。
>
>Workfront オブジェクトの更新の管理について詳しくは、[作業の更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。


次の情報は、実稼動環境への新しいコメント機能エクスペリエンスのリリースの主要なマイルストーンとタイムラインの説明です。 以下のマイルストーンに加えて、小さな機能強化も継続して行いコメントエクスペリエンスを改善し続けます。

ベータ版期間終了後に新しいコメントエクスペリエンス用にリリースされた機能については、現在のリリースの概要ページを参照してください。 詳しくは、[ 製品リリース ](/help/quicksilver/product-announcements/product-releases/product-releases.md) を参照してください。

次に、新しいコメントエクスペリエンスのリリースの予定タイムラインを示します。

* 23.2 リリース（2023年4月6日（PT））：
   * イシューに関するコメント機能のBetaを立ち上げました
   * 目標に関する新しいコメント機能を（唯一のエクスペリエンスとして）リリースしました
* 23.3 リリース（2023年7月20日（PT））：
   * プロジェクト、タスク、ドキュメントへのコメント機能のBetaを立ち上げました。
   * ボード領域のカードの新しいコメント機能を（唯一のエクスペリエンスとして）リリースしました
* 2023年第 4 四半期リリース（早期リリースを選択したお客様のみが利用できる限定リリース）：
   * テンプレート、テンプレートタスク、プログラム、ポートフォリオ、チーム、ユーザーおよびタイムシートの新しいコメント機能エクスペリエンス（唯一のエクスペリエンス）がリリースされました
   * プロジェクト、タスク、イシューおよびドキュメントのコメント機能のBetaがデフォルトのオプションに更新されました。 「Beta」ラベルが削除されました。
* 2023年第 4 四半期（23.10）リリース（2023年10月26日）
   * すべての顧客に（唯一のエクスペリエンスとして）テンプレート、テンプレートタスク、プログラム、ポートフォリオ、チーム、ユーザーおよびタイムシートの新しいコメント機能エクスペリエンスをリリースしました。
   * プロジェクト、タスク、イシュー、ドキュメントの新しいコメント機能がデフォルトオプションになりました。

  >[!IMPORTANT]
  >
  >    これにより、新しいコメント体験のBeta段階が終了しました。

   * 現在の通常の月次および四半期リリースのこの日付部分から始めて、新しいコメントエクスペリエンス用にリリースされたすべての機能を追加しました。
* 2023年末：
   * 従来のコメント機能を、プロジェクト、タスク、イシュー、ドキュメントなどのオブジェクトの補助的なオプションとして維持しました。 新しいコメントエクスペリエンスは、すべてのユーザーに対して、これらのオブジェクトのデフォルトのオプションになります。
   * 新しいコメント機能が、他のすべてのオブジェクトで唯一のエクスペリエンスになりました。

* 2024年第 2 四半期リリース（2024年4月11日（PT））：

  従来のコメントストリームに戻り、新しいコメントストリームをすべてのオブジェクトで唯一のエクスペリエンスにするオプションを削除しました。

* 2024 年 10 月 3 日（PT）:

  「更新」領域の「フィードバックを残す」ボタンを削除しました。

## 新しいコメントエクスペリエンスを検索

Workfrontの次の領域で、新しいコメント機能を使用できます。

* すべてのオブジェクトの「更新」セクションで以下を行います。

  Workfront オブジェクトの更新セクションへのアクセスについては、[更新セクションの概要](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)を参照してください。

* これが使用可能なすべての領域（リスト、タイムシート、ワークロードバランサー、ホーム）のタスク、問題、ドキュメントの概要パネルに表示されます。
* タスクおよび問題のホーム エリア。



<!--

The new commenting experience is currently available for all customers and for all environments.

Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

    * Project
    * Task (this includes Stories)
    * Issue
    * Document

      >[!NOTE]
      >
      ><span class="preview">The legacy commenting experience has been removed from the Preview environment since April 1, 2024. </span>

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

    * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations
    
    There is no option to enable the new commenting experience for iterations. Only the legacy commenting experience is available for iterations. 

-->


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

<!--

To enable the commenting experience option for projects, tasks, issues, and documents: 

1. (Conditional) In the Production environment, go to an object that you want to activate the new commenting experience for, then click **Updates** in the left panel.
1. (Conditional) If it is disabled, enable the **New commenting** option in the upper-right corner of the Updates area to enable it. This should be enabled by default. 
<span class="preview">The New commenting option has been removed from the Preview environment.</span> 

    ![New commenting toggle off](assets/new-commenting-toggle-off-highlighted.png)

1. Start typing an update in the **Comments** tab. The Comments tab is the default tab when the new experience opens

    Or

    Click the  **System Activity** tab to view the activity updates generated by Workfront. 

1. (Optional) To disable the new commenting experience and return to legacy commenting, deselect the **New commenting** option. 

-->
