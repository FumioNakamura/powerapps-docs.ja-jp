---
title: プレビュー機能と試験的な機能を理解する | Microsoft Docs
description: 新機能をテストして導入を開始します。
author: gregli-msft
manager: kvivek
ms.service: powerapps
ms.topic: conceptual
ms.custom: canvas
ms.reviewer: anneta
ms.date: 07/16/2018
ms.author: gregli
ms.openlocfilehash: d976a81603d48d72ecb2dc7c279b59d0e70800eb
ms.sourcegitcommit: b9fa569153924af9815db45d52c04e764ddb7fa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2018
ms.locfileid: "39094833"
---
# <a name="understand-experimental-and-preview-features-in-powerapps"></a>PowerApps の試験的な機能とプレビュー機能を理解する

すべてのリリースで、PowerApps がユーザーのニーズに最適なツールになるように変更を加えたり、機能を追加したりしています。 製品を上位に進めます。  

Microsoft は下位互換性を重要視しています。 しかし、どのような変更や改善でも、意図しない副作用が導入されてしまう可能性があり、ご利用のアプリが以前とまったく同じようには動作しないこともあります。

既存のアプリ上の影響に対するバランスの改善に役立てるために、ステージを進めて機能の規模を大きくします。 この記事では、このプロセス、およびデプロイされている機能へのエクスポージャを制御する方法について説明します。

## <a name="feature-roll-out-stages"></a>機能のロールアウト ステージ

機能は、製品の公式の部分になるために 3 つのステージを移動します。

1. **試験的**: この機能は準備段階です。 まだこの機能に依存しないでください。大幅な変更が加えられる可能性があります。
1. **プレビュー**: この機能はほぼ完了しており、安定しています。 現在、既存のアプリの移行を開始しています。
1. **出荷済み**: この機能は完成しています。 すべてのアプリでこの機能が有効になっており、オフにすることはできません。

各ステージで、その機能がお客様に必要な内容であり、意図しない副作用を導入しないということの検証にご協力いただくと、機能を使用するユーザーの数が上昇します。

**このプロセスには、お客様のフィードバックが不可欠です。**  [PowerApps コミュニティ フォーラム](https://powerusers.microsoft.com/t5/PowerApps-Community/ct-p/PowerApps1)からフィードバックを投稿してください。

機能が各ステージにとどまる期間は、 機能によって異なります。 Microsoft では、機能を使用するアプリの数、報告された問題の数、機能の必要性に関する緊急度など、多くの要因を確認します。 機能が 1 つのステージにとどまる期間は数週間のことも数か月のこともあります。

この表は、参加する必要があるタイミングを決定するのに役立つ場合があります。 

| ステージ | いつ使用すればよいですか? | 自信を持って使用できますか? | 新しいアプリに対して既定で有効にされていますか? | 
|----|----|----|-----|------|
| **試験的** | 初期採用者の場合、役立つものが表示されたら、機能のテストに協力します。 | いいえ。  試験的な機能は大幅に変更されたり、いつでもまったく表示されなくなったりする可能性があります。 | いいえ。 この機能を明示的に利用する必要があります。  |  
| **プレビュー** | 新しいアプリには自動的にこの機能が含まれます。  この機能は最終的に既存のアプリでもオンにされるため、既存のアプリで有効にしてテストを開始します。 | はい。 この機能は順調で、製品の一部として恒久的に保存されます。  | はい。 問題が発生した場合は、オフにする必要がある可能性があります。  問題を報告してください。これが機能がプレビューされている主な理由です。 | 
| **出荷済み** (**[詳細設定]** に表示されなくなります) | すべてのアプリにこの機能があります。 | はい。 | はい。  ほとんどの場合、無効にすることができません。  |  

プレビューの終盤に、Microsoft ではすべてのアプリに対して 1 回で機能を有効にする可能性があり、**最終検証**としてマークします。  この変更では、ほとんどのユーザーに機能を試す最後のチャンスが提供されますが、まだオフにすることができます。 次のステージでは、機能は完全に出荷され、オフにできないため、この期間はタイムリーなフィードバックが重要です。  

## <a name="documentation"></a>ドキュメント

これらの機能に関する情報を確認できる場所  Microsoft はプレビュー機能を完了した機能として扱うので、他の製品の機能を実行するように、それらの機能について詳しく確認することができます。 
- [PowerApps の概要](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/getting-started)。 新機能の基本 (利点、作業を開始する方法、参照情報) を提供します。
- [PowerApps コミュニティ フォーラム](https://powerusers.microsoft.com/t5/PowerApps-Community/ct-p/PowerApps1)。  他のユーザーがお客様と共に新機能を調べます。 他のユーザーの体験から学んで、自分の体験を共有しましょう。
- [PowerApps ブログ](https://powerapps.microsoft.com/en-us/blog/)。  常にではありませんが、ブログの投稿には新機能を伴うことが多いです。

試験的な機能は異なります。  これらの機能は作業中であり、完了したとは見なしていません。 **[アプリの設定]** ウィンドウ (以下を参照) にある簡単な説明は、それらに関する情報のみである可能性があります。 通常、試験的な機能は、ドキュメントには表示されません。 コミュニティ フォーラムは、情報における最適なソースである可能性が高いです。  場合によっては、初期のブログの投稿で機能について説明されています。  十分な情報が見つからない場合は、フォーラムで質問するか、この機能がプレビュー ステージに移るまで待ちます。

## <a name="controlling-which-features-are-enabled"></a>有効にする機能を制御する

試験的な機能とプレビュー機能は、アプリの **[詳細設定]** に一覧表示されます。  アプリ内から **[ファイル]** メニュー、**[アプリの設定]**、**[詳細設定]** の順に選択します。 **[プレビュー機能]** と **[試験的な機能]** セクションまで下にスクロールします。

![](media/working-with-experimental/advanced-settings.png)

各機能にトグル スイッチがあります。  **[オフ]** はこの機能が無効であることを意味します。  すべてのスイッチがオフの状態が、アプリを実行する基準で最も安全な方法です。

場合によっては、設定を変更した後、アプリを閉じてもう一度開く必要がある可能性があります。  機能の説明では、この手順を行う必要があるタイミングを示します。

**[詳細設定]** パネルの上部で、プレビューまたは試験的ではない、完全に依存できる、全出荷完了の機能に対する設定を確認することができます。 

これらの設定は各アプリに固有のため、トグル スイッチの変更は現在開かれているアプリにのみ影響します。 アプリを作成すると、これらのスイッチはそのアプリの既定の設定に戻ります。