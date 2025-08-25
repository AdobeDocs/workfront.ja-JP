---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 環境推進に関するよくある質問
description: Workfront環境のプロモーションに関するよくある質問を紹介します。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 17%

---

# 環境推進に関するよくある質問

環境のプロモーションに関するよくある質問を次に示します。

## クロスドメインプロモーションはサポートされていますか？

### 回答

クロスドメイン環境のプロモーションは、現在サポートされていません。 同じドメイン内の環境間で昇格させる必要があります。-->

<!--DELETE THIS SECTION MARCH 2026-->

<!--## Is the Adobe Business Platform / IMS a prerequisite for environment promotion?

### Answer

No. Environment Promotion is available for both IMS-enabled and non-IMS Workfront instances.-->

## Workfront インスタンスがPrime ライセンスまたはUltimate ライセンスのどちらにあるか調べるにはどうすればよいですか？

### 回答

* Workfront管理者は、組織のライセンスを見つけることができます。

   1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
   1. 左側のパネルで、「**システム**」をクリックします。
   1. Workfrontのプランを表示するには、「**ライセンス**」を選択します。
プランがページの右上隅付近に表示されます。
      ![ 計画の検索 ](assets/locate-plan.png)

  または
* Workfront アカウント担当者にお問い合わせください。

## 環境プロモーションは双方向ですか？

### 回答

はい。例えば、サンドボックスから実稼動環境に、または実稼動環境からサンドボックスに昇格させることができます。

## 共有はサポートされていますか？

### 回答

いいえ。共有は現在サポートされていません。

## パッケージをロールバックできますか？

### 回答

パッケージのロールバックは、パッケージのインストールから 24 時間以内に、最新のパッケージで使用できます。

## 個々のコンポーネントのプロモーションをスキップするオプションはありますか？ オプション「`Use Existing`」、「`Overwrite`」、「`Save with a new Name`」が存在する場所に `Skip` 追加して、個々のパラメーターの昇格をスキップできますか？

### 回答

* 「既存を使用」は、ターゲット環境内の既存のオブジェクトにマッピングされ、変更を行わないため、「スキップ」またはデプロイメントを無視するのと同じです。
* オブジェクトをスキップするには、プロモーションパッケージまたはソース環境から直接インストールしないオブジェクトを削除することをお勧めします。 オブジェクトを削除した後、パッケージを再アセンブリします。
