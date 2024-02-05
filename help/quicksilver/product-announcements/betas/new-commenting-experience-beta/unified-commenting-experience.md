---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: 新しいコメントエクスペリエンス
description: Adobe Workfront のコメント機能エクスペリエンスのアップデートは現在開発中です。この更新には、新しいインターフェイス、新機能、一部のオブジェクトの「更新」セクションのパフォーマンスの向上などが含まれています。
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 35%

---

# 新しいコメントエクスペリエンス

<!--take out legacy, preview, prod references from below-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.  </span>  

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>この記事の情報は、新しいコメント作成機能にリリースされた機能を指します。
>
>新しいコメンティングエクスペリエンスのベータプログラムは 2023 年 4 月に開始され、2023 年 10 月に終了しました。 新しいコメント作成エクスペリエンスのベータ版プログラムは、2023 年 10 月のリリースで終了しました。
>
>2023 年 10 月から、新しいコメント作成機能の新機能がすべてのお客様にリリースされます。 詳しくは、各リリースの現在のリリースの概要ページを参照してください。

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## 機能

新しいコメントエクスペリエンスには、Adobe Workfrontオブジェクトの「更新」セクションの改善と変更が含まれています。

新しいコメントエクスペリエンスの改善点には以下が含まれます。

* パフォーマンスとユーザーエクスペリエンスの向上
* システムアクティビティの更新からのユーザーコメントの分離
* オブジェクトに新しいコメントが追加されたときのリアルタイムインジケーター
* コメントの送信後の編集

次の機能は、削除されたか、新しいエクスペリエンスで非推奨（廃止予定）になります：

* システム更新に対するコメント
* タスクと問題に関するコメントを作成中に、ステータス、条件、コミット日、完了率を編集できる
* カスタムフォームを編集
* Workfrontまたはグループ管理者が別のユーザーとしてログインし、自分に代わってコメントを追加したときの「&lt; ユーザー名 > の代理」情報が最初に削除されました。 2023 年 10 月 19 日に復帰しました。
* ドキュメントにコメントを追加する際に担当者にタグを付ける際に「承認を求める」オプション。
* ユーザーのプロファイルボックスの編集時の「更新ステータスでパーセント完了を表示」設定は削除されます。 タスクまたはイシューの完了率を更新する機能が削除されました。
* タスクまたはイシューの担当者がコミット日を編集した「更新」領域のプロジェクト所有者に対する通知 <!--ensure this is correct when re remove the legacy and leave only new commenting-->

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
   <td><strong>以前のコメントエクスペリエンスに存在</strong>
   </td>
   <td><strong>新しいコメントエクスペリエンスに存在</strong>
   </td>
   <td><strong>新しいコメントエクスペリエンスで導入予定</strong>
   </td>
   <td><strong>新しいコメントエクスペリエンスでの導入時期</strong>
   </td>
   <td><strong>調査中</strong>
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
   </td>
   <td> 2023年第 2 四半期
   </td>
   <td> 
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
   <td> 
   </td>
   <td> 2023年第 2 四半期
   </td>
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
   </td>
   <td>2023年第 2 四半期 
   </td>
   <td> 
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
   <td> 
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
   <td> 
   </td>
   <td>2023年第 2 四半期 
   </td>
   <td> 
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
   <td>
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
   <td> 
   </td>
   <td>2024 年第 1 四半期 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>コメント内の画像をコピーして貼り付ける
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>2024 年第 1 四半期 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>コメント内の画像をドラッグ&amp;ドロップ
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>2024 年第 1 四半期 
   </td>
   <td> 
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
   <td>
   </td>
   <td> 
   </td>
  </tr>
</table>

## リリースタイムライン

