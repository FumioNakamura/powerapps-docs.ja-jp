---
title: キャンバス アプリのアクセシビリティを確認する | Microsoft Docs
description: キャンバス アプリの視覚、聴覚などに障碍があるユーザーへのアクセシビリティを向上させる方法を特定します
author: emcoope-msft
ms.service: powerapps
ms.topic: article
ms.date: 07/05/2018
ms.author: emcoope
search.audienceType:
- maker
search.app:
- PowerApps
ms.openlocfilehash: 05ac3d3705fc56b5714d6cb704d2d3cc3dc87124
ms.sourcegitcommit: b4df7d781cda50dfe2f6609f1cc4d2b531428b3c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "70161295"
---
# <a name="review-a-canvas-app-for-accessibility-in-powerapps"></a>PowerApps でキャンバス アプリのアクセシビリティを確認する

アプリの外観や動作を設計するときにアクセシビリティが考慮されている場合、視覚、聴覚などに障碍があるユーザーは、キャンバス アプリをより簡単に正しく使用できます。 アプリのアクセシビリティを向上させる方法がわからない場合、PowerApps Studio でアクセシビリティ チェックを実行できます。 このツールは可能性があるアクセシビリティの問題を見つけるだけでなく、それぞれが特定の障碍があるユーザーに対して問題になる可能性がある理由を説明し、各問題を解決する方法も提案します。
アクセシビリティ チェックでは、ユーザーのスクリーン リーダーとキーボードの問題を検出し、[アクセシビリティ対応の色](accessible-apps-color.md)を使用することで、色コントラストの問題を修正する方法に関する情報を確認することができます。

アクセシビリティ チェックは、変更が必要な設定の特定に役立ちますが、アプリで実行する必要があることという観点から提案を常に検討する必要があります。 多くの提案が有益である可能性がありますが、有益というよりも悪い結果を増やすと思われる提案はすべて無視することができます。

## <a name="find-accessibility-issues"></a>アクセシビリティの問題を見つける

1. PowerApps Studio の右上隅で、アプリのチェックのアイコンを選択します。

    ![アプリのチェック アイコン](./media/accessibility-checker/app-checker-icon.png)

2. 表示されたメニューで、 **[アクセシビリティ]** を選択します。

    ![アプリのチェック ウィンドウのオプション リスト](./media/accessibility-checker/app-checker-menu.png)

    問題のリストが表示され、最初に深刻度別、次に画面別で並べ替えられます。

    ![アクセシビリティ チェック ウィンドウと項目の一覧](./media/accessibility-checker/accessibility-checker-pane.png)

3. 項目の横にある矢印を選択して、その詳細を表示します。

    ![アクセシビリティ チェックの詳細](./media/accessibility-checker/details-pane.png)

4. 戻る矢印を選択して、項目の一覧に戻ります。

5. 問題に対処する場合は、選択して影響を受けるプロパティを開きます。

6. 1 つまたは複数のプロパティを変更した後、 **[再確認]** を選択して問題の一覧を更新します。

    解決済みの項目は一覧から消えます。新しい項目が表示される場合もあります。

## <a name="severity-of-issues"></a>問題の深刻度

アクセシビリティ チェックでは、問題の深刻度に基づいてエラー、警告、またはヒントとして各問題を分類します。

- **エラー**は、障碍があるユーザーがアプリを使用および理解することを困難にしたり、使用できないようにしたりする問題を特定します。
- **警告**は、ほぼすべての障碍があるユーザーがアプリを使用および理解することを困難にする問題を特定します。
- **ヒント**は、障碍があるユーザーのエクスペリエンス向上に役立ちます。

## <a name="types-of-issues"></a>問題の種類

