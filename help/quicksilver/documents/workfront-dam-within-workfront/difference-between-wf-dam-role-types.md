---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfront ライセンスの役割タイプと Adobe Workfront DAM の役割タイプの比較
description: Adobe Workfront 管理者は、アクセスレベルを使用して、アプリケーションでユーザーが実行できる操作を決定します。
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: ht
source-wordcount: '471'
ht-degree: 100%

---

# Adobe Workfront ライセンスの役割タイプと Adobe Workfront DAM の役割タイプの比較

Adobe Workfront 管理者は、アクセスレベルを使用して、アプリケーションでユーザーが実行できる操作を決定します。

* Workfront では、ユーザーのアクセスレベルはライセンスで決まります。
* Workfront DAM では、役割タイプによって、DAM 内のアセットに対するユーザーのアクセス権が定義されます。

ライセンスタイプと役割タイプは互いに交換できないので、一方のアプリケーションにおけるアクセスレベルが割り当てられていても、他方のアプリケーションへのアクセス権があるわけではありません。例えば、ユーザーが Workfront のワークライセンスを持っていても、Workfront DAM 内のコントリビューターの役割は自動的には割り当てられません。

## Workfront ライセンスタイプ

Workfront 管理者は、ライセンスタイプを割り当てることで、ユーザーのアクセスレベルを定義します。各ライセンスには、ユーザにライセンスを割り当てる前に変更できるデフォルトのアクセス機能のセットが付属しています。 

ライセンスを使用して、Workfront でユーザーが表示および実行できる内容を決定します。Workfront では、以下の 5 種類のライセンスタイプを使用できます。

* プラン
* ワーク
* レビュー
* リクエスト
* 外部

Workfront の様々なライセンスタイプについては、[レガシーライセンスの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)を参照してください。

## Workfront DAM の役割タイプ

Workfront DAM の Workfront 管理者は、ユーザーに役割タイプを割り当てて、アセットに対するアクセス権を定義します。さらに役割タイプは、ユーザーが作業できる DAM 内のエリアも指定します。

役割タイプは、ユーザーのアクセス権を確立する際に、グループと連携して機能します。グループは、フォルダーやアセット自体に対するユーザーのアクセス権を制御します。アセットでユーザーが実行できるアクションは、役割タイプで決まります。すべての DAM ユーザーを、少なくとも 1 つのグループに関連付ける必要があります。役割タイプとアクセス設定について詳しくは、Workfront DAM のヘルプを参照してください。

Workfront DAM では、以下の 4 つの異なる役割タイプを使用できます。

### Brand Portal

この役割タイプを持つユーザーは、DAM で Brand Connect ポータルのみにアクセスできます。ポータル内で、ユーザーは権限を持っているアセットを表示およびダウンロードできます。

Brand Portal ユーザーは、ライトボックスを作成し共有することで、他のユーザーと共同作業を行えます。

### 標準ユーザー

この役割タイプを持つユーザーは、Workfront DAM および Brand Connect ポータルからアセットを表示およびダウンロードできます。

標準ユーザーは、ライトボックスを作成し共有することで、他のユーザーと共同作業も行えます。

### コントリビューター

この役割タイプを持つユーザーは、Workfront DAM と Brand Connect ポータルにアクセスできます。

コントリビューターは、アクセス権を持つアセットやフォルダーの表示、ダウンロード、アップロード、編集、移動および削除を行うことができます。さらにコントリビューターは、ライトボックスを作成し共有することで、他のユーザーと共同作業を行えます。 

### 管理者

Workfront 管理者は、期限切れのアセットや非アクティブなステータスのアセットも含め、Brand Connect ポータルおよび Workfront DAM 内のあらゆるものにアクセスできます。

管理者アクセス権を持つには、管理者の役割タイプを持つユーザーが管理者グループに属している必要があります。
