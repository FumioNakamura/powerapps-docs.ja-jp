---
title: フォームのフィールドを追加、移動、または削除 | MicrosoftDocs
ms.custom: ''
ms.date: 04/21/2019
ms.reviewer: ''
ms.service: powerapps
ms.suite: ''
ms.tgt_pltfrm: ''
ms.topic: get-started-article
applies_to:
  - Dynamics 365 (online)
  - Dynamics 365 Version 9.x
  - PowerApps
author: Aneesmsft
ms.author: matp
manager: kvivek
tags:
  - PowerApps maker portal impact
search.audienceType:
  - maker
search.app:
  - PowerApps
  - D365CE
---

# <a name="add-move-or-delete-fields-on-a-form"></a>フォームのフィールドを追加、移動、または削除  
[!INCLUDE [cc-beta-prerelease-disclaimer](../../includes/cc-beta-prerelease-disclaimer.md)]

フォーム デザイナーを使用してフィールドを追加、移動、削除します。

> [!NOTE]
> ドラッグ アンド ドロップを使用してフィールドを追加または移動するときには、フォーム プレビューの反応が敏感で、複数のセクション列を重ねてレンダリングする場合があることに注意してください。 追加または移動するフィールドが正しいセクション列にあることを確認するには、すでにそのセクション列にある別のフィールドに固定されたフィールドにドロップまたは貼り付けます。

## <a name="add-fields-to-a-form"></a>フォームのフィールドを追加
フォームにフィールドを追加するには、**フィールド** ウィンドウを使用します。 **フィールド** ウィンドウを使用すると、検索およびフィルター処理を実行して、フィールドを素早く検索することができます。 また、使用されていないフィールドのみ表示するオプションが含まれています。 

> [!div class="mx-imgBorder"] 
> ![](media/fields-pane.png "フィールド ウィンドウ")

### <a name="add-fields-to-a-form-using-drag-and-drop"></a>ドラッグ アンド ドロップを使用してフォームにフィールドを追加

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. コマンド バーで**フィールドの追加**を選択するか、左のウィンドウで**フィールド**を選択します。  **フィールド** ウィンドウは、既定ではフォーム デザイナーが開くときに開きます。 
3. **フィールド** ウィンドウでは、追加するフィールドを見つけるために、検索、フィルター、またはスクロールします。 フィールドが見つからない場合は、フォーム上に既に存在する可能性があります。 既にフォームに追加されたものを含む、すべてのフィールドが表示するには、**未使用のフィールドのみを表示**をクリアします。 
4. **フィールド** ウィンドウでフィールドを選択し、フォーム プレビューにドラッグします。 フォーム プレビューにフィールドをドラッグすると、フィールドを追加できるドロップ ターゲットが表示されます。 
5. 希望の場所にフィールドをドロップします。 以下に注意します。 
    - フィールドは既存のフィールドの前か後にドロップできます。
    - また、フィールドはセクション内の空の領域でドロップできます。 この場合、新しいフィールドは使用可能なスペースに追加され、フィールドがセクション列全体で等しく配布されます。
    - フィールドをドラッグするときにタブ ヘッダーの上にカーソルを移動すると、現在選択されているタブが変更され、そのフィールドを別のタブに追加できます。   
6. フィールドをさらに追加するには、上の手順 3～5 を繰り返します。
7. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

### <a name="add-fields-to-a-form-using-selection"></a>選択を使用してフォームにフィールドを追加 

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、他の既存のフィールドまたはセクションを選択します。 以下に注意します。
    - 既存のフィールドを選択すると、新しいフィールドは既存のフィールドの後に追加されます。 
    - セクションを選択すると、新しいフィールドは使用可能なスペースに追加され、フィールドがセクション列全体で等しく配布されます。 