| 問題のタイトル                            | Severity | 問題の説明  | 修正方法 | 修正理由|
| ------------------------------         |:---------| -----| ------|------ |
| **アクセシビリティのラベルなし**           | Error    | 対話型コントロールにおけるアクセシビリティのラベルのプロパティにテキストが含まれない場合。 対話型コントロールは、ボタンのとおり対話型、または対話型のプロパティを含む可能性があります。 たとえば、画像の **OnSelect** プロパティを設定しているか、その **TabIndex** プロパティを 0 以上に設定している可能性があります。  | アクセシビリティのラベルのプロパティを編集して、項目を説明してください。 | アクセシビリティのラベルのプロパティにテキストがない場合、画面を見ることができないユーザーは、画像やコントロールの内容を理解できません。 |
| **フォーカスが表示されていない**                | Error    | コントロールの **FocusBorderThickness** が 0 に設定されている場合。 明確に表示されるように、フォーカスの境界とコントロール自体の間の色コントラストの比率が適切であることを確認することをお勧めします。 | **FocusedBorderThickness** プロパティを 0 より大きい値に変更します。  | フォーカスが表示されない場合、マウスを使用しないユーザーはアプリと対話するときに、それを見ることができません。   |
| **キャプションが見つかりません**                   | 警告  | **オーディオ**または**ビデオ** コントロールの **ClosedCaptionsURL** プロパティが空の場合。 | **ClosedCaptionsURL** プロパティにキャプション用の URL を設定します。 | キャプションがなければ、障碍のあるユーザーはビデオやオーディオのセグメント内の情報を何も取得できない可能性があります。 |
| **有用なコントロールの設定なし**   | 警告  | いずれかの設定 (グラフのラベルとマーカーの表示、**オーディオ**、**ビデオ**、**ペン入力**コントロールの既定のコントロールの表示など) がオフになっている場合。 | 警告を選択して、プロパティを **true** に設定します。 | このプロパティの設定を変更すると、ユーザーはアプリのコントロールがどのように機能するかについてより詳細な情報を得ることができます。 |
| **HTML がアクセシビリティに対応していない**           | 警告  | HTML テキスト コントロール以外のコントロールに HTML が含まれている場合。 その場合は、PowerApps でカスタムの HTML 要素のアクセシビリティをサポートしません。 | HTML 以外の方式を使用するか、この要素から HTML を削除します。 | 対話型の HTML 要素を追加すると、アプリは正常に動作せず、アクセシビリティに対応しなくなります。 |
| **自動開始をオフにする**                 | 警告  | **オーディオ**または**ビデオ** コントロールの **Autostart** プロパティが **true** に設定されている場合。 | コントロールの **Autostart** プロパティを **false** に設定します。 | ビデオやオーディオ ファイルが自動的に再生されると、ユーザーの気が散る可能性があります。 ユーザーがクリップを再生するかどうかを選択できるようにします。 |
| **画面名を変更する**                 | ヒント      | 画面に既定の名前があると、ユーザーがアプリに移動した場合、スクリーン リーダーによって読み取られます。 | 画面に表示される内容またはその使用目的を説明する名前を画面に指定します。| 視覚に障碍のあるユーザー、弱視のユーザー、失読症のユーザーは、スクリーン リーダーを使用して移動するために、画面名を使用します。 |
| **状態の表示テキストを追加する**          | ヒント      |  コントロールに状態 (切り替えなど) を含むが、値のラベルがオフになっている場合。 | コントロールの **ShowValue** プロパティを **true** に設定して、その現在の状態を表示します。 | コントロールの状態が表示されない場合、ユーザーは自分の操作の確認が得られません。 |
| **画面の項目順序を確認する**| ヒント      | **TabIndex**プロパティが0より大きい場合。 アプリの作成者は、 **TabIndex** プロパティを0より大きい値に設定することにより、カスタムタブの順序を設定できますが、適切に取得して維持し、スクリーンリーダーを中断するのは困難です。 | 可能な場合は、すべての**TabIndex** プロパティを0または-1 に設定します。  **TabIndex**を使用する代わりに、**強化**されたグループコントロールを使用して、ナビゲーション順序を既定値から変更します。  **TabIndex**の値として0より大きい値を使用する必要がある場合は、画面の要素がタブを通過する順序と一致していることを確認してください。 | ナビゲーション順序は、画面に表示されるコントロールの順序 (既定) を反映している必要があります。  手動による調整が行われた場合、特にブラウザーのアドレスバーやアプリ以外のコントロールが存在する場合は、正しい順序を維持することは困難です。  これにより、スクリーンリーダーを使用するのが非常に困難になる可能性があります。  スクリーンリーダーによって読み取られた場合、コントロールは、直感的な順序ではなく、画面上に表示される順序と同じ順序で表示される必要があります。  |
| **別の入力方式の追加**           | ヒント      | アプリに**ペン** コントロールが含まれる場合。 このヒントでは、別の入力方式を含めるように通知されます。 | アクセシビリティのエクスペリエンスのために**ペン** コントロールに加えて、**テキスト入力**を追加します。 | 一部のユーザーはペンを使用できず、情報を指定するために別の方法が必要です (例: 署名の入力)。 |

## <a name="next-steps"></a>次の手順

- [アクセシビリティ対応アプリの作成](accessible-apps.md)
- [アクセシビリティ対応の色](accessible-apps-color.md)
- [アクセシビリティのプロパティ](controls/properties-accessibility.md)
