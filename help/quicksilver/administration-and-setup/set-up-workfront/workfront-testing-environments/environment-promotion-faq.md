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
source-git-commit: 2bbfd449d913a5134c9c36b1ee10567973c56eaa
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 16%

---

# 環境推進に関するよくある質問

環境のプロモーションに関するよくある質問を次に示します。

## クロスドメインプロモーションはサポートされていますか？

### 回答

クロスドメイン環境のプロモーションは、現在サポートされていません。 同じドメイン内の環境間で昇格させる必要があります。

## AdobeBusiness Platform/IMS は環境推進のための前提条件ですか？

### 回答

いいえ。環境のプロモーションは、IMS 対応Workfront インスタンスと非 IMS AEM Forms インスタンスの両方で利用できます。

## Workfront インスタンスが Prime または Ultimate ライセンス上にあるかどうかを確認するにはどうすればよいですか？

### 回答

* Workfront管理者は、組織のライセンスを見つけることができます。

   1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
   1. 左側のパネルで、「**システム**」をクリックします。
   1. Workfrontのプランを表示するには、「**ライセンス**」を選択します。
プランがページの右上隅付近に表示されます。
      ![](assets/locate-plan.png)

  または
* Workfront アカウント担当者にお問い合わせください。

## 環境プロモーションは双方向ですか？

### 回答

はい。例えば、サンドボックスから実稼動環境に、または実稼動環境からサンドボックスに昇格させることができます。

## 共有はサポートされていますか？

### 回答

いいえ。共有は現在サポートされていません。

## ロールバック機能が使用できるようになるのはいつですか。

### 回答

ロールバックは最優先事項であり、現在開発中です。 ロールバック機能は、2024 年第 3 四半期または第 4 四半期にリリースされる予定です。

## 個々のコンポーネントのプロモーションをスキップするオプションはありますか？ オプション「`Use Existing`」、「`Overwrite`」、「`Save with a new Name`」が存在する場所に `Skip` 追加して、個々のパラメーターの昇格をスキップできますか？

### 回答


* 「既存を使用」は、ターゲット環境内の既存のオブジェクトにマッピングされ、変更を行わないため、「スキップ」またはデプロイメントを無視するのと同じです。
* オブジェクトをスキップするには、を削除することをお勧めします。
プロモーションパッケージから、またはソース環境から直接インストールしたくないオブジェクト。 オブジェクトを削除した後、パッケージを再アセンブリします。
