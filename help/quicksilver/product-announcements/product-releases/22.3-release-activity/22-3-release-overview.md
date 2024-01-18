---
title: 22.3 リリースの概要
description: 22.3 リリースの概要
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bfc7ce9e-b715-47b7-bab7-2e3540d0da3e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3220'
ht-degree: 0%

---

# 22.3 リリースの概要

このページでは、22.3 リリースに含まれる機能について説明します。 一覧に表示されるすべての機能は、新しいAdobe Workfrontエクスペリエンスで使用できます。 一部の機能はAdobe Workfront Classic でも使用できますが、 [Workfront Classic は 2022 年 3 月に廃止されます](https://one.workfront.com/s/new-workfront-experience)。その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります。

これらの機能強化は、2022 年 7 月 11 日の週に実稼動環境で公開されました。

## Adobe Workfrontの機能強化

* [管理者の機能強化](#administrator-enhancements)
* [プロジェクトの強化](#project-enhancements)
* [リソース管理の強化](#resource-management-enhancements)
* [レポートの機能強化](#reporting-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfrontと JumpSeat の統合
</a></p></p> <p>JumpSeat とWorkfrontを統合して、ユーザー向けのカスタムの製品内ガイダンスを作成できるようになりました。 統合を有効にするには、Adobe Workfrontエンタープライズライセンスとアクティブな JumpSeat サブスクリプションが必要です。</p>  
    </td>
    <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">承認プロセスでのロック解除済みステータスの使用
</a></p></p> <p>この機能は、22.3 実稼動リリースから削除されました。 この機能は、将来実稼動環境にリリースされる予定です。</p> 
<p>システム内の承認プロセスとステータスをより詳細に制御できるように、ロックが解除されたシステムステータスに基づいて承認プロセスを作成できるようになりました。 さらに、承認プロセスで既に使用されているステータスをロック解除できるようになりました。 以前は、承認プロセスで使用されるシステムステータスをロックする必要がありました。 これにより、すべてのグループに対して（削除や名前の変更を行わなくても）使用できるようになったので、グループ管理者は、特定のニーズに合わせてグループのステータスリストを合理化できませんでした。</p>   
   </td> 
    <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動リリース： 2022 年 9 月 16 日</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">配達確認のデフォルト設定がWorkfrontに移動されました
</a></p></p> <p>「Workfront Setup」領域内で、次の配達確認設定を編集できるようになりました。</p> 
<ul>
   <li><p>配達確認のデフォルト設定</p></li>
   <li><p>配達確認の決定設定</p></li>
   </ul> 
   </td> 
    <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 2 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームにPDFファイルを追加する
</a></p></p> <p>アドビでは、画像やビデオなど、新しく追加できるアセットウィジェットを使用して、カスタムフォームをより視覚的かつ有益に作成するのに引き続き役立ちます。 これで、カスタムフォームにPDFファイルへのリンクを追加できます。 フォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーは、フォーム内からPDFの表示と操作を行うことができます。</p>
   </td> 
    <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームフィールドの計算エディターにエラー情報が表示されます
</a><span style="color: #ff0000; font-weight: bold;"> （一時的に利用不可）</span></p></p> <p>カスタムフィールドの計算を簡単に編集できるようになりました。計算に直接示される便利なエラー情報が追加されました。 カスタムフォームで計算フィールドを作成する場合、エラーはピンク色で強調表示されます。 ハイライト表示された部分にマウスポインターを置くと、問題の内容を示すツールチップが表示されます。</p>
    </td> 
    <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 10 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">プロジェクトヘッダーのカスタマイズ
</a></p></p> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートの使用時にプロジェクトのヘッダーに表示されるフィールドをカスタマイズできるようになりました。</p>
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
    <td>
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
   </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">空のプロジェクトの作成を制御</a></p></p> <p>システム管理者またはグループ管理者は、テンプレートを使用せずに、空白のプロジェクトを作成できるかどうかを制御できるようになりました。 「設定」の「プロジェクトの環境設定」領域に新しい設定が追加され、次の領域で空のプロジェクトの作成を無効にできるようになりました。</p> 
   <ul>
   <li><p>プロジェクトのリストの「新規プロジェクト」オプションから</p></li>
   <li><p>イシューページからイシューをプロジェクトに変換する場合</p></li>
   </ul>
   <p>新しい設定は、「ユーザーがテンプレートを使用せずにプロジェクトを作成できるようにする」で、デフォルトで有効になっています。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 5 月 20 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用 </p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">グループページからグループを非アクティブ化します。</a> </p> <p>最近では、グループの非アクティブ化と再アクティブ化の機能が追加されました。 この操作を迅速かつ容易にするために、グループのページに追加しました。 グループ名をクリックしてそのページに移動した後、その他のメニューを選択できます。 <img src="assets/more-icon.png"> グループ名の横にある「非アクティブ化」または「再アクティブ化」を選択します。</p> <p>以前は、グループの詳細ページの「アクティブ」チェックボックスを使用してのみ、グループのアクティベートを解除または再アクティブ化できました。 </p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 4 月 15 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用 </p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフォームにビデオを追加する</a> </p> <p>ビデオを追加することで、新しい情報、視覚的な興味、創造性をカスタムフォームに提供できます。 フォームがオブジェクトに添付されている場合、オブジェクトを操作するユーザーはいつでもビデオを再生できます。</p> <p>以前は、カスタムフォームに追加できるのはテキストベースのフィールドと画像だけです。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 4 月 15 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用 </p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">不在作業の委任</a></p> <p>これで、短期間不在を予定している場合に、割り当てられたタスクや問題を一時的に他のユーザーに委任できます。 これにより、不在が完了するのを妨げることがなくなります。</p> 
   <p>この機能強化以前は、承認の委任のみ可能でした。</p></td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 10 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">イシューをタスクに変換する際の新しいエクスペリエンス</a></p> <p>Workfrontを新しいWorkfrontエクスペリエンスと一貫して使用できるように、イシューをタスクに変換するためのインターフェイスを再設計しました。</p> 
   </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 10 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">イシューをテンプレートなしのプロジェクトに変換する際の新しいエクスペリエンス</a></p> <p>Workfrontを新しいWorkfrontエクスペリエンスと一貫して使用できるように、テンプレートを使用せずにイシューをプロジェクトに変換するためのインターフェイスを再設計しました。</p> 
   <p>新しいWorkfrontエクスペリエンスの残りに適した更新されたユーザーインターフェイスに加えて、問題をリストまたはレポートから空のプロジェクトに変換する機能も追加しました。</p></td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">更新ストリームのスマートタグ</a></p> <p>新しい更新を作成したり、既存の更新に返信したりする際の、更新ストリーム内のユーザーのタグ付けを改善しました。 これで、ユーザーにタグを付けて更新に含める際に、ユーザーの名前やアバターに加えて、プライマリの役割と電子メールも表示されるようになりました。 これは、似た名前や同一の名前の複数のユーザーを区別するのに役立ちます。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 5 月 20 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタムフィールドの計算に関する新しい構文</a> </p> <p>カスタムフォームに計算を追加する際に役立つ今後の機能強化に備えて、計算に追加する参照フィールドの構文を標準化しました。 この新しい構文は、フィールド名の入力を開始して選択するときに入力されるので、簡単に使用できます。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 5 月 6 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">共通の役割を持つ 2 人のユーザーが承認プロセスに関与する場合は、正確な情報を保持します</a> </p> <p>作業を承認するためのデータの正確性を確保するため、複数の役割を持つ承認プロセスがアイテムに関連付けられている場合に、アイテムに対する承認情報の記録方法を変更しました。</p> <p>一部の承認プロセスでは 2 つの異なる役割からの承認が必要で、2 つの異なる承認者には、それらの役割の 1 つが共通している場合があります。 これが発生した場合、承認の決定がおこなわれた後、Workfrontでは、各承認者と、承認プロセスに関連付けられているそれぞれの役割が記録されます。</p> <p>この変更がおこなわれる前は、2 人目のユーザーは 1 人目の承認者と 1 人目の承認者の役割の 1 つを共有しているので、両方の承認が記録されていました。 この場合、2 番目の承認者は、最初の承認者の情報を上書きしていました。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 4 月 22 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されました</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">イシューレベルでテンプレートを使用してイシューをプロジェクトに変換する際の新しいエクスペリエンス</a> </p> <p>Workfrontを新しいWorkfrontエクスペリエンスと一貫して使用できるように、イシューページから変換する際に、テンプレートを使用してイシューをプロジェクトに変換する際のインターフェイスを再設計しました。</p> <p>イシューを変換するために選択した後、すぐにお気に入りのリストに簡単にアクセスできるようになりました。</p> <p>再設計されたインターフェイスは、最近更新したテンプレートからプロジェクトを作成する場合のエクスペリエンスと一致します。</p> </td> 
   <td><strong>次の日に利用可能：</strong> 
    <ul> 
     <li> <p>プレビューリリース： 2021 年 12 月 8 日<br></p> </li> 
     <li> <p>実稼動リリース：2022 年 4 月 28 日から段階的なロールアウトがおこなわれます。 <span style="color: #ff0000; font-weight: bold;">この機能は、2022 年 3 月 4 日に実稼動環境から一時的に削除されました。 その後、2022 年 4 月 28 日より段階的に公開されました。 公開日は 2022 年 5 月 5 日。 これは、すべての顧客がプレビューと実稼動で使用できるようになりました。</span></p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">リスト、レポート、ダッシュボードのテンプレートを使用して、問題をプロジェクトに変換する</a> </p> <p>作業の効率を高め、ペースの速い環境で問題を簡単に変換できるように、リスト、レポート、ダッシュボードのテンプレートを使用して問題をプロジェクトに変換する機能が追加されました。</p> <p>この機能強化がおこなわれるまでは、この機能は、イシューページからイシューを変換した場合にのみ存在していました。</p> </td> 
   <td><strong>次の日に利用可能：</strong> 
    <ul> 
     <li> <p>プレビューリリース： 2021 年 12 月 8 日<br></p> </li> 
     <li> <p>実稼動リリース：2022 年 4 月 28 日から段階的なロールアウトがおこなわれます。 <span style="color: #ff0000; font-weight: bold;">この機能は、2022 年 3 月 4 日に実稼動環境から一時的に削除されました。 その後、2022 年 4 月 28 日より段階的に公開されました。 公開日は 2022 年 5 月 5 日。 これは、すべての顧客がプレビューと実稼動で使用できるようになりました。</span></p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">割り当てに変更を加える際に、割り当て時間が削除されなくなります</a> </p> <p>データの正確性を確保するため、割り当て時間を保持し、タスクの割り当てを変更する際にタスクの計画時間を変更しないように変更しました。</p> <p>シンプルな期間タイプのタスクに対して、次の変更が加えられました。</p> 
    <ul> 
     <li> <p>ユーザーとロールを置き換える際に、個々の割り当ての割り当てが保持されます。</p> </li> 
     <li> <p>個々の割り当ての割り当ては、ユーザーを削除する際に役割に対して保持されます。</p> </li> 
    </ul> </td> 
   <td><strong>次の日に利用可能：</strong> 
    <ul> 
     <li> <p>プレビューリリース：2022 年 2 月 11 日<br></p> </li> 
     <li> <p>実稼動リリース： 2022 年 4 月 22 日 </p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されました</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">フォルダー階層の上位 5 レベルのみのフォルダーを共有する</a> （この機能が最初にプレビューで導入された 20.2 リリースノートへのリンクです）。</p> <p>フォルダーを共有するユーザーにとって最高のパフォーマンスを確保するため、現在、共有は 1 つのオブジェクト上のフォルダー階層の上位 5 レベルに制限されています。</p> <p>6 番目以下のフォルダーは、そのすぐ上のフォルダーから共有設定を継承します。</p> </td> 
   <td><strong>次の日に利用可能：</strong> 
    <ul> 
     <li> <p>プレビューリリース：2022 年 2 月 11 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.2 リリースを使用 <span style="color: #ff0000; font-weight: bold;">この機能は一時的に利用できません。 このページは、この機能が実稼動環境で使用可能になると更新されます。</span></p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic は 2022 年 3 月に廃止されます</a>( その後、まもなく 2022 年 7 月にWorkfront Classic のサポート終了日になります )</p> </li> 
    </ul> </td> 
  </tr> 
  <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront Campaigns（ベータ版）</a> </p>
                        <p>現在、Adobe Workfrontに新しいオブジェクトを導入し、作業の管理方法を変更する可能性があります。 </p>
                        <p>Workfront Campaigns を使用すると、様々なポートフォリオやプログラムのプロジェクトを新しい作業用コンテナに整理できます。
Campaigns は、2022 年 7 月に 22.3 リリースでプレビューベータ版にリリースされました。 詳しくは、 <a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">22.3 プロジェクトの機能強化</a> </p>
<p>この新しいコンテナは、現在別々のサイロで管理されている作業オブジェクトを接続するために、今後のリリースで進化する予定です。</p>

</td>
                    <td><span class="bold">次の日に利用可能：</span>
                        <ul>
                            <li>
                                <p>プレビューリリース： 22.4 リリース期間を通じて<br /><span style="color: #ff0000; font-weight: bold;">この機能は、2023 年 1 月 10 日にプレビューから削除される予定です。 詳しくは、 <a href="../23.1-release-activity/23-1-release-overview.md">23.1 リリースの概要ページ</a> </span></p>
                            </li>
                            <li>
                                <p>実稼動版リリース：未定</p>
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">ワークロードバランサーでの並べ替え環境設定とユーザビリティの強化</a> </p> <p>ワークロードバランサーを使用する際のエクスペリエンスを向上させるために、「Unnasigned」セクションと「Assigned」セクションの並べ替えの改善、プロジェクトバーの新しい外観と操作性、予測日付の読みやすいデザインなど、次の機能強化が導入されました。</p> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">リストとレポートのリソース予算フィールドの削除と追加
</a> </p> <p>リソース・プランナからのリソース予算設定情報を反映するために、リストとレポートに新しい「リソース・プランナの予算時間」フィールドを追加しました。 様々なフィールドは、以前のリリースでWorkfrontから削除された廃止されたツールを参照していたので、リストやレポートから削除されました。</p> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 24 日<br></p> </li> 
     <li> <p>実稼動リリース： 2022 年 6 月 24 日</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for Experience Manager Assetsの統合</a> </p> <p>Adobe Workfront Experience Manager Assetsの統合がCloud Service可能になりました。</p>
   <p>また、Cloud ServiceとAssets Essentialsの両方に新しい機能が導入されました。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：なし<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">複数のファイルを 1 つの配達確認でCreative Cloudプラグインで結合</a> </p> <p>Workfrontで複数ファイルの配達確認を作成するために、Adobe Workfrontで作成したコンテンツを使用して、外部のファイルをアップロードできるようになりました。 外部のファイルは、Workfront内に追加の配達確認ページとして表示されます。 この機能強化により、配達確認作成エクスペリエンスのルックアンドフィールも更新しました。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース：なし<br></p> </li> 
     <li> <p>実稼動版リリース：未定</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">新しいSharePoint(Graph API) 統合が利用できるようになりました</a> </p> <p>よりシンプルな新しいSharePoint統合を作成しました。 今は、SharePoint統合を設定する必要はありません。 代わりに、新しいSharePoint統合は、他のドキュメント統合と同様に、単に選択できるオプションです。</p>
   <p>従来のSharePoint統合を通じて現在リンクされているドキュメントへのアクセス権は失われません。 ただし、従来の統合を通じて新しいドキュメントをリンクすることはできません。</p>
   <p>Workfront管理者は、組織のニーズに応じて、SharePointと従来のSharePointの統合を別々に有効化および無効化できます。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">モバイルアプリの校正機能の強化</a> </p> <p>Adobe Workfrontモバイルアプリで、配達確認コメントに関する添付ファイルを表示し、新しい添付ファイルを追加できるようになりました。 添付ファイルでサポートされるファイルタイプは、画像、ドキュメントおよびビデオです。</p> </td>
   <td> <p><b>次の日に利用可能：</b> </p> 
   <p>コメントおよび返信で、他の配達確認ユーザーにタグ付けすることもできます。 タグを付けた人に電子メール通知が届きます。</p>
    <ul> 
     <li> <p>プレビューリリース：なし<br></p> </li> 
     <li> <p>実稼動版リリース：2022 年 7 月中旬～7 月下旬にApple App StoreおよびGoogle Playストアで利用可能。</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">更新されたタイムシート</a> </p> <p>タイムシートの操作時に、エクスペリエンスの改善と更新を継続して行っています。 </p> </td>
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 6 月 3 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">22.3 リリース期間のルックアンドフィールの更新</a> </p> <p>22.3 のリリース期間内に、アプリケーションの様々な領域のルックアンドフィールに対するマイナーアップデートがおこなわれています。 これらの機能強化は、プレビューのリリース後最低 2 週間で実稼動環境で利用できるようになります。</p> </td>
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 22.3 リリース期間を通じて<br></p> </li> 
     <li> <p>実稼動版リリース：プレビューにリリースしてから最低 2 週間（特に指定のない限り）後</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">カスタム OAuth2 アプリケーションで自動更新トークンローテーションを有効にする</a></p> <p>カスタム OAuth2 アプリケーションのセキュリティをより詳細に制御できるように、更新トークンのローテーションを有効にするオプションが追加されました。 このオプションを有効にすると、更新トークンが使用されるたびに、アプリケーションは新しい更新トークンを自動的に作成して送信し、古い更新トークンを無効にします。</p> <p>更新のたびに新しい更新トークンをアプリケーションに保存する必要があります。 Workfrontは、この更新トークンを保存しません。</p> <p>以前は、更新トークンは、カスタム OAuth2 アプリケーション設定で設定された設定時間が経過すると有効期限が切れていました。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 5 月 6 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">シングルページ Web アプリケーションのカスタム OAuth2 統合で PKCE を使用する</a></p> <p>PKCE を使用して、カスタム統合で単一ページ Web アプリケーションを作成できるようになりました。 PKCE は、モバイルアプリケーションなどの動的に更新するアプリケーションで適切に機能する、安全な認証フローですが、すべての OAuth2 クライアントで役立ちます。 PKCE では、静的なクライアントシークレットの代わりに動的に生成された文字列を使用するので、クライアントシークレットの漏洩を防ぐことができます。</p> <p>以前は、カスタム OAuth2 アプリケーションで使用可能なオプションは、ユーザーの名前とパスワード、またはクライアントの秘密鍵のいずれかを使用していました。</p> </td> 
   <td> <p><b>次の日に利用可能：</b> </p> 
    <ul> 
     <li> <p>プレビューリリース： 2022 年 5 月 6 日<br></p> </li> 
     <li> <p>実稼動版リリース： 22.3 リリースを使用</p> </li> 
    </ul> <p><strong>次の環境で使用できます。</strong> </p> 
    <ul> 
     <li> <p>新しいAdobe Workfrontエクスペリエンス </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion の機能強化

Workfront Fusion の新機能は、実稼動環境の 22.3 リリーススケジュール以外のサイクルで使用できます。 最新の機能について詳しくは、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## WorkfrontScenario プランナーの機能強化

リリースのこの時点では、シナリオプランナーの更新はありません。 この領域は、更新が利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof の機能強化

このリリースでは、現時点でWorkfront Proof の更新はありません。 この領域は、更新が利用可能になると更新されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

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

22.3 リリースでおこなわれたメンテナンスアップデートについて詳しくは、 [Workfrontメンテナンスの更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

## 22.3 リリースウェビナー

22.3 リリースウェビナーは 2022 年 6 月 23 日に提示されました。 記録を表示できます [ここ](https://webinars.on24.com/adobe_workfront/whatsnew223?partnerref=WF1).
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

各Adobe Workfront製品リリースの学習プログラム、学習パス、ビデオ、ガイドに対しておこなわれた最新のアップデートを確認します。 詳しくは、 [トレーニングリリースの更新ページ](https://one.workfront.com/s/training-release-updates).

## サポートされなくなった機能

### Internet Explorer 11

Internet Explorer のサポートが削除され、WorkfrontはMicrosoft Edge を正式にサポートするようになりました。

サポートされているブラウザーについて詳しくは、 [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).
