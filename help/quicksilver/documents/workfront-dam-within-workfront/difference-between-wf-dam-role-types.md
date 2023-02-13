---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfrontライセンスの役割の種類とAdobe Workfront DAM の役割の種類の比較
description: Adobe Workfront管理者は、アクセスレベルを使用して、アプリケーションでユーザーが実行できる操作を決定します。
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 2%

---

# Adobe Workfrontライセンスの役割の種類とAdobe Workfront DAM の役割の種類の比較

Adobe Workfront管理者は、アクセスレベルを使用して、アプリケーションでユーザーが実行できる操作を決定します。

* Workfrontでは、ライセンスはユーザーのアクセスレベルを決定します。
* Workfront DAM では、役割タイプによって、DAM 内のアセットに対するユーザーのアクセス権が定義されます。

ライセンスの種類と役割の種類は入れ替えができないので、1 つのアプリケーションにアクセスレベルを持つと、他のアプリケーションでのアクセスを意味するわけではありません。 例えば、Workfrontの作業用ライセンスを持つユーザーには、Workfront DAM 内で自動的に寄稿者の役割が割り当てられません。

## Workfront ライセンスタイプ

Workfront管理者は、ライセンスの種類を割り当てて、ユーザーのアクセスレベルを定義します。 各ライセンスには、ユーザにライセンスを割り当てる前に変更できるデフォルトのアクセス機能のセットが付属しています。 

ライセンスを使用して、Workfrontでユーザーが表示および実行できる内容を決定します。 Workfrontでは、次の 5 つのライセンスタイプを使用できます。

* 計画
* 作業
* 確認
* リクエスト
* 外部

詳しくは、 [Adobe Workfrontライセンスの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) Workfrontの様々なライセンスタイプの説明

## Workfront DAM の役割タイプ

Workfront DAM Workfront管理者は、ユーザーにロールタイプを割り当てて、アセットに対するアクセス権を定義します。 さらに、役割タイプは、DAM 内のユーザーが作業できる領域を指定します。

ロールタイプは、ユーザーアクセス権を確立する際にグループと連携して機能します。 グループは、ユーザーがフォルダーやアセット自体に対して持つアクセスを制御します。 ロールタイプは、アセットに対してユーザーが実行できるアクションを決定します。 すべての DAM ユーザーは、少なくとも 1 つのグループに関連付ける必要があります。 ロールのタイプとアクセス設定について詳しくは、 Workfront DAM のヘルプを参照してください。

Workfront DAM では、次の 4 つの異なるロールタイプを使用できます。

### Brand Portal

この役割タイプを持つユーザーは、DAM の Brand Connect ポータルにのみアクセスできます。 ポータル内で、ユーザーは権限を持つアセットを表示およびダウンロードできます。

Brand Portalのユーザーは、Lightbox を作成して共有することで、他のユーザーと共同作業できます。

### 正規ユーザー

この役割タイプを持つユーザーは、Workfront DAM および Brand Connect ポータルからアセットを表示およびダウンロードできます。

通常のユーザーは、ライトボックスを作成して共有することで、他のユーザーと共同作業することもできます。

### コントリビューター

この役割タイプを持つユーザーは、Workfront DAM と Brand Connect ポータルにアクセスできます。

寄稿者は、アクセス権を持つアセットやフォルダーの表示、ダウンロード、アップロード、編集、移動、削除をおこなうことができます。 さらに、寄稿者は、ライトボックスを作成して共有することで、他のユーザーと共同作業できます。 

### 管理者

Workfront管理者は、期限切れのアセットや非アクティブなステータスを持つアセットを含め、Brand Connect ポータルおよびWorkfront DAM 内のすべての項目にアクセスできます。

管理者アクセス権を持つには、管理者の役割の種類を持つユーザーが管理者グループに属している必要があります。
