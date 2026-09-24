---
title: 2026年第4四半期ドキュメントの機能強化
description: 2026年第4四半期ドキュメントの機能強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b16738e5fbfa99fe2e9288adc059559fa3a725d3
workflow-type: tm+mt
source-wordcount: '1333'
ht-degree: 3%
---
# 2026年第4四半期ドキュメントの機能強化

このページでは、プレビュー環境への2026年第4四半期リリースで行われたドキュメントの機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第4四半期リリースサイクルのこの時点で利用可能なすべての変更のリストについては、[2026年第4四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)を参照してください。

<!--

## Access Workfront projects in Adobe Creative Cloud apps

>[!NOTE]
>
>Preview: N/A
>Production fast release: [DATE]
>Production for everyone: [DATE]

You can now access your Workfront projects directly from Adobe Photoshop, Illustrator, and InDesign, using the Projects panel. Projects that use Adobe cloud storage appear in the panel, allowing you to open, edit, and save documents in a Workfront project without leaving the app.

The Documents folder structure in a Workfront project is mirrored in the Projects panel. When you open a document from a project folder, edit it, and save, your changes appear in Workfront. You can also request a document approval on any document connected with Photoshop, Illustrator, or InDesign from Workfront.

For more information, see:

* [Adobe Creative Cloud Projects overview](/help/quicksilver/documents/adobe-creative-cloud-projects/adobe-creative-cloud-projects-overview.md)
* [Use Workfront documents in Creative Cloud apps](/help/quicksilver/documents/adobe-creative-cloud-projects/use-wf-documents-in-cc-apps.md)

-->

## 承認テンプレートの表示と使用を許可するユーザーを制御する

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年8月13日（PT）
>すべての人のための制作：2026年10月15日

承認テンプレートは、デフォルトで非公開になりました。 以前は、すべての承認依頼者がシステム内のあらゆるテンプレートを確認できていたため、テンプレートリストは長く、ナビゲートするのが困難でした。 テンプレートは、作成者が共有しない限り、作成したユーザーにのみ表示されます。

テンプレート作成者は、Workfront設定の承認テンプレートリストから、特定のユーザーまたは組織内の全員とテンプレートを共有できます。 承認をリクエストする場合、ユーザーは自分が作成した、または自分と共有されたテンプレートのみを表示します。

この変更は新規と既存の両方のテンプレートに適用され、テンプレートが要求される方法に関係なく、アクセスが一貫して適用されます。

詳しくは、以下を参照してください。