>[!IMPORTANT]
>
>新しいコメント作成機能にリリースされた機能について詳しくは、 [新しいコメントベータ版エクスペリエンスリリースアクティビティ](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Workfront オブジェクトの更新の管理について詳しくは、[作業の更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。


新しいコメントエクスペリエンスを実稼動環境にリリースする予定のタイムラインを、主要なマイルストーンとともに以下に示します。以下のマイルストーンに加えて、より小さな機能強化でコメント作成のエクスペリエンスも引き続き向上します。

ベータ版が終了した後に新しいコメント作成機能としてリリースされた機能について詳しくは、現在のリリースの概要ページを参照してください。

次に、新しいコメント作成エクスペリエンスのリリースに向けた計画的なタイムラインを示します。

* 23.2 リリース（2023年4月6日（PT））：
   * 問題については、Commenting Experience Beta を起動してください。
   * 目標に向けて新しいコメントエクスペリエンスをリリース（唯一のエクスペリエンスとして）
* 23.3 リリース（2023年7月20日（PT））：
   * プロジェクト、タスク、ドキュメントの Commenting Experience Beta を起動します。
   * （唯一のエクスペリエンスとして）ボード領域のカード用の新しいコメントエクスペリエンスをリリースします。
* 2023 年第 4 四半期リリース（限定リリース。高速リリースを選択したお客様のみが利用できます）:
   * テンプレート、テンプレートタスク、プログラム、ポートフォリオ、チーム、ユーザー、タイムシートに関する新しいコメント作成機能をリリースします（唯一のエクスペリエンスとして）。
   * プロジェクト、タスク、問題、ドキュメントに関するコメント作成エクスペリエンスベータ版を更新し、デフォルトのオプションにします。 「Beta」ラベルが削除されました。
* 2023 年第 4 四半期 (23.10) リリース（2023 年 10 月 27 日）
   * テンプレート、テンプレートタスク、プログラム、ポートフォリオ、チーム、ユーザー、タイムシートに関する新しいコメント作成機能を、すべての顧客に（唯一のエクスペリエンスとして）リリースします。
   * プロジェクト、タスク、イシュー、ドキュメントに対する新しいコメント作成機能をデフォルトのオプションにします。

  >[!IMPORTANT]
  >
  >    これにより、新しいコメント作成エクスペリエンスのベータ段階が終了します。

   * 新しいコメントエクスペリエンス用にリリースされたすべての機能は、現在の通常の月次および四半期リリースのこの日付の部分から始まります。
* 2023年末：
   * プロジェクト、タスク、問題、ドキュメントの各オブジェクトのセカンダリオプションとして、従来のコメントエクスペリエンスを保持します。 新しいコメントエクスペリエンスは、これらのオブジェクトのすべてのユーザーのデフォルトオプションです。
   * 新しいコメントエクスペリエンスを他のすべてのオブジェクトの唯一のエクスペリエンスにします。

  >[!NOTE]
  >
  >    繰り返し処理では、従来のコメント操作が引き続きおこなわれます。 新しいコメントエクスペリエンスは、繰り返しでは使用できません。

* 2024 年第 2 四半期（2024 年 4 月）:

   * 「繰り返し」を除き、旧式のコメントストリームに切り替え、新しいコメントストリームをすべてのオブジェクトで唯一のエクスペリエンスにします。

## 新しいコメントエクスペリエンスを検索

&lt;! — 重要：従来のエクスペリエンスを削除したら、このバージョンを「更新」作業記事または「更新」セクションの概要に移動します。繰り返し以外は、エクスペリエンスがすべて異なると言います —>

現在、すべてのお客様およびすべての環境で、新しいコメント作成機能を利用できます。

どのオブジェクトに対してコメント作成機能にアクセスするかに応じて、「更新」セクションに次の機能が表示されます。

* 次のオブジェクトの新しいコメントエクスペリエンスと従来のコメントエクスペリエンスの両方：

   * プロジェクト
   * タスク（ストーリーを含む）
   * イシュー
   * ドキュメント

  >[!TIP]
  >
  >この節で説明するように、新しいコメントエクスペリエンス（有効にした場合）または従来のコメントエクスペリエンス（無効にした場合）を表示するには、「新しいコメント」オプションを使用します。 新しいコメントエクスペリエンスがデフォルトです。

   * 以下に示すオブジェクトの新しいコメントエクスペリエンスのみ。 これらのオブジェクトに対して従来のコメント作成機能を有効にするオプションはありません。

      * 目標

     >[!NOTE]
     >
     >Workfront のこのエリアにアクセスするには、Adobe Workfront Goals に対する追加のライセンスが必要です。詳しくは、[Workfront Goals の使用要件](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md)を参照してください。
      * ボード上のカード
      * チーム
      * テンプレート
      * テンプレートタスク
      * タイムシート
      * プログラム
      * ポートフォリオ
      * ユーザー

* 次のオブジェクトに対する従来のコメントエクスペリエンスのみ：

   * イテレーション

     繰り返しの新しいコメントエクスペリエンスを有効にするオプションはありません。 繰り返しに使用できるのは、従来のコメントエクスペリエンスのみです。


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

プロジェクト、タスク、問題およびドキュメントに対して Commenting Experience オプションを有効にするには：

1. 新しいコメントエクスペリエンスを有効にするオブジェクトに移動し、左側のパネルの「**更新**」をクリックします。
1. （条件付き）無効になっている場合、 **新しいコメント** 」オプションを使用して、この機能を有効にします。 これは、デフォルトで有効になっている必要があります。

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. 「**コメント**」タブで、アップデートを入力します。「コメント」タブは、新しいエクスペリエンスを開いたときのデフォルトのタブです

   または

   「**システムアクティビティ**」タブをクリックして、Workfront で生成されたアクティビティのアップデートを表示します。

1. （オプション）新しいコメントエクスペリエンスを無効にして従来のコメントに戻るには、「 **新しいコメント** オプション。

