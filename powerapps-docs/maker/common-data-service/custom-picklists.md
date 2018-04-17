---
title: オプション セット作成のクイック スタート | Microsoft Docs
description: このクイック スタートでは、オプション セットを作成します。
services: powerapps
documentationcenter: na
author: clwesene
manager: kfile
editor: ''
tags: ''
ms.service: powerapps
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 3/21/2018
ms.author: clwesene
ms.openlocfilehash: 0e4c106e853b39c71e9cd4b40d4bf94f1c506e2e
ms.sourcegitcommit: 59785e9e82da8f5bd459dcb5da3d5c18064b0899
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2018
---
# <a name="quickstart-create-an-option-set"></a>クイック スタート: オプション セットを作成する

オプション セットを使用すると、アプリ内のドロップダウンに固定値のリスト (他のアプリケーションでは候補リストまたは選択フィールドと呼ばれる場合があります) を含め、データの一貫性を確保することができます。 エンティティと同様に、標準的なオプション セットと、アプリ内で使用するカスタム オプション セットを作成することができます。

オプション セットは、ポータル内でオプション セット リストから作成するか、フィールドの作成中にエンティティ内から直接作成することもできます。 エンティティを作成する方法の詳細については、「[エンティティの作成](data-platform-create-entity.md)」を参照してください。

## <a name="creating-an-option-set-while-adding-a-field"></a>フィールドの追加中にオプション セットを作成します。

1. [powerapps.com](https://web.powerapps.com) で、**[データ]** セクションを展開し、左側のナビゲーション ウィンドウで **[エンティティ]** をクリックまたはタップします。

    ![エンティティの詳細](./media/data-platform-cds-create-entity/entitylist.png "エンティティの一覧")

2. 既存のエンティティまたは [[新しいエンティティを作成する]](data-platform-create-entity.md) を、タップまたはクリックします。

3. **[フィールドの追加]** をクリックして、エンティティに新しいフィールドを追加します。

4. [新しいフィールド] パネルで、フィールドの **[表示名]** を入力します。**[名前]** は自動的に設定され、フィールドの一意名として使われます。 **[表示名]** はユーザーにこのフィールドを表示するときに使われ、**[名前]** はアプリを構築するときや、式や数式で使われます。

    ![新しいフィールド](./media/data-platform-cds-create-entity/newfieldpanel.png "[新しいフィールド] パネル")

5. **[データ型]** ドロップダウンをクリックし、**[オプション セット]** または **[複数選択オプション セット]** を選択します。

6. **[オプション セット]** ドロップダウンを選び、**[新しいオプション セット]** を選択します。

    > [!NOTE]
    > エンティティに既存のオプション セットを使用する場合、新規に作成することがなくこの一覧から選択することができます。

    ![オプション セット一覧](./media/data-platform-cds-newoptionset/fieldpanel-1.png "オプション セット一覧")

7. オプション セットを作成するための新しいパネルが開き、**[表示名]** と **[名前]** には、既定でフィールドの名前が付けられますが、必要な場合に変更することができます。 **[新しい項目の追加]** をクリックして、オプションの一覧の作成を開始します。 すべての項目が作成されるまで、この手順を繰り返します。

    ![新しいオプション セット](./media/data-platform-cds-newoptionset/field-optionsetpanel.png "新しいオプション セット")

8. 項目を入力したら、**[保存]** をクリックして、オプション セットを作成します。

    ![新しいオプション セット](./media/data-platform-cds-newoptionset/field-optionsetpanel-values.png "新しいオプション セット")

9. **[完了]** をクリックしてフィールド パネルを閉じ、**[エンティティの保存]** をクリックして、Common Data Service にエンティティを保存します。

    > [!NOTE]
    > いずれかの項目をこのフィールドの**既定**として選択することができます。この項目はユーザーが、エンティティに新しいレコードを作成するときに既定で選択されます。

    ![新しいフィールド](./media/data-platform-cds-newoptionset/fieldpanel-2.png "[新しいフィールド] パネル")

## <a name="creating-an-option-set-from-the-option-set-list"></a>オプション セット一覧からからオプション セットを作成する

1. [powerapps.com](https://web.powerapps.com) で、**[データ]** セクションを展開し、左側のナビゲーション ウィンドウで **[オプション セット]** をクリックまたはタップします。

    ![オプション セット](./media/data-platform-cds-newoptionset/optionsetlist.png "オプション セット一覧")

2. **[新しいオプション セット]** をクリックします。

3. オプション セットを作成するための新しいパネルが開き、**表示名**と**名前**を入力します。 **[新しい項目の追加]** をクリックして、オプションの一覧の作成を開始します。 すべての項目が作成されるまで、この手順を繰り返します。

    ![オプションのセットの作成](./media/data-platform-cds-newoptionset/optionset-create.png "オプション セットの作成")

4. 項目を入力したら、**[保存]** をクリックして、オプション セットを作成します。

    ![新しいオプション セット](./media/data-platform-cds-newoptionset/optionset-create-values.png "新しいオプション セット")

5. エンティティに新しいフィールドを作成して、このオプション セットを使用できます。

## <a name="global-and-local-option-sets"></a>グローバルおよびローカルのオプション セット

既定では、オプション セットは、複数のエンティティにわたって再利用できるように、グローバル オプション セットとして作成されます。 新しいオプション セットを作成するときに、**[詳細を表示]** オプションで、オプション セットを**ローカル**にすることができます。 このオプションは、オプション セット一覧からではなく、フィールドの追加中にオプション セットを作成するときにのみ使用できます。 ローカルのオプション セットは、作成対象のエンティティとフィールドでのみ使用することができ、他のエンティティで再利用することはできません。 このアプローチはのみ、ローカル オプションに対する特定のニーズがある上級ユーザーにのみ推奨されます。

> [!IMPORTANT]
> ローカルまたはグローバルとしてオプション セットが作成されると、これは変更できません。