---
title: 2026年第 2 四半期の管理者の機能強化
description: 2026年第 2 四半期の管理者の機能強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ce152c48-ed72-47ed-b1c5-940c93b4a9ec
source-git-commit: 9160a68653999c35de32dd417b18ea8197ef446f
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 20%

---

# 2026年第 2 四半期の管理者の機能強化

このページでは、2026 年第 2 四半期リリースで行われた、プレビュー環境に対する管理者の機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2026年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)を参照してください。



## リッチテキストフィールドタイプがカスタムフォームで使用できるようになりました

>[!NOTE]
>
>プレビュー：2026 年 1 月 29 日（PT）
>実稼動迅速リリース：2026 年 2 月 12 日（PT）
>すべてのユーザー向けの実稼動：2026 年 4 月 16 日（PT）
>
>この機能は、2026 年 2 月 13 日（PT）に実稼動環境から一時的に削除されました。

カスタムフォームの新しい **リッチテキスト** フィールドタイプは堅牢なテキストエディターで、太字、斜体、下線、箇条書き、番号付け、ハイパーリンク、ブロック引用の従来のオプションに加えて、上付き文字、下付き文字、見出し、表などの書式設定オプションが用意されています。 文字数の制限は 15,000 のままです。

リッチテキストフィールドタイプが、テキストを書式設定フィールドタイプに置き換えています。 右側のフィールドオプションのボタンをクリックして、フィールドが書式設定されている既存のテキストをリッチテキストにすばやく変換できます。 変換する場合、履歴データはフィールドに残り、レポートでも同じように使用されます。

詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

## Workfront メール通知用の新しい IP アドレス

Workfrontからメール通知を送信するために使用される IP アドレスを更新しています。 メールまたはファイアウォールの許可リストを維持している場合、Workfrontの通知を引き続き配信するには、以下に新しい IP アドレスを追加する必要があります。

これらの更新は、承認、リマインダー、プルーフ通知、その他のシステムメッセージなど、Workfront アプリケーションで生成されたすべてのアウトバウンドメールに適用されます。

米国：

* 206.55.149.212
* 206.55.149.214
* 206.55.149.215
* 206.55.149.213
* 206.55.149.211

EU:

* 24.110.76.224
* 24.110.76.223

詳しくは、[ファイアウォールの許可リストの設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。
