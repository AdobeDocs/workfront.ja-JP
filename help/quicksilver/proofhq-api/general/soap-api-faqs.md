---
title: SOAP API に関する FAQ
description: SOAP API に関する FAQ
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# SOAP API に関する FAQ

## 最初のファイル配達確認を作成する方法を教えてください。

次の 3 つの簡単な手順を実行します。

**手順 1**：ファイルをに Post リクエストを介して送信し、Workfront Proof にアップロードします。  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). 私たちはあなたにファイルのハッシュを返します — これは非常に重要です！ この段階では、お客様のアカウントに何も表示されないことに注意してください。あなたがこれまで行ったことは、ファイルを送信するだけですが、そのファイルの処理方法を教えてください。

**手順 2**：まだセッション ID がない場合は、 doLogin() または getSessionID() メソッドを使用して取得します。 前者を使用してユーザーの電子メールアドレスとパスワードを使用して「ログイン」するか、後者の方法を使用してユーザーの電子メールアドレスと認証トークンを持っている場合。

**手順 3:** 次に、配達確認を作成する時間です。 createProof() メソッドを使用し、少なくとも必須フィールドを送信します（現在は 5 つしかありません）。 「手順 1」で返されたファイルハッシュに Hash パラメーターを設定してください。設定すると、配達確認の作成時に使用するファイルを指定できます。

アカウントにログインすると、配達確認が表示されます。

## 最初の Web スナップショット配達確認を作成する方法を教えてください。

次の 2 つの簡単な手順を実行します。

**手順 1**：まだセッション ID がない場合は、 doLogin() または getSessionID() メソッドを使用して取得します。 前者を使用してユーザーの電子メールアドレスとパスワードを使用して「ログイン」するか、後者の方法を使用してユーザーの電子メールアドレスと認証トークンを持っている場合。

**手順 2:**次に、配達確認を作成します。 createProof() メソッドを使用し、少なくとも必須フィールドを送信します（現在は 5 つしかありません）。 Hash パラメーターを&quot;web&quot;に設定し、SourceName パラメーターを取得する Web ページの URL に設定してください。

アカウントにログインすると、配達確認が表示されます。

## 配達確認とバージョンの違いは何ですか？

Workfrontの配達確認のバージョンは、単一の配達確認として表示されます。 Web UI で特定のバージョンをクリックすると、そのバージョンの詳細が表示されます。 実際には、各バージョンは個別の配達確認で、Web UI はこれらを一緒に表示します。

API の観点からすると、各バージョンは個別の配達確認で、配達確認は ID で相互にリンクされます。

**createProof()** 常に作成されます **バージョン 1** 配達確認の 例では、この配達確認に対して返された ID「100」があるとします。

を使用する場合 **createProofVersion()** は常に以前のバージョンの ID を送信します。 作成する場合 **バージョン 2** 「100」を証明する場合、 **ParentFileID に&quot;100&quot;を渡す** パラメーター。 これにより、この配達確認はセットのバージョン 2 である必要があるとシステムに伝えられます。 メソッドは、一意の配達確認 ID を返します。例えば、これが「101」であるとします。

3 番目のバージョンの場合、 **バージョン 3** が必要な場合は、 **createProofVersion()** 今回も **ParentFileID に&quot;101&quot;を渡す** リンクされたバージョンのリストが正しく作成されるようにします。

## 呼び出しの前に新しいセッション ID を取得する必要がありますか？

すべてのセッション ID は基本的に、アクションを実行するユーザーであることを示すことが重要です。 

API の呼び出しのたびに、新しいセッション ID を取得する必要はなく、24 時間有効なままになります。 有効期限は、API を呼び出すたびにリセットされます。

## 配達確認/個人 URL とは何ですか？

**チーム/公開**：各配達確認バージョンには、一意のチーム（公開）URL があります。 有効にすると、配達確認が読み取り専用モードで開きます。 チーム URL は、 [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html) メソッド。

**個人**：個人用 URL は、すべてのレビュー担当者および配達確認のバージョンで一意です。 配達確認セットに 3 つのバージョンが含まれ、レビュー担当者がすべてのバージョンに含まれている場合、レビュー担当者には個別に 3 つの個人 URL が割り当てられます。 個人用 URL を指定すると、レビュー担当者が既に特定した配達確認のバージョンが開きます。そのため、配達確認の URL は安全に保たれ、共有されないようにする必要があります。 個人 URL は、 [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html) メソッドを使用し、  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) パラメータ「proof_url」を取得します。

## >Miniproof を開く際にカスタムパラメーターを含めるには？

ミニプルーフを使用すると、校正ツールを独自のページに埋め込むことができます。 「リファラー」パラメーターを縮小配達確認の一部として含めて、ユーザーが縮小配達確認の閉じるボタンをクリックしたときのリダイレクト URL を指定できます。 このリダイレクト URL の一部に任意の数のカスタムパラメーターを含めるには、エスケープされた「&amp;」文字（%26 など）を使用して追加します。

例えば、縮小配達確認の URL などです。
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` は、次のようにエンコードする必要があります： 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` を使用して、カスタムパラメーターを渡すことができます。

## Java Web サービスクライアントを作成する方法は？

[このビデオ](https://screencast.com/t/xsSNrqs5b) に、Eclipse とWorkfront Proof WSDL の定義を使用して Java Web サービスクライアントを作成する方法を示します。

