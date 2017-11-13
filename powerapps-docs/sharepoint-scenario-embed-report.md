---
title: "SharePoint Online に Power BI のプロジェクト レポートを埋め込む | Microsoft Docs"
description: "このタスクでは、2 つのリストをホストしているのと同じ SharePoint Online サイトに、Power BI のレポートを埋め込みます。"
services: 
suite: powerapps
documentationcenter: na
author: mgblythe
manager: anneta
editor: 
tags: 
ms.service: powerapps
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/12/2017
ms.author: mblythe
ms.openlocfilehash: 6574ad1c67c6fc42da3b1cd5940f163307829333
ms.sourcegitcommit: 43be6a4e08849d522aabb6f767a81c092419babc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/07/2017
---
# <a name="embed-the-power-bi-project-report-in-sharepoint-online"></a>SharePoint Online に Power BI のプロジェクト レポートを埋め込む
**注:** この記事は、SharePoint Online で PowerApps、Microsoft Flow、Power BI を使用するチュートリアル シリーズの一部です。 シリーズ全般に関することや、関連するファイルのダウンロードの詳細については、[シリーズの概要](sharepoint-scenario-intro.md)に関する記事をご覧ください。

このシナリオの最後のタスクでは、2 つのリストをホストしているのと同じ SharePoint Online サイトに、Power BI のレポートを埋め込みます。 Power BI は、さまざまな埋め込み方法をサポートしています。また、Power BI には先般、Web およびモバイルのビューに対応した SharePoint ページへの統合機能が直接追加されました。

このような埋め込み機能により、Power BI は Web パーツとしてレポートを埋め込み、ユーザーが適切にアクセスできるようにします。ユーザーは、埋め込まれたレポートから powerbi.com のレポートまでをクリックできるようになります。最初に、Power BI で埋め込みリンクを生成します。次に、作成したページでそのリンクを使用します。 埋め込みの詳細については、「[SharePoint Online にレポート Web パーツを埋め込む](https://powerbi.microsoft.com/documentation/powerbi-service-embed-report-spo)」 (特に「要件」セクション) をご覧ください。

## <a name="step-1-generate-an-embed-link"></a>手順 1: 埋め込みリンクを生成する
1. Power BI にサインインし、左側のナビゲーション ウィンドウからレポート名をクリックまたはタップします。
   
    ![レポートに移動](./media/sharepoint-scenario-embed-report/08-01-01-reports.png)
2. **[SharePoint Online に埋め込む]** をクリックまたはタップします。
   
    ![SharePoint Online に埋め込む](./media/sharepoint-scenario-embed-report/08-01-02-embed-spo.png)
3. ダイアログ ボックスから埋め込みリンクをファイルにコピーし、**[閉じる]** をクリックします。 このリンクは、SharePoint ページを作成した後で使用します。
   
    ![SharePoint のリンクを埋め込む](./media/sharepoint-scenario-embed-report/08-01-03-embed-url.png)

## <a name="step-2-embed-the-report"></a>手順 2: レポートを埋め込む
1. SharePoint にサインインし、**[サイト コンテンツ]** をクリックまたはタップします。
   
    ![SharePoint サイト コンテンツ](./media/sharepoint-scenario-embed-report/08-01-04-site-contents.png)
2. チームのホーム ページに単にレポートを追加することもできますが、レポート用に別ページを作成する方法についても説明します。 **[新規]**、**[ページ]** の順にクリックまたはタップします。
   
    ![新しい SharePoint ページ](./media/sharepoint-scenario-embed-report/08-01-05-new-page.png)
3. ページの名前を入力します (例: “プロジェクトの分析”)。
4. ![プラス アイコン](./media/sharepoint-scenario-embed-report/icon-plus.png)、**[Power BI]** の順にクリックまたはタップします。
   
    ![Power BI ページのパーツの追加](./media/sharepoint-scenario-embed-report/08-01-06-add-page-part.png)
5. **[レポートの追加]** をクリックまたはタップします。
   
    ![レポートの追加](./media/sharepoint-scenario-embed-report/08-01-07-add-report.png)
6. 右側のウィンドウで、埋め込み URLを **[Power BI report link]\(Power BI のレポート リンク\)** ボックスにコピーします。 **[Show Filter Pane]\(フィルター ウィンドウの表示\)** と **[ナビゲーション ウィンドウの表示]** の両方を **[オン]** に設定します。
   
    ![レポートの設定](./media/sharepoint-scenario-embed-report/08-01-08-report-settings.png)
7. レポートがページに埋め込まれました。 **[発行]** をクリックすると、基になるレポートにアクセスできるユーザーが、レポートを利用できるようになります。
   
    ![レポートの埋め込みの完了](./media/sharepoint-scenario-embed-report/08-01-09-report-complete.png)

## <a name="step-3-grant-access-to-the-report"></a>手順 3: レポートへのアクセスを許可する
Office 365 グループを使用している場合 (推奨)、アクセスを必要とするユーザーが Power BI サービス内のグループ ワークスペースのメンバーであることを確認してください。 これにより、ユーザーはそのグループのコンテンツを表示できるようになります。 詳細については、[Power BI でのグループの作成](https://powerbi.microsoft.com/documentation/powerbi-service-create-a-group-in-power-bi)に関するページをご覧ください。

今回のシナリオでの Power BI での作業は以上です。 SharePoint リストから Power BI にデータを抽出することから開始し、Power BI レポートを SharePoint に戻して埋め込む作業までを行いました。

## <a name="next-steps"></a>次の手順
このチュートリアル シリーズの次の手順では、[作成したワークフローを最初から最後まで一通り実行します](sharepoint-scenario-summary.md)。
