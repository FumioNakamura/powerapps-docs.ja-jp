---
title: "ルックアップ フィールド経由でのエンティティのリレーションシップ | Microsoft Docs"
description: "ルックアップ フィールドを使用してエンティティ間のリレーションシップを構築します。"
services: powerapps
documentationcenter: na
author: kfend
manager: kfend
editor: 
tags: 
ms.service: powerapps
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 12/09/2016
ms.author: kfend
ms.openlocfilehash: 1aff4df6e314f50a67aff6a08298d3d7aa4a9cfa
ms.sourcegitcommit: 43be6a4e08849d522aabb6f767a81c092419babc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/07/2017
---
# <a name="build-a-relationship-between-entities"></a>エンティティ間のリレーションシップを構築する
エンティティのデータに、別のエンティティのデータとの関連性があることは少なくありません。 たとえば、**Customers** エンティティと **Orders** エンティティがある場合、**Orders** エンティティは、どの顧客からの発注であるかを示す **Customers** エンティティに対するルックアップ リレーションシップを持つことが考えられます。 ルックアップ フィールドを使用すれば、発注した顧客の **Customers** エンティティからのデータを表示することができます。 詳細については、「[Entity relationships and lookup fields](https://docs.microsoft.com/en-us/common-data-service/entity-reference/relationships)」 (エンティティ リレーションシップとルックアップ フィールド) を参照してください。

## <a name="define-a-relationship"></a>リレーションシップの定義
2 つのエンティティ間 (または同じエンティティ間) で作成できるリレーションシップには、いくつかの種類があります。 1 つのエンティティは、複数のエンティティとのリレーションシップを持つことができます。また、1 つのエンティティが、別のエンティティに対して複数のリレーションシップを持つこともできます。 以下に、いくつかの一般的なリレーションシップの種類を示します。

* **標準** - このタイプのリレーションシップは、2 つのエンティティの間に存在します。
* **自己** - このタイプのリレーションシップは、同じエンティティ間に存在します。
* **一対一** - このタイプのリレーションシップでは、エンティティ A の各レコードが、エンティティ B の 1 件のレコードとのみ対応関係を持つことができます (その逆も同様)。 現行リリースの Common Data Service は、カスタム エンティティのこのタイプのリレーションシップをサポートしていません。
* **一対多** - このタイプのリレーションシップでは、エンティティ A の各レコードが、エンティティ B の複数のレコードと対応関係を持つことができます。一方、エンティティ B の各レコードは、エンティティ A の 1 件のレコードに対してしか対応関係を持つことができません。
* **多対多** - このタイプのリレーションシップでは、エンティティ A の各レコードが、エンティティ B の複数のレコードと対応関係を持つことができます (その逆も同様)。 現行リリースの Common Data Service は、このタイプのリレーションシップをサポートしていません。

## <a name="add-a-lookup-relation"></a>ルックアップ リレーションシップの追加
エンティティにルックアップ リレーションシップを追加するには、**[リレーションシップ]** タブでリレーションシップを作成し、リレーションシップを作成するエンティティを指定します。

1. [powerapps.com](https://web.powerapps.com) で、**[Common Data Service]** セクションを展開し、左側のナビゲーション ウィンドウで **[エンティティ]** をクリックまたはタップします。
2. エンティティの一覧で、目的のエンティティをクリックまたはタップすると、そのフィールドが表示されます。 この一覧は、その上に表示される検索バーに文字を入力してフィルタリングできます。
3. 画面の上部に表示される **[リレーションシップ]** をクリックまたはタップします。 このタブには、エンティティのすべてのリレーションシップが表示されます。 **[新しいリレーションシップ]** をクリックします。
4. **[リレーションシップの作成]** ページで、リレーションシップを作成する関連エンティティを指定します。次に、リレーションシップの名前と表示名を指定します。
5. **[保存]** をクリックまたはタップして変更を確定します。 同じ名前のルックアップ フィールドが自動的に作成されます。

## <a name="use-a-lookup-field-in-an-app"></a>アプリでのルックアップ フィールドの使用
ルックアップ フィールドを含むエンティティから[自動的にアプリを作成](data-platform-create-app.md)した場合、そのエンティティは**ドロップダウン** コントロールとして表示され、折りたたまれた状態にある参照先エンティティの**プライマリ キー** フィールドからのデータを含みます。 展開時にドロップダウンで 2 つのフィールドを表示するには、ルックアップ リレーションシップの関連エンティティの **[Default Lookup]** (既定のルックアップ) フィールド グループに PrimaryId フィールドと任意の 2 番目のフィールドを追加する必要があります。

## <a name="delete-a-record-with-a-lookup-relation"></a>ルックアップ リレーションシップを持つレコードの削除
エンティティ A がエンティティ B に対するルックアップ リレーションシップを持つ場合、次のことが当てはまります。

* エンティティ A のレコードは自由に削除することができます。
* エンティティ A のレコードとの対応関係を持つレコードがエンティティ B に存在する場合、エンティティ B のレコードを削除するためにはまず、エンティティ A の、対応するすべてのレコードを削除する必要があります。

**注**: エンティティ B が標準エンティティで、エンティティ A に対する親リレーションシップを持つ場合、エンティティ A からレコードを削除すると、エンティティ B からも、対応するすべてのレコードが削除されます。

フィールドを削除する方法については、[フィールドの管理](data-platform-manage-fields.md)に関するページを参照してください。

## <a name="next-steps"></a>次の手順
* [Common Data Service データベースを使用してアプリを生成する](data-platform-create-app.md)
* [Common Data Service データベースを使用してアプリを最初から作成する](data-platform-create-app-scratch.md)