3. コマンド バーで**フィールドの追加**を選択するか、左のウィンドウで**フィールド**を選択します。 **フィールド** ウィンドウは、既定ではフォーム デザイナーが開くときに開きます。 
4. **フィールド** ウィンドウでは、追加するフィールドを見つけるために、検索、フィルター、またはスクロールします。 フィールドが見つからない場合は、フォーム上に既に存在する可能性があります。 既にフォームに追加されたものを含む、すべてのフィールドが表示するには、**未使用のフィールドのみを表示**をクリアします。 
5. **フィールド** ウィンドウで、フォームに追加するフィールドを選択します。 または、目的のフィールドの隣の **...** を選択してから、**選択したセクションに追加**を選択します。 
6. フィールドをさらに追加するには、上の手順 2～5 を繰り返します。
7. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

## <a name="move-fields-on-a-form"></a>フォームのフィールドを移動

### <a name="move-fields-on-a-form-using-drag-and-drop"></a>ドラッグ アンド ドロップを使用してフォームのフィールドを移動

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、移動するフィールドを選択し、ドラッグを開始します。 フォーム プレビューにフィールドをドラッグすると、フィールドを移動できるドロップ ターゲットが表示されます。 
3. 希望の場所にフィールドをドロップします。 以下に注意します。 
    - フィールドは既存のフィールドの前か後にドロップできます。
    - また、フィールドはセクション内の空の領域でドロップできます。 この場合、新しいフィールドは使用可能なスペースに追加され、フィールドがセクション列全体で等しく配布されます。
    - フィールドをドラッグするときにタブ ヘッダーの上にカーソルを移動すると、現在選択されているタブが変更され、そのフィールドを別のタブに追加できます。   
4. フィールドをさらに移動するには、上の手順 2～3 を繰り返します。
5. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

    > [!NOTE]
    >   ヘッダーおよびフッターのフィールドの移動におけるドラッグ アンド ドロップの使用は、まだサポートされていません。 

### <a name="move-fields-on-a-form-using-cut-and-paste"></a>切り取りおよび貼り付けを使用してフォームのフィールドを移動

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、移動するフィールドを選択します。
3. コマンド バーで、**切り取り**を選択します。
4. フォーム プレビューで、他の既存のフィールドまたはセクションを選択します。 または、必要に応じて他のタブに切り替えることもできます。
5. コマンド バーで、**貼り付け**またはシェブロンを選択し、その後**前に貼り付け**を選択します。 以下に注意します。
    - **貼り付け**を選択すると、移動中のフィールドは既存のフィールドの後に貼り付けられます。 
    - **前に貼り付け**を選択すると、移動中のフィールドは既存のフィールドの前に貼り付けられます。
    - セクションを選択すると、移動中のフィールドは使用可能なスペースに追加され、フィールドがセクション列全体で等しく配布されます。 **前に貼り付け**操作は適用されないため、この場合は利用できません。
6. フィールドをさらに移動するには、上の手順 2～5 を繰り返します。
7. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

## <a name="delete-fields-on-a-form"></a>フォームのフィールドを削除
1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、フォームから削除するフィールドを選択します。 
3. コマンド バーで、**削除**を選択します。 
4. フィールドをさらに削除するには、上の手順 2～3 を繰り返します。
5. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

     > [!NOTE]
     >   -  フィールドを誤って削除した場合は、コマンド バーで**元に戻す**を選択してフォームを以前の状態に戻します。 
     >   -  必須またはロックされたフィールドは削除することができません。 

### <a name="see-also"></a>関連項目
[モデル駆動型フォーム デザイナーの概要](form-designer-overview.md)  
[フォーム デザイナーを使用してフォームを作成または編集](create-and-edit-forms.md)  
[フォーム デザイナーを使用してフォームのセクションを追加、移動、または削除](add-move-or-delete-sections-on-form.md)  
[フォーム デザイナーを使用してフォームのタブを追加、移動、または削除](add-move-or-delete-tabs-on-form.md)  
[フォーム デザイナーで使用可能なプロパティ](form-designer-properties.md)  
[フォーム デザイナーのツリー ビューを使用](using-tree-view-on-form.md)  
[フィールドの作成および編集](../common-data-service/create-edit-field-portal.md)
