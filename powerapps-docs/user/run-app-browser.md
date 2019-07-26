---
title: Web ブラウザーでアプリを実行する | Microsoft Docs
description: このトピックでは、Web ブラウザーでアプリを実行する方法を説明します
author: Mattp123
ms.service: powerapps
ms.component: pa-user
ms.topic: quickstart
ms.date: 11/16/2018
ms.author: matp
manager: kvivek
ms.custom: ''
ms.reviewer: ''
ms.assetid: ''
search.audienceType:
- enduser
search.app:
- PowerApps
- D365CE
ms.openlocfilehash: 31bef01ef46fd0fe2ed7bae30e63d53c169812db
ms.sourcegitcommit: 483c777a1537ccab6a2a2da6a5d1fe4470dd0e7e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/19/2019
ms.locfileid: "63321604"
---
# <a name="run-an-app-in-a-web-browser"></a>アプリを Web ブラウザーで実行する
自分でアプリを作成したり、他のユーザーがあなたとアプリを共有したりしたときは、Windows、iOS、Android、または Web ブラウザーでそのアプリを実行できます。 このトピックでは、キャンバス アプリまたはモデル駆動型アプリを、[Dynamics 365 ホーム ページ](https://home.dynamics.com)から Web ブラウザーで実行する方法を説明します。

このクイック スタートを実行するには、以下が必要です。
- PowerApps のライセンス。 これは、PowerApps プラン ([PowerApps プラン 2 の試用版](https://docs.microsoft.com/powerapps/maker/signup-for-powerapps)など)、または [Microsoft Office 365](https://signup.microsoft.com/Signup?OfferId=467eab54-127b-42d3-b046-3844b860bebf&dl=O365_BUSINESS_PREMIUM&ali=1) または PowerApps を含む [Dynamics 365](https://dynamics.microsoft.com/pricing/) プランのいずれかで入手できます。 
- 自分で作成したアプリ、または他のユーザーが作成して共有されたアプリへのアクセス。
- サポートされている Web ブラウザーとオペレーティング システムへのアクセス。
   - キャンバスアプリについては、以下を参照してください。[システム要件、制限、および構成値](../maker/canvas-apps/limits-and-config.md)
   - モデル駆動型アプリの場合は、以下を参照してください。[サポートされている web ブラウザーとモバイルデバイス](https://docs.microsoft.com/dynamics365/customer-engagement/admin/supported-web-browsers-and-mobile-devices)


## <a name="sign-in-to-dynamics-365"></a>Dynamics 365 にサインインする
[https://home.dynamics.com](https://home.dynamics.com) で Dynamics 365 にサインインします。

## <a name="find-an-app-on-the-home-page"></a>ホーム ページでアプリを探す
ホーム ページには、複数の種類のビジネス アプリが表示される場合がありますが、検索ボックスにアプリ名の一部を入力すると特定のアプリを見つけることができます。 また、一覧をフィルター処理して、特定のソース (PowerApps など) によって作成されたアプリのみを表示することもできます。 そのためには、 **[フィルター]** をクリックまたはタップして、ソースを選びます。

最近インストールしたアプリは、アプリの一覧にすぐに表示されない場合があります。 すべてのアプリを表示するには、 **[同期]** をクリックまたはタップします。 この処理には最大で 1 分ほどかかることがあります

![](./media/run-app-browser/dynamics-365-home.png)

## <a name="run-an-app-from-the-task-pane"></a>作業ウィンドウからアプリを実行する
アプリが見つかったら、より簡単にアクセスできるように、そのアプリを作業ウィンドウにピン留めすることができます。 アプリをピン留めするには、アプリ タイルの省略記号 (...) をクリックまたはタップし、 **[Pin this app] /(このアプリをピン留め/)** をクリックまたはタップします。

![](./media/run-app-browser/homepage-pin.png)

ピン留めされたアプリを作業ウィンドウから実行するには、左上隅の **[Dynamics 365]** をクリックまたはタップし、 **[マイ アプリ]** でアプリを探して、それをクリックまたはタップします。

![](./media/run-app-browser/taskpane.png)

## <a name="run-an-app-from-a-url"></a>URL からアプリを実行する
ブラウザーのブックマークとしてアプリの URL を保存し、ブックマークを選んでアプリを実行したり、メールでリンクとして URL を送信したりすることができます。 他のユーザーが作成したアプリをメールで共有されている場合は、メールのリンクをクリックまたはタップして、アプリを実行できます。 URL を使ってアプリを実行するときは、Azure Active Directory の資格情報をってサインインするように求められることがあります。

![](./media/run-app-browser/web-login.png)

## <a name="connect-to-data"></a>データに接続する
アプリでデータ ソースへの接続またはデバイスの機能 (カメラや位置情報サービスなど) を使うためのアクセス許可が必要な場合は、アプリを使う前に同意する必要があります。 通常、これが求められるのは初回のみです。

![Connection](./media/run-app-browser/app-connection.png)

## <a name="close-an-app"></a>アプリを閉じる
アプリを閉じるには、Dynamics 365 ホーム ページからサインアウトするか、別のアプリを開きます。

## <a name="next-steps"></a>次の手順
このトピックでは、Web ブラウザーでキャンバス アプリまたはモデル駆動型アプリを実行する方法について説明しました。 次の方法を学習します。
- モバイルデバイスでキャンバスアプリを実行する方法については、「[モバイルデバイスでキャンバスアプリを実行](run-app-client.md)する」を参照してください。
- モバイルデバイスでモデル駆動型アプリを実行する方法については、「[モバイルデバイスでモデル駆動型アプリを実行](run-app-client-model-driven.md)する」を参照してください。
- モデル駆動型アプリの使用については、「[モデル駆動型アプリの使用](use-model-driven-apps.md)」を参照してください。

