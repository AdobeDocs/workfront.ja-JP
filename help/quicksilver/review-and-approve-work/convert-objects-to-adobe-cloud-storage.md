---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 従来のオブジェクトをAdobe クラウドストレージに変換
description: 従来のWorkfront ストレージオブジェクトをAdobe クラウドストレージに変換できる3つのケースについて説明し、各コンバージョンで何が動き、何が残るかを理解します。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---
# 従来のオブジェクトをAdobe クラウドストレージに変換

多くの場合、Workfront オブジェクトは、ストレージモデルと同様にストレージモデル間でのみ移動、コピー、変換できます。 例えば、タスクを1つのAdobe クラウドストレージプロジェクトから別のAdobe クラウドストレージプロジェクトに移動できます。 具体的には、従来のWorkfront ストレージオブジェクトをAdobe クラウドストレージに変換できます。

* 従来のWorkfront ストレージタスクをAdobe クラウドストレージプロジェクトに変換する
* 従来のWorkfront ストレージポートフォリオをAdobe クラウドストレージポートフォリオに変換する
* 従来のAdobe ストレージテンプレートからWorkfront クラウドストレージプロジェクトを作成する

Adobe クラウドストレージでの移動方向と違いについては、[Adobe クラウドストレージでのWorkfrontへの移動](/help/quicksilver/review-and-approve-work/workfront-storage.md)を参照してください。

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## 従来のタスクをAdobe クラウドストレージプロジェクトに変換

従来のWorkfront ストレージタスクをAdobe クラウドストレージプロジェクトに変換するには、そのタスクで既存のプロジェクトに変換フローを使用します。 コンバージョン時：

* サブタスクとイシューは、新しいプロジェクトに移動します。
* タスクに添付されたドキュメントとその承認ワークフローは、元のプロジェクトに残ります。
* 作業の承認と解決オブジェクトリンクが削除されます。
* 元のタスクが削除されます。

## 従来のポートフォリオをAdobe クラウドストレージポートフォリオに変換する

Workfront管理者は、従来のWorkfront ストレージポートフォリオを設定領域からAdobe クラウドストレージポートフォリオに変換できます。 変換後：

* 従来のWorkfront ストレージプロジェクトをポートフォリオに移動できなくなります。
* ポートフォリオで作成されたすべての新規プロジェクトでは、Adobe クラウドストレージが使用されます。
* Frame.ioは、ポートフォリオのAdobe クラウドストレージプロジェクトのドキュメントのビューアーです。
* 従来のWorkfront ストレージを使用する子プロジェクトは、従来のストレージに残ります。
* 子プログラムはレガシーストレージに残ります。

>[!NOTE]
>
>子レガシープログラムは、誰かが手動でAdobe クラウドストレージプロジェクトを追加した場合にのみ、Adobe クラウドストレージに自動的に変換されます。

詳しくは、[従来のポートフォリオをAdobe クラウドストレージに変換](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md)を参照してください。

## 従来のテンプレートからAdobe クラウドストレージプロジェクトを作成する

従来のWorkfront ストレージテンプレートからプロジェクトを作成する場合、プロジェクト作成ダイアログボックスの「**このプロジェクトをAdobe クラウドストレージに作成**」チェックボックスによって、新しいプロジェクトのストレージタイプが決まります。 チェックボックスの動作は、プロジェクトを作成する場所によって異なります。

* **ポートフォリオ外**: チェックボックスはデフォルトで使用でき、オフになっています。 これを選択して、Adobe クラウドストレージに新しいプロジェクトを作成します。
* **Adobe クラウドストレージポートフォリオ内**: チェックボックスが選択され、ロックされています。 新しいプロジェクトは、ポートフォリオのストレージタイプと一致する必要があります。
* **従来のWorkfront ストレージポートフォリオ内**: チェックボックスは使用できません。 新しいプロジェクトでは、従来のWorkfront ストレージが使用されます。

詳しくは、[ プロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project.md)を参照してください。