* ドキュメントの承認ワークフローテンプレートの作成の[ テンプレートの共有](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md#share-a-template)
* [ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

## システム管理者による承認テンプレートへの完全アクセス

>[!NOTE]
>
>プレビュー：2026年9月8日（PT）
>プロダクション高速リリース：2026年9月8日（PT）
>すべての人のための制作：2026年9月8日
>[!BADGE スケジュール外]{type=Neutral}

システム管理者は、作成者や共有者に関係なく、アカウント内のすべての承認テンプレートを表示、編集、削除、一括削除できるようになりました。 以前は、システム管理者は他のユーザーと同じ共有ルールの対象となり、作成したテンプレートや共有されたテンプレートのみを表示または管理することができました。

詳しくは、[承認テンプレートの管理](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md)を参照してください。

## WorkfrontでのFrame.io コメントの表示

>[!NOTE]
>
>プレビュー：該当なし
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

文書の承認ワークフローが作成されると、ユーザーはFrame.io ビューアでコメントを残したり、注釈を付けたりできます。 これらのコメントはWorkfrontのコメントパネルには表示されませんが、Frame.io ビューアで表示できます。

Workfrontのコメントパネルに、Frame.ioで新しいコメントが使用可能になったときにわかるメッセージが表示されるようになりました。

詳しくは、[ドキュメントへの更新の追加](/help/quicksilver/documents/managing-documents/add-update-documents.md)を参照してください。

## 承認メールのリンクから直接プルーフアクセス

>[!NOTE]
>
>プレビュー：該当なし
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

ドキュメントにプルーフが添付されている場合、承認メールの「レビューに移動」リンクでプルーフビューアーが直接開かれるようになり、レビュー担当者と承認者はすぐにレビューを開始できるようになりました。 文書にプルーフがない場合、リンクは以前と同様に、文書の「承認」セクションを開きます。

## Adobe クラウドストレージを使用したオブジェクトの承認へのチームの追加

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

Workfront チームを、各人を個別に追加するのではなく、ドキュメントの承認テンプレートまたは承認テンプレートに承認者またはレビュー担当者として追加できるようになりました。

* Adobe クラウドストレージ上のオブジェクト：Workfrontは、アクティブな各チームメンバーを個別に追加するため、承認者リストには常に現在チームのメンバーが反映されます。
* 従来のWorkfront ストレージを使用するオブジェクト：デフォルトでは、チームは1人の参加者として追加されますが、各チームメンバーを個々の参加者として追加できるようになりました。
* 承認テンプレートでは、Workfrontはチームへの参照を保存し、テンプレートを保存する場合ではなく、テンプレートをドキュメントに適用する場合にアクティブなメンバーに展開します。

詳しくは、以下を参照してください。

* [新しいドキュメント領域での承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [レガシードキュメント領域での承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [ドキュメントの承認ワークフローテンプレートの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

## プロジェクトテンプレートにFrame.io ワークスペースを設定する

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

組織でAdobe クラウドストレージを使用しており、Frame.io Enterprise ライセンスをお持ちの場合は、プロジェクトテンプレートのプロジェクト詳細でFrame.io ワークスペースを選択できるようになりました。 テンプレートから作成されたプロジェクトでは、テンプレートに設定されたワークスペースが自動的に使用されるため、プロジェクトの作成時に追加のアクションを必要とせずに、目的のFrame.io ワークスペースにプロジェクトがルーティングされます。

新しいフィールドには、プロジェクトの割り当て権限を持つFrame.io ワークスペースが一覧表示されます。 このフィールドは、いつでもテンプレートで編集可能です。変更内容は、更新後に作成されたプロジェクトにのみ適用されるので、既存のプロジェクトは元のワークスペースを維持します。

テンプレートからプロジェクトを作成すると、そのFrame.io ワークスペースフィールドは読み取り専用になり、Frame.ioのワークスペースにリンクされます。

Frame.io エンタープライズライセンスをお持ちでない場合、プロジェクトは引き続きWorkfrontのデフォルトワークスペースに移動します。

詳しくは、[ プロジェクト テンプレートの編集](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)および[ プロジェクトの概要エリアでの情報の管理](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md)を参照してください。

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

## メール件名のカスタムメッセージ

>[!NOTE]
>
>プレビュー：該当なし
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

ドキュメントの承認時にカスタムメッセージを設定すると、そのメッセージが承認依頼メールの件名にも表示され、設定された期日までに送信されるようになりました。 これにより、レビュー担当者は電子メールを開くことなく、いつ受信トレイに届くのかを直接確認できます。

詳しくは、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

## 新しいドキュメント領域のバージョンパネルを再設計

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

組織でAdobe クラウドストレージを使用している場合、新しいドキュメント領域のバージョンパネルに新しいデザインが追加されます。

* バージョンには「V1」や「V2」などのラベルが付けられ、Frame.ioでの一貫性を高めています。
* 各バージョンは、「承認済み」や「撤回」などの承認ステータスをリストに直接表示します。
* パネルにはバージョン履歴のみが表示されるようになりました。上部には別の「最新ファイル」エントリは表示されなくなりました。

以前は、バージョンには番号付けではなくタイムスタンプが付いていました。

詳しくは、[ドキュメントバージョンを管理](/help/quicksilver/documents/managing-documents/manage-document-versions.md)を参照してください。

## 新しいドキュメント領域の「承認」パネルを再設計

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

組織でAdobe クラウドストレージを使用している場合、新しいドキュメント領域の承認パネルに、バージョン間の承認履歴が表示されるようになりました。

* パネルには、現在のバージョンだけでなく、バージョンを持つすべてのバージョンの承認ワークフローが一覧表示されます。
* 取り消されたワークフローはリストに残るので、以前の決定を確認できます。
* 任意のバージョンを展開すると、パネルを離れることなく、ステージ、承認者の決定、決定ルール、期限が表示されます。

以前は、承認パネルには現在のバージョンのワークフローのみが表示されていました。

詳しくは、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

## Adobe クラウドストレージオブジェクトのコメントに画像を添付する

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年7月30日（PT）
>すべての人のための制作：2026年7月30日
>[!BADGE スケジュール外]{type=Neutral}

統一されたレビューと承認の一環としてAdobe クラウドストレージを使用している組織は、画像ファイルをコメントに直接添付し、フィードバック、コンテキスト、サポートビジュアルを1つの追跡可能なコメントスレッドにまとめることができるようになりました。 これにより、従来のWorkfrontストレージ上の組織のみがコメントに画像を添付できる以前のギャップが解消されます。

Adobe クラウドストレージ組織では、すべてのメディアタイプ画像フォーマットがサポートされるようになりました。 （従来のオブジェクトコメントでは、引き続き.jpg、.gif、および.png ファイルのみをサポートします）。 レガシーオブジェクトまたはAdobe クラウドストレージオブジェクトのコメントでは、画像ファイル以外のファイルはサポートされていません。

詳しくは、[作業の更新](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

## Experience Manager AssetsのアセットをAdobeクラウドストレージにリンクする

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年8月13日（PT）
>すべての人のための制作：2026年10月15日

組織でAdobe クラウドストレージを使用している場合は、Experience Manager Assetsの個々のアセットを、ドキュメントをサポートする任意のWorkfront オブジェクトにリンクできます。 リンクされたコンテンツは自動的に同期されます。Experience Manager Assetsで行った変更はWorkfrontに表示され、Workfrontから離れることなく新しいアセットバージョンを取り込むことができます。

Content Advisorを利用すれば、コンテンツを選択しながら、AI 検索、スマートな提案、キャンペーンの概要の分析などを取得できます。

詳しくは、「[Experience Manager AssetsからAdobe クラウドストレージにコンテンツをリンクする](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md#link-content-from-experience-manager-assets)」を参照してください。

<!--

## Approval workflow templates are private by default

>[!NOTE]
>
>Preview: July 30, 2026
>Production fast release: August 13, 2026
>Production for everyone: October 15, 2026

Approval templates are now private by default. Previously, every approval requester could see every template in the system, which made template lists long and hard to navigate. Now, a template is visible only to the user who created it, unless the creator shares it.

For more information, see:

* [Share a template](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/manage-approval-templates.md#share-a-template) in Manage approval templates
* [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)

-->

