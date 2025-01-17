---
title: フォーム デザイナーを使用してフォームのタブを追加、移動、または削除 | MicrosoftDocs
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

# <a name="add-move-or-delete-tabs-on-a-form"></a>フォームのタブを追加、移動、または削除  
[!INCLUDE [cc-beta-prerelease-disclaimer](../../includes/cc-beta-prerelease-disclaimer.md)]

フォーム デザイナーを使用してフォームのタブを追加、移動、または削除します。

## <a name="add-tabs-to-a-form"></a>フォームにタブを追加
フォームにタブを追加するには、**レイアウト** ウィンドウを使用します。  

> [!div class="mx-imgBorder"] 
> ![](media/layouts-pane.png "レイアウト ウィンドウ")
   
  > [!NOTE]
  >  タブは、メイン フォームのみに追加できます。 詳細: [フォームの種類](types-forms.md)

### <a name="add-tabs-to-a-form-using-drag-and-drop"></a>ドラッグ アンド ドロップを使用してフォームにタブを追加

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. コマンド バーで**コントロールの追加**を選択するか、左のウィンドウで**レイアウト**を選択します。 
3. **レイアウト** ウィンドウでタブ コントロールを選択し、フォーム プレビューにドラッグします。 フォーム プレビューにタブをドラッグすると、タブを追加できるドロップ ターゲットが表示されます。 
4. 希望の場所にタブをドロップします。 以下に注意します。 
    - タブは、タブ ヘッダーの上にカーソルを移動することにより、既存のタブの前か後にドロップできます。
    - またタブは、現在のタブの左端または右端の上にカーソルを移動することにより、既存のタブの前か後にドロップできます。
5. タブをさらに追加するには、上の手順 3～4 を繰り返します。
6. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

### <a name="add-tabs-to-a-form-using-selection"></a>選択を使用してフォームにタブを追加 

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、他の既存のタブまたはフォームを選択します。 以下に注意します。
    - 既存のタブを選択すると、新しいタブは既存のタブの後に追加されます。 
    - フォームを選択すると、新しいタブはフォームの最後のタブとして追加されます。 
3. コマンド バーで**コントロールの追加**を選択するか、左のウィンドウで**レイアウト**を選択します。  
4. **レイアウト** ウィンドウで、フォームに追加するタブ コントロールを選択します。 または、目的のタブ コントロールの隣の **...** を選択してから、**フォームに追加**を選択します。 
5. タブをさらに追加するには、上の手順 2～4 を繰り返します。
6. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

## <a name="move-tabs-on-a-form"></a>フォームのタブを移動

### <a name="move-tabs-on-a-form-using-drag-and-drop"></a>ドラッグ アンド ドロップを使用してフォームのタブを移動

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、移動するタブのタブ ヘッダーを選択し、ドラッグを開始します。 フォーム プレビューにタブをドラッグすると、タブを移動できるドロップ ターゲットが表示されます。  
3. 希望の場所にタブをドロップします。 以下に注意します。
    - タブは、タブ ヘッダーの上にカーソルを移動することにより、既存のタブの前か後にドロップできます。
    - またタブは、現在のタブの左端または右端の上にカーソルを移動することにより、既存のタブの前か後にドロップできます。
4. タブをさらに移動するには、上の手順 2～3 を繰り返します。
5. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

### <a name="move-tabs-on-a-form-using-cut-and-paste"></a>切り取りおよび貼り付けを使用してフォームのタブを移動

1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、移動するタブを選択します。
3. コマンド バーで、**切り取り**を選択します。
4. フォーム プレビューで、他の既存のタブまたはフォームを選択します。
5. コマンド バーで、**貼り付け**またはシェブロンを選択し、その後**前に貼り付け**を選択します。 以下に注意します。 
    - **貼り付け**を選択すると、移動中のタブは既存のタブの後に貼り付けられます。 
    - **前に貼り付け**を選択すると、移動中のタブは既存のタブの前に貼り付けられます。
    - フォームを選択すると、移動中の新しいタブはフォームの最後のタブとして追加されます。 **前に貼り付け**操作は適用されないため、この場合は利用できません。
6. タブをさらに移動するには、上の手順 2～5 を繰り返します。
7. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

## <a name="delete-tabs-on-a-form"></a>フォームのタブを削除
1. フォーム デザイナーを開いてフォームを作成または編集します。 詳細: [フォームの作成](create-and-edit-forms.md#create-a-form)または[フォームの編集](create-and-edit-forms.md#edit-a-form)
2. フォーム プレビューで、フォームから削除するタブを選択します。 
3. コマンド バーで、**削除**を選択します。
4. タブをさらに削除するには、上の手順 2～3 を繰り返します。
4. コマンド バーで、変更内容を保存してユーザーに対して可視にする場合は、**保存**を選択してフォームを保存または**公開**を選択します。 

    > [!NOTE]
    >   - タブは、メイン フォームのみで削除できます。 詳細: [フォームの種類](types-forms.md)
    >   - タブを誤って削除した場合は、コマンド バーで**元に戻す**を選択してフォームを以前の状態に戻します。 
    >   - 必須またはロック済みフィールドがあるセクションを含むタブは削除できません。 
    >   - ロック済みセクションを持つタブは削除することができません。 
    >   - フォームには少なくとも 1 つのタブが必要です。フォーム上の最後に残っているタブは削除できません。 

### <a name="see-also"></a>関連項目
[モデル駆動型フォーム デザイナーの概要](form-designer-overview.md)  
[フォーム デザイナーを使用してフォームを作成または編集](create-and-edit-forms.md)  
[フォーム デザイナーを使用してフォームのフィールドを追加、移動、または削除](add-move-or-delete-fields-on-form.md)  
[フォーム デザイナーを使用してフォームのセクションを追加、移動、または削除](add-move-or-delete-sections-on-form.md)  
[フォーム デザイナーで使用可能なプロパティ](form-designer-properties.md)  
[フォーム デザイナーのツリー ビューを使用](using-tree-view-on-form.md)  
[フィールドの作成および編集](../common-data-service/create-edit-field-portal.md) 
