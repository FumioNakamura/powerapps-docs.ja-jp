---
title: SharePoint Online に Power BI のプロジェクト レポートを埋め込む | Microsoft Docs
description: このタスクでは、2 つのリストをホストしているのと同じ SharePoint Online サイトに、Power BI のレポートを埋め込みます。
author: NickWaggoner
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: canvas
ms.reviewer: ''
ms.date: 01/30/2018
ms.author: niwaggon
search.audienceType:
- maker
search.app:
- PowerApps
ms.openlocfilehash: 92ae77237064d28e3070f7e7bc9cb94c4493a3c6
ms.sourcegitcommit: 4ed29d83e90a2ecbb2f5e9ec5578e47a293a55ab
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "63321244"
---
# <a name="embed-the-power-bi-project-report-in-sharepoint-online"></a>SharePoint Online に Power BI のプロジェクト レポートを埋め込む
> [!NOTE]
> この記事は、SharePoint Online で PowerApps、Microsoft Flow、Power BI を使用するチュートリアル シリーズの一部です。 シリーズ全般に関することや、関連するファイルのダウンロードの詳細については、[シリーズの概要](sharepoint-scenario-intro.md)に関する記事をご覧ください。

今から 2 つのリストをホストしているのと同じ SharePoint Online サイトに、Power BI のレポートを埋め込みます。 Power BI は、Web およびモバイル表示の SharePoint ページへの直接統合を含む、さまざまな埋め込み方法をサポートしています。

このような埋め込み機能により、Power BI は Web パーツとしてレポートを埋め込み、ユーザーが適切にアクセスできるようにします。ユーザーは、埋め込まれたレポートから powerbi.com のレポートまでをクリックできるようになります。 最初に、Power BI で埋め込みリンクを生成します。次に、作成したページでそのリンクを使用します。 埋め込みの詳細については、「[SharePoint Online にレポート Web パーツを埋め込む](https://docs.microsoft.com/power-bi/service-embed-report-spo)」をご覧ください。

## <a name="step-1-generate-an-embed-link"></a>手順 1:埋め込みリンクを生成します。
1. Power BI にサインインし、左側のナビゲーション ウィンドウからレポート名をクリックまたはタップします。
   
    ![レポートに移動](./media/sharepoint-scenario-embed-report/08-01-01-reports.png)
2. **[ファイル]**、**[SharePoint Online に埋め込む]** の順にクリックまたはタップします。
   
    ![SharePoint Online に埋め込む](./media/sharepoint-scenario-embed-report/08-01-02-embed-spo.png)
3. ダイアログ ボックスから埋め込みリンクをファイルにコピーし、**[閉じる]** をクリックまたはタップします。 このリンクは、SharePoint ページを作成した後で使用します。
   
    ![SharePoint のリンクを埋め込む](./media/sharepoint-scenario-embed-report/08-01-03-embed-url.png)

## <a name="step-2-embed-the-report"></a>手順 2:レポートを埋め込む
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

## <a name="step-3-grant-access-to-the-report"></a>手順 3:レポートへのアクセスを許可します。
Office 365 グループを使用している場合 (推奨)、アクセスを必要とするユーザーが Power BI サービス内のグループ ワークスペースのメンバーであることを確認してください。 これにより、ユーザーはそのグループのコンテンツを表示できるようになります。 詳細については、「[Power BI アプリ ワークスペースでの共同作業](https://docs.microsoft.com/power-bi/service-collaborate-power-bi-workspace)」を参照してください。

今回のシナリオでの Power BI での作業は以上です。 SharePoint リストから Power BI にデータを抽出することから開始し、Power BI レポートを SharePoint に戻して埋め込む作業までを行いました。

## <a name="next-steps"></a>次の手順
このチュートリアル シリーズの次の手順では、[作成したワークフローを最初から最後まで一通り実行します](sharepoint-scenario-summary.md)。

