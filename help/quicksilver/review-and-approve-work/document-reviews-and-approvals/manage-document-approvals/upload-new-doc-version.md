---
product-area: documents
navigation-topic: approvals
title: 新しいドキュメント バージョンをアップロードし、承認を要求する
description: 新しいドキュメントバージョンをアップロードし、Adobe Workfrontの他のユーザーの承認をリクエストできます。
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: cf2a6353df0ea0e3e1c473092dab5f263a98a2fd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 56%

---


# 新しいドキュメント バージョンをアップロードし、承認を要求する

以前のレビューで「作業が必要」とマークされたドキュメントの場合、新しいバージョンを元のドキュメントにアップロードし、別の承認を開始することができます。

新しいバージョンのファイル名が以前のバージョンのファイル名と異なる場合、Workfront は新しいファイル名を持つドキュメントを表示します。

承認が未処理のドキュメントに新しいバージョンが追加されると、以前のバージョンの承認は「取り消し」と表示されます。 一部の参加者がまだ決定を行っていない場合でも、前回の承認プロセスが終了します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在：Request 以上</p>
   または
   <p>新規：Contributor 以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントに関連付けられたオブジェクトへの編集アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

+++

## ドラッグ＆ドロップを使用して新しいバージョンを追加する

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。

1. ドキュメントがアップロードされるドキュメントエリアに移動します。
1. デスクトップまたは別のブラウザータブから、ドキュメントの新しいバージョンを Workfront の既存のバージョンの上にドラッグします。

   新しいバージョンをドラッグする際に、Workfront ドキュメントフォルダーの上にポインタを合わせると、そのバージョンを開くことができます。次に、ファイルを画面の上部または下部にドラッグして、上下にスクロールできます。

1. 「**ドキュメント**」タブの既存のファイルの上に新しいバージョンをドロップします。

1. ドキュメントがアップロードされたら、それをクリックしてドキュメントの概要パネルを開きます。

1. ドキュメントの概要ウィンドウの「**承認**」セクションにスクロールして、「**追加**」をクリックします。

![](assets/doc-summary-add-approvers.png)

1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. 以前のバージョンのレビュー担当者や承認者をすばやく追加するには、以下に示す名前の横にある「追加」ボタンをクリックします。
   <!--need screenshot when working-->

1. （任意）承認者/レビュアーから役割を変更します。

1. 新しい承認者とレビュアーを追加するには、**レビュアー** または **承認者** をクリックし、ユーザーまたはチームの入力を開始します。

   ![](assets/add-approver-and-deadline.png)