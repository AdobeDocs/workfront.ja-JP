---
title: 22.3 リリースの概要
description: 22.3 リリースの概要
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bfc7ce9e-b715-47b7-bab7-2e3540d0da3e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '3220'
ht-degree: 100%

---

# 22.3 リリースの概要

このページでは、22.3 リリースに含まれる機能について説明します。一覧に表示される機能はすべて、新しい Adobe Workfront エクスペリエンスで使用できます。一部の機能は Adobe Workfront Classic でも使用できますが、[Workfront Classic は 2022年3月に廃止され](https://one.workfront.com/s/new-workfront-experience)、続いて 2022年7月に Workfront Classic のサポートが終了しました。）

これらの機能強化は、2022年7月11日（PT）の週に実稼動環境で公開されました。

## Adobe Workfront の機能強化

* [管理者の機能強化](#administrator-enhancements)
* [プロジェクトの機能強化](#project-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [レポートの機能強化](#reporting-enhancements)
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
   <td> <p><strong>リリース日と環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront と JumpSeat を統合
</a></p></p> <p>JumpSeat とWorkfront を統合して、ユーザー向けのカスタムガイダンスを製品内で作成できるようになりました。統合を有効にするには、Adobe Workfront エンタープライズライセンスと、アクティブな JumpSeat サブスクリプションが必要です。</p>  
    </td>
    <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">ロックを解除されたステータスを承認プロセスで使用
</a></p></p> <p>この機能は、22.3 実稼動リリースから削除されました。この機能は、将来実稼動環境にリリースされる予定です。</p> 
<p>システム内の承認プロセスとステータスをより詳細に制御できるように、ロックが解除されたシステムステータスに基づいて承認プロセスを作成できるようになりました。さらに、承認プロセスで既に使用されているステータスをロック解除できるようになりました。以前は、承認プロセスで使用するシステムステータスは、ロックする必要がありました。これはすべてのグループに当てはまるので、ステータスの削除や名前の変更を行うことができず、グループ管理者は、個々のニーズに合わせてグループのステータスリストを合理化できませんでした。</p>   
   </td> 
    <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動リリース：2022年9月1日（PT）</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">プルーフのデフォルト設定を Workfront に移動
</a></p></p> <p>Workfront の設定エリアで、次のプルーフ設定を編集できるようになりました。</p> 
<ul>
   <li><p>プルーフのデフォルト設定</p></li>
   <li><p>プルーフ決定の設定</p></li>
   </ul> 
   </td> 
    <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月1日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームに PDF ファイルを追加
</a></p></p> <p>画像や動画などの新しいアセットウィジェットを追加することで、より視覚的で役に立つカスタムフォームを作成できるようになります。カスタムフォームに PDF ファイルへのリンクを追加できるようになりました。フォームがオブジェクトに添付されていると、オブジェクトを操作するユーザーは、フォーム内から PDF の表示と操作を行うことができます。</p>
   </td> 
    <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームフィールドの計算エディターにエラー情報が表示されます
</a><span style="color: #ff0000; font-weight: bold;">（一時的に利用不可）</span></p></p> <p>カスタムフィールドの計算を簡単に編集できるようになり、役に立つエラー情報が計算に直接表示されるようになりました。カスタムフォームで計算フィールドを作成しているとき、エラーがピンク色で強調表示されます。強調表示された部分にカーソルを合わせると、問題の内容を説明したツールヒントが表示されます。</p>
    </td> 
    <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月9日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">プロジェクトヘッダーのカスタマイズ
</a></p></p> <p>Workfront 管理者またはグループ管理者は、レイアウトテンプレートの使用時にプロジェクトのヘッダーに表示されるフィールドをカスタマイズできるようになりました。</p>
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
    <td>
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
   </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">空のプロジェクトの作成を制御</a></p></p> <p>システム管理者またはグループ管理者は、テンプレートを使用せずに、空のプロジェクトを作成できるかどうかを制御できるようになりました。設定のプロジェクトの環境設定領域に新しい設定が追加され、次のエリアで空のプロジェクトの作成を無効にできるようになりました。</p> 
   <ul>
   <li><p>プロジェクトのリストの「新規プロジェクト」オプションから</p></li>
   <li><p>イシューページからイシューをプロジェクトに変換する場合</p></li>
   </ul>
   <p>新しい設定は「テンプレートを使用せずにユーザーによるプロジェクト作成を許可する」で、デフォルトで有効になっています。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年5月19日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用 </p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">グループページからグループを非アクティブ化</a> </p> <p>最近では、グループの非アクティブ化と再アクティブ化の機能が追加されました。この操作を迅速かつ容易にするために、グループのページに追加しました。グループ名をクリックしてそのページに移動した後、グループ名の横にある詳細メニュー <img src="assets/more-icon.png"> を選択して、「非アクティブ化」または「再アクティブ化」を選択できます。</p> <p>以前は、グループの詳細ページの「アクティブ」チェックボックスを使用してのみ、グループの非アクティブ化または再アクティブ化できました。 </p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年4月14日<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用 </p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームに動画を追加</a> </p> <p>ビデオを追加することで、新しい情報、視覚的な興味および創造性をカスタムフォームに提供できます。フォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーはいつでもビデオを再生できます。</p> <p>以前は、カスタムフォームに追加できるのはテキストベースのフィールドと画像だけでした。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年4月14日<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用 </p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">不在時の作業の委任</a></p> <p>短期間不在を予定している場合に、割り当てられたタスクやイシューを一時的に他のユーザーにデリゲートできるようになりました。これにより、不在が作業完了の妨げにならないようにします。</p> 
   <p>この機能強化以前は、デリゲートできたのは承認のみでした。</p></td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月9日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">イシューをタスクに変換する際の新しいエクスペリエンス</a></p> <p>Workfront の使用を新しい Workfront エクスペリエンスと一致させるために、イシューをタスクを変換するためのインターフェイスを再設計しました。</p> 
   </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月9日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">イシューをテンプレートなしのプロジェクトに変換する際の新しいエクスペリエンス</a></p> <p>Workfront の使用を新しい Workfront エクスペリエンスと一致させるために、テンプレートを使用せずにイシューをプロジェクトに変換するためのインターフェイスを再設計しました。</p> 
   <p>新しい Workfront エクスペリエンスの残りに一致した更新されたユーザーインターフェイスに加えて、イシューをリストまたはレポートから空のプロジェクトに変換する機能も追加しました。</p></td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">更新ストリームのスマートなタグ付け</a></p> <p>新しい更新を作成したり、既存の更新に返信したりする際の、更新ストリーム内のユーザーのタグ付けを改善しました。これで、ユーザーにタグを付けて更新に含める際に、ユーザーの名前やアバターに加えて、プライマリの役割とメールも表示されるようになりました。これは、似た名前のユーザーや、名前が同じ複数のユーザーを区別するのに役立ちます。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年5月19日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフィールドの計算に関する新しい構文</a> </p> <p>カスタムフォームに計算を追加する際に役立つ今後の機能強化に備えて、計算に追加する参照フィールドの構文を標準化しました。この新しい構文は、フィールド名の入力を開始して選択するときに入力されるので、簡単に使用できます。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年5月5日<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">共通の役割を持つ 2 人のユーザーが承認プロセスに関与する場合は、正確な情報を保持する</a> </p> <p>作業を承認するためのデータの正確性を確保するため、複数の役割を持つ承認プロセスが項目に関連付けられている場合に、項目に対する承認情報の記録方法を変更しました。</p> <p>一部の承認プロセスでは 2 つの異なる役割からの承認が必要で、2 つの異なる承認者には、それらの役割の 1 つが共通している場合があります。これが発生した場合、承認の決定が行われた後、Workfront では、各承認者と、承認プロセスに関連付けられているそれぞれの役割が記録されます。</p> <p>この変更が行われる前は、2 人目のユーザーは承認役割の 1 つを 1 人目の承認者と共有していたため、両方の承認が記録されていました。この場合、2 人目の承認者によって、1 人目の承認者の情報が上書きされていました。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年4月21日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
     <li> <p>Adobe Workfront Classic（<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022年3月に廃止され</a>、続いて 2022年7月に Workfront Classic のサポートが終了しました。）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">イシューレベルでテンプレートを使用してイシューをプロジェクトに変換する際の新しいエクスペリエンス</a> </p> <p>一貫して新しい Workfront エクスペリエンスで Workfront を使用できるように、イシューページからテンプレートを使用してイシューをプロジェクトに変換する際のインターフェイスを再設計しました。</p> <p>イシューの変換を選択した直後から、お気に入りリストにアクセスしやすくなりました。</p> <p>再設計されたインターフェイスは、最近更新したテンプレートからプロジェクトを作成する場合のエクスペリエンスと同じです。</p> </td> 
   <td><strong>利用可能になる日時：</strong> 
    <ul> 
     <li> <p>プレビューリリース：2021年12月8日（PT）<br></p> </li> 
     <li> <p>実稼動リリース：2022年4月28日（PT）から段階的なロールアウトが行われます。<span style="color: #ff0000; font-weight: bold;">この機能は、2022年3月4日（PT）に実稼動環境から一時的に削除されました。その後、2022年4月28日（PT）より段階的に公開されました。公開は 2022年5月5日（PT）に完了しました。現在では、すべての顧客がプレビューと実稼動で使用できるようになっています。</span></p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">リスト、レポート、ダッシュボードからテンプレートを使用してイシューをプロジェクトに変換</a> </p> <p>作業の効率を高め、ペースの速い環境でイシューを簡単に変換できるように、リスト、レポート、ダッシュボードのテンプレートを使用してイシューをプロジェクトに変換できる機能を追加しました。</p> <p>この機能強化以前は、この機能は、イシューページからイシューを変換した場合にのみ利用できました。</p> </td> 
   <td><strong>公開日：</strong> 
    <ul> 
     <li> <p>プレビューリリース：2021年12月8日（PT）<br></p> </li> 
     <li> <p>実稼動リリース：2022年4月28日（PT）から段階的なロールアウトが行われます。<span style="color: #ff0000; font-weight: bold;">この機能は、2022年3月4日（PT）に実稼動環境から一時的に削除されました。その後、2022年4月28日（PT）より段階的に公開されました。公開は 2022年5月5日（PT）に完了しました。現在では、すべての顧客がプレビューと実稼動で使用できるようになっています。</span></p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">割り当てに変更を加える際に、割り当て時間が削除されなくなります</a> </p> <p>データの正確性を確保するため、割り当て時間を保持し、タスクの割り当てを変更する際にタスクの計画時間を変更しないように変更しました。</p> <p>シンプルな期間タイプのタスクに対して、次の変更が加えられました。</p> 
    <ul> 
     <li> <p>ユーザーとロールを置き換える際に、個々の割り当ての割り当てが保持されます。</p> </li> 
     <li> <p>ユーザーを削除しても、個別に付与された割り当ては役割に対して保持されます。</p> </li> 
    </ul> </td> 
   <td><strong>公開日：</strong> 
    <ul> 
     <li> <p>プレビューリリース：2022年2月10日<br></p> </li> 
     <li> <p>実稼動リリース：2022年4月21日 </p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
     <li> <p>Adobe Workfront Classic（<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022年3月に廃止され</a>、続いて 2022年7月に Workfront Classic のサポートが終了しました。）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">フォルダー階層の上位 5 レベルのみのフォルダーを共有</a>（この機能が最初にプレビューで導入された 20.2 リリースノートへのリンクです。）</p> <p>フォルダーを共有するユーザーにとって最高のパフォーマンスを確保するため、現在、共有は 1 つのオブジェクト上のフォルダー階層の上位 5 レベルに制限されています。</p> <p>6 番目以下のフォルダーは、そのすぐ上のフォルダーから共有設定を継承します。</p> </td> 
   <td><strong>公開日：</strong> 
    <ul> 
     <li> <p>プレビューリリース：2022年2月10日<br></p> </li> 
     <li> <p>実稼動版リリース：22.2 リリースを使用<span style="color: #ff0000; font-weight: bold;">この機能は一時的に利用できません。このページは、この機能が実稼動環境で使用可能になると更新されます。</span></p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
     <li> <p>Adobe Workfront Classic（<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022年3月に廃止され</a>、続いて 2022年7月に Workfront Classic のサポートが終了します。）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Campaigns（ベータ版）</a> </p>
                        <p>現在、作業の管理方法を変える可能性がある新しいオブジェクトを Adobe Workfront に導入しているところです。 </p>
                        <p>Workfront Campaigns を使用すると、様々なポートフォリオやプログラムのプロジェクトを新しい作業コンテナに整理できます。
Campaigns は、2022年7月に 22.3 リリースでプレビューベータ版にリリースされました。詳しくは、<a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">22.3 プロジェクトの機能強化</a>を参照してください。 </p>
<p>この新しいコンテナは、現在別々のサイロで管理されている作業オブジェクトを接続するために、今後のリリースで進化する予定です。</p>

</td>
                    <td><span class="bold">公開日：</span>
                        <ul>
                            <li>
                                <p>プレビューリリース：22.4 リリース期間を通じて<br /><span style="color: #ff0000; font-weight: bold;">この機能は、2023年1月9日（PT）にプレビューから削除される予定です。詳しくは、<a href="../23.1-release-activity/23-1-release-overview.md">23.1 リリースの概要ページ</a>を参照してください。</span></p>
                            </li>
                            <li>
                                <p>実稼動リリース：未定</p>
                            </li>
                        </ul>
                    </td>
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">ワークロードバランサーでの環境設定の並べ替えとユーザビリティの強化</a> </p> <p>ワークロードバランサーを使用する際のエクスペリエンスを向上させるために、「未割り当て」セクションと「割り当て済み」セクションの並べ替えの改善、プロジェクトバーの新しいルックアンドフィール、見込日の読みやすいデザインなど、次の機能強化が導入されました。</p> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">リストとレポートのリソース予算計上フィールドの削除と追加
</a> </p> <p>リソースプランナーからのリソース予算計上情報を反映させるために、リストとレポートに新しい「リソースプランナーの予算計上時間」フィールドを追加しました。様々なフィールドは、以前のリリースで Workfront から削除された、非推奨ツールを参照していため、リストやレポートから削除されました。</p> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月24日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：2022年6月23日（PT）</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Experience Manager Assets の統合向けの Adobe Workfront</a> </p> <p>Adobe Workfront Experience Manager Assets の統合が Cloud Service で利用可能になったことをお知らせします。</p>
   <p>また、Cloud Service と Assets Essentials の両方に新しい機能が導入されました。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：該当なし<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Creative Cloud プラグインで複数のファイルを単一のプルーフに結合</a> </p> <p>Creative Cloud 用 Adobe Workfront プラグインで作成したコンテンツを含んだ外部ファイルをアップロードして、Workfront で複数ファイルのプルーフを作成できるようになりました。外部ファイルは、Workfront 内に追加のプルーフページとして表示されます。この機能強化により、プルーフ作成エクスペリエンスのルックアンドフィールも更新されました。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：該当なし<br></p> </li> 
     <li> <p>実稼動リリース：未定</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">新しい SharePoint（Graph API）統合が使用可能に</a> </p> <p>新しくよりシンプルな SharePoint 統合が作成されました。SharePoint 統合を設定しなくてもよくなりました。代わりに、新しい SharePoint 統合は、他のドキュメント統合と同様に、選択できるオプションにすぎなくなりました。</p>
   <p>従来の SharePoint 統合を通じて現在リンクされているドキュメントへのアクセス権は、失われません。ただし、従来の統合を通じて新しいドキュメントをリンクすることはできません。</p>
   <p>Workfront 管理者は、組織のニーズに応じて、SharePoint と従来の SharePoint の統合を個別に有効または無効にすることができます。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">モバイルアプリのプルーフ機能の強化</a> </p> <p>Adobe Workfront モバイルアプリで、プルーフコメントの添付ファイルを表示したり、新しい添付ファイルを追加できるようになりました。添付できるファイルのタイプは、画像、ドキュメントおよびビデオです。</p> </td>
   <td> <p><b>公開日：</b> </p> 
   <p>コメントと返信で、他のプルーフユーザーをタグ付けすることもできます。タグ付けされたすべてのユーザーにメール通知が届きます。</p>
    <ul> 
     <li> <p>プレビューリリース：該当なし<br></p> </li> 
     <li> <p>実稼動リリース：2022年7月中旬～下旬に Apple App Store および Google Play ストアで入手できます。</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">タイムシートの更新</a> </p> <p>タイムシートの使用時のエクスペリエンスを継続的に向上させ更新しています。 </p> </td>
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年6月2日（PT）<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">22.3 リリース期間中のルックアンドフィールの更新</a> </p> <p>22.3 リリース期間に、アプリケーションの様々な領域のルックアンドフィールに対するマイナーアップデートを行っています。これらの機能強化はプレビューにリリース後、最低 2 週間で実稼動環境で利用できるようになります。</p> </td>
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：22.3 リリース期間中<br></p> </li> 
     <li> <p>実稼動リリース：プレビューにリリースしてから最短で 2 週間後（特に指定のない限り）</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタム OAuth2 アプリケーションで更新トークンの自動ローテーションを有効化</a></p> <p>カスタム OAuth2 アプリケーションのセキュリティをよりきめ細かく制御できるように、更新トークンのローテーションを有効にするオプションを追加しました。このオプションを有効にすると、アプリケーションは更新トークンを使用するたびに、新しい更新トークンを自動的に作成して送信し、古い更新トークンを無効にします。</p> <p>アプリケーションでは、更新のたびに新しい更新トークンを保存する必要があります。Workfront は、この更新トークンを保存しません。</p> <p>これまでは、カスタム OAuth2 アプリケーション設定で指定された設定時間が経過すると、更新トークンの有効期限が切れていました。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年5月5日<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">シングルページ web アプリケーションのカスタム OAuth2 統合で PKCE を使用</a></p> <p>PKCE を使用して、カスタム統合でシングルページ web アプリケーションを作成できるようになりました。PKCE は、モバイルアプリなどの動的に更新するアプリケーションでうまく機能するセキュアな認証フローですが、すべての OAuth2 クライアントで役に立ちます。PKCE では、静的なクライアントシークレットではなく、動的に生成された文字列を使用するので、クライアントシークレットの漏洩のリスクを排除できます。</p> <p>これまでは、カスタム OAuth2 アプリケーションで使用できるオプションは、ユーザー名とパスワードか、クライアントシークレットのいずれかでした。</p> </td> 
   <td> <p><b>公開日：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：2022年5月5日<br></p> </li> 
     <li> <p>実稼動版リリース：22.3 リリースを使用</p> </li> 
    </ul> <p><strong>利用可能な環境：</strong> </p> 
    <ul> 
     <li> <p>新しい Adobe Workfront エクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境では 22.3 リリーススケジュール以外のサイクルで利用できます。最新機能について詳しくは、[Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

## Workfront Scenario Planner の機能強化

リリースの現時点では、シナリオプランナーの更新はありません。このエリアは、アップデートが利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof の機能強化

リリースの現時点では、Workfront Proof の更新はありません。このエリアは、アップデートが利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Workfront Goals の強化

リリースの現時点では、Workfront Goals の更新はありません。このエリアは、アップデートが利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API バージョン 14

API バージョン 14 では、いくつかのリソースとエンドポイントが変更されました。変更の中には、新しい機能をサポートするものもあれば、API を通じて利用可能な情報をより簡単に使用できるようにするものもあります。

新機能と更新内容については、[API バージョン 14 の新機能](../../../wf-api/api/new-api-version-14.md)を参照してください。

API バージョンの詳細については、[API のバージョン管理とサポートスケジュール](../../../wf-api/api/api-version-support-schedule.md)を参照してください。

## Workfront のメンテナンスアップデート

22.3 リリース時に実施されたメンテナンス更新については、[Workfront メンテナンス更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja)を参照してください。

## 22.3 リリースウェビナー

22.3 リリースウェビナーは 2022年6月23日（PT）に実施されました。その録画を[こちら](https://webinars.on24.com/adobe_workfront/whatsnew223?partnerref=WF1)で視聴できます。
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Workfront 22.2 Release Webinar will be presented on March 24, 2022 at 8:00 a.m. MST. You can register for the event on the <a href="https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne" target="_blank">Events page on Workfront One</a>.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
</p>
-->

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

各 Adobe Workfront 製品リリースの学習プログラム、学習パス、ビデオ、ガイドに加えられた最新の更新を確認します。詳しくは、[トレーニングリリースの更新ページ](https://one.workfront.com/s/training-release-updates)を参照してください。

## サポートされなくなった機能

### Internet Explorer 11

Internet Explorer のサポートが廃止され、Workfront は Microsoft Edge を正式にサポートするようになりました。

サポートされているブラウザーについて詳しくは、[Adobe Workfront のブラウザー要件](../../../workfront-basics/workfront-browser-requirements.md)を参照してください。
