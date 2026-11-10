---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境のプロモーションに関するよくある質問
description: Workfront環境プロモーションに関するよくある質問をご覧ください。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
TQID: 'https://experienceleague.adobe.com/f8iQHTrVCbtK-tIFlCmojM-FQfV0JLCMa6hVfWCEzXY'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: d00e08bb44ff533f6bbdbbe6f932a85533514269
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 7%
---
# 環境のプロモーションに関するよくある質問

環境プロモーションに関してよく質問される質問です。

## クロスドメインプロモーションはサポートされていますか？

### 回答

クロスドメイン環境のプロモーションは現在サポートされていません。 同じドメイン内の環境間で昇格する必要があります。

## Workfront インスタンスがPrimeまたはUltimate ライセンスを使用しているかどうかを確認するにはどうすればよいですか？

### 回答

* Workfront管理者は、組織のライセンスを検索できます。

  1. Workfrontの左上隅にある&#x200B;**[!UICONTROL メインメニュー]** アイコン ![ メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックし、**[!UICONTROL セットアップ]** ![ セットアップアイコン ](/help/_includes/assets/gear-icon-setup.png)をクリックします。
  1. 左側のパネルで、「**システム**」をクリックします。
  1. Workfront プランを表示するには、「**ライセンス**」を選択します。
プランがページの右上隅付近に表示されます。
     ![ プランの検索](assets/locate-plan.png)

  または
* Workfrontの担当者にお問い合わせください。

## 環境保護は双方向ですか？

### 回答

はい。 例えば、SandoxからProductionに、またはProductionからSandboxに昇格できます。

## 共有はサポートされていますか？

### 回答

いいえ、共有は現在サポートされていません。

## パッケージのロールバックは利用できますか？

### 回答

パッケージのロールバックは、最新のパッケージで、パッケージのインストールから24時間以内に利用できます。

## 個々のコンポーネントのプロモーションをスキップするオプションはありますか？ オプション `Use Existing`、`Overwrite`、`Save with a new Name`&quot;が存在する場合、個々のパラメーターのプロモーションをスキップできるように`Skip`を追加できますか？

### 回答

* 「既存のオブジェクトを使用」は、ターゲット環境の既存のオブジェクトにマッピングされ、変更を行わないため、「スキップ」またはデプロイメントを無視することと同じです。
* オブジェクトをスキップするには、プロモーションパッケージから、またはソース環境から直接インストールしないオブジェクトを削除することをお勧めします。 オブジェクトを削除した後、パッケージを再構築します。
