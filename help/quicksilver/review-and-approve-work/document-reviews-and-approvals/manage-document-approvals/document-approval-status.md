---
product-area: documents
navigation-topic: approvals
title: ドキュメントの決定ステータスの概要
description: ドキュメントの決定ステータスがリストされ、説明されます
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 30a10ed9-ae11-4ff1-a66c-58ea94fe9959
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VESaWT8Xq7iU85LiRJCAL-tldNpXtdLqlTFxSqpK3Ok
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 78%

---

# ドキュメントの決定ステータスの概要

ドキュメントのステータスは、ドキュメントリストで直接表示できます。

![&#x200B; ドキュメントリストのステータス &#x200B;](assets/status-in-doc-list.png)


以下のステータスを使用できます。

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        レビュー保留中</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                レビュー担当者と承認者は通知を受けましたが、まだアセットを開いていません。
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        レビュー中</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>少なくとも 1 人のレビュー担当者がアセットを閲覧しました</p>
                            </li>
                            <li>
                                <p>少なくとも 1 人のレビュー担当者がレビューを完了していません</p>
                            </li>
                            <li>
                                <p>このアセットには承認者が割り当てられていません</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        レビュー済み</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>すべてのレビュー担当者がレビューを完了しました</p>
                            </li>
                            <li>
                                <p>このアセットには承認者が割り当てられていません</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>作業が必要</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>すべての承認とレビューが完了しました</p>
                            </li>
                            <li>
                                <p>少なくとも 1 人の承認者が「作業が必要」との決定を行いました</p>
                                <p>他の承認者は「変更して承認済み」または「承認済み」という決定を行っている可能性があります
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>変更後承認</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>すべての承認とレビューが完了しました</p>
                            </li>
                            <li>
                                <p>少なくとも 1 人の承認者が「変更して承認済み」の決定を行いました</p>
                                <p>他の承認者は「承認済み」という決定を行っている可能性があります
                            </li>
                            <p>注意：このオプションは、レビューと承認にFrame.io統合を使用している場合は使用できません。</p>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>承認済み</p>
                    </td>
                    <td>
                        <ul>
                           <!--
                           <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            -->
                            <li>
                                <p>すべての承認者が「承認済み」という決定を行っている可能性があります
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>



<!--



<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        Pending review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                Reviewers and approvers have been notified, but have not yet opened the asset.
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        In review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>At least one reviewer or approver has viewed the asset</p>
                            </li>
                            <li>
                                <p>At least one reviewer has not completed their review</p><p>Or</p>
                                <p>At least one approver has not made an approval decision</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        Reviewed</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                All reviews are complete
                            </li>
                            <li>
                                There are no approvers
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Needs work</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Needs work"</p>
                                <p>Other approvers may have given decisions of "Approved with changes" or "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>Approved with changes</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Approved with changes"</p>
                                <p>Other approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Approved</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>All approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>


-->
