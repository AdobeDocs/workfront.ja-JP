---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: 2019.4 のその他の機能強化
description: このページでは、2019.4 リリースで行われた様々な機能強化について説明します。2019年11月11日（PT）の週に実稼動環境で公開されます。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 100%

---

# 2019.4 のその他の機能強化

このページでは、2019.4 リリースで行われた様々な機能強化について説明します。2019年11月11日（PT）の週に実稼動環境で公開されます。

2019.4 で行われたすべての変更のリストについては、[2019.4 リリースの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Adobe CC ドキュメントから自動プルーフワークフローを開始</strong> <p>作成した Adobe CC ドキュメントの自動プルーフワークフローを、Adobe CC から離れることなく開始できます。詳しくは、<a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Workfront Extension for Illustrator と InDesign の使用</a>の記事の <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Illustrator または InDesign からプルーフを生成</a>を参照してください。</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>メールアドレスの重複を防止</strong> <p>Workfront で複数のユーザーを作成する際に、同じメールアドレスを使用できなくなりました。アドレスが大文字と小文字で異なる場合でも使用できません。例えば、あるユーザーをメールアドレス JohnDoe@example.com で、別のユーザーをメールアドレス johndoe@example.com で作成することはできません。 </p> <p>この変更を行う前は、大文字と小文字で異なる、同じメールアドレスのユーザーを作成することができました。 </p> <p>メモ：大文字と小文字が異なるだけでメールアドレスが同じ既存のユーザーは、将来更新する必要があります。Workfront インスタンス内に大文字と小文字が異なるだけでメールアドレスが同じユーザーがいる場合、Workfront から追加のお知らせと変更が必要な期限をご連絡します。</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>カスタムフォームの先行入力フィールドで使用できるオブジェクトタイプを追加</strong> 
     <p>先行入力のカスタムフィールドを作成する際に、ユーザー、会社、グループ、担当業務、ポートフォリオ、プログラム、プロジェクト、テンプレートの各オブジェクトタイプをフィールドに関連付けることができるようになりました。</p> 
     <p>以前は、ユーザーのオブジェクトタイプのみを先行入力カスタムフィールドに関連付けることができました。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>ドキュメントの最新バージョンのファイル名を表示</strong> <p>ファイル名が既存のバージョンとは異なるバージョンのドキュメントをアップロードすると、その新しいファイル名が Workfront に表示されるようになりました。</p> <p>以前は、異なるファイル名で新しいバージョンを追加しても、引き続き以前のバージョンのファイル名が Workfront で表示されていました。</p> <p>詳しくは、<a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">新しいバージョンのドキュメントをアップロード</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>カスタムフォームの先行入力フィールドにフィルターを追加</strong> <p>カスタムフォームに先行入力フィールドを追加する際に、ユーザーがフィールドに入力できるオブジェクトを制限するフィルターを追加できるようになりました。例えば、組織のマーケティングチームとセールスチームのメンバーのみを選択できるように、フィールドを制限できます。</p> <p>詳しくは、「カスタムフォームを作成」の記事の「新しいフィールドの作成と追加」の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>カスタムフォームのフィールドの表示タイプを変更</strong> 
     <p>これで、カスタムフォーム内のフィールドの表示タイプを変更できます。</p> 
     <p>例えば、「チェックボックス」フィールドを作成した場合は、そのフィールドを「ドロップダウン」フィールドまたは「ラジオボタン」フィールドに変更できます。これらの 3 つのフィールド表示タイプは相互に入れ替えることができます。</p> 
     <p>また、1 行のテキストフィールドを作成した場合は、そのフィールドを段落テキストフィールドに変更できます。これら 2 つのフィールド表示タイプは交換可能です。</p> 
     <p>以前は、カスタムフィールドの表示タイプを変更するには、新しいフィールドを作成し、古いフィールドを削除する必要がありました。これにはデータの転送が必要でしたが、多くの場合は時間がかかりました。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>休暇カレンダーと報告の作成</strong> 
     <p>ユーザーの休暇を確認して、より適切な計画と実行が可能になりました。また、ユーザーの空き時間をリアルタイムで表示するために、新しい休暇レポートやカレンダーをダッシュボードに追加することもできます。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
