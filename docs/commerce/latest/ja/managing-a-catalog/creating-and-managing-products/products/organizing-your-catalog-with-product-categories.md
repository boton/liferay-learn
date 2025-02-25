# 商品カテゴリを使用してカタログを整理する

商品はカテゴリに分類できます。 これらのグループ化により、複数の商品をグループ化し、一括して扱うことができます。 商品カテゴリを使用して、商品のセットに割引やその他のオファーを適用したり、購入者が商品を見つけやすくしたり、特定の商品を特定のアカウントまたはアカウントグループにプロモートしたりできます。

カテゴリを階層的に編成して、カテゴリの分類を形成することもできます。 商品をカテゴリに整理するには、最初にカテゴリを作成してから商品を割り当てる必要があります。 さらに、すべてのLiferay Commerce商品はグローバルレベルで処理されるため、すべてのボキャブラリとカテゴリはグローバルスコープレベルである必要があります。

グローバルスコープとサイト管理の詳細は、この記事で [データ範囲](https://help.liferay.com/hc/articles/360018168991-Data-Scopes) および [設定範囲](https://help.liferay.com/hc/articles/360017895452-Introduction-to-Setting-Up#configuration-scope) について参照してください。

<a name="prerequisites" />

## 前提条件

カタログを整理する前に、カテゴリを入力する必要があります。 [新しい商品カテゴリ](./creating-a-new-product-category.md) 作成の記事を参照してください。

```{note}
Miniumなどのアクセラレータを使用してサンプルデータでサイトを作成した場合、VocabularyとCategoriesはGlobalスコープに入力されます。 これは、すべてのサンプルカテゴリがすべてのサイトで利用できることを意味します。
```

<a name="managing-product-categories" />

## 商品カテゴリを管理

ボキャブラリとカテゴリを使用して分類を作成したら、カタログ内の商品にカテゴリを追加できます。

1. ［**グローバルアプリケーション**］メニュー &rarr; ［**Commerce**］&rarr; ［**商品**］に移動します。
1. 商品をクリックします。 （Miniumを使用してサンプルデータを含むサイトを作成した場合は、［**Transmission Fluid**］をクリックします。 **Transmission Fluid** 商品はすでにサンプルのボキャブラリとカテゴリにリンクされています。）

    ![Commerce 2.1でのカテゴリの関連付け](./organizing-your-catalog-with-product-categories/images/01.png)

1. ［**詳細**］タブで、［**カテゴリ** ウィジェットのカタログの横にある［**選択**］をクリックします。
1. 適切なボキャブラリのラベルの下にある［**Select**］ボタンをクリックし、表示されるポップアップで、該当する各カテゴリの横にあるチェックボックスをオンにします。

    ![カテゴリーの選択](./organizing-your-catalog-with-product-categories/images/02.png)

1. ［**完了**］ をクリックします。

<a name="commerce-21-and-below" />

## Commerce 2.1以前

1. ［**コントロールパネル**］ → ［**コマース**］ → ［**商品**］に移動します。
1. 商品をクリックします。 （Miniumを使用してサンプルデータを含むサイトを作成した場合は、［**Transmission Fluid**］をクリックします。 **Transmission Fluid** 商品はすでにサンプルのボキャブラリとカテゴリにリンクされています。）

    ![Commerce 2.1でのカテゴリの関連付け](./organizing-your-catalog-with-product-categories/images/01.png)

1. ［**詳細**］タブで、［**カテゴリ** ウィジェットのカタログの横にある［**選択**］をクリックします。
1. 適切なボキャブラリのラベルの下にある［**Select**］ボタンをクリックし、表示されるポップアップで、該当する各カテゴリの横にあるチェックボックスをオンにします。

    ![カテゴリーの選択](./organizing-your-catalog-with-product-categories/images/02.png)

1. ［**完了**］ をクリックします。

### Commerce 2.0以前

1. ［**コントロールパネル**］ → ［**コマース**］ → ［**商品**］に移動します。
1. 商品をクリックしてから、［**カテゴリー設定**］タブをクリックします。 （Miniumを使用してサンプルデータを含むサイトを作成した場合は、［**Transmission Fluid**］をクリックします。 **Transmission Fluid** 商品はすでにサンプルのボキャブラリとカテゴリにリンクされています。）

    ![カテゴリを管理](./organizing-your-catalog-with-product-categories/images/03.png)

1. 適切なボキャブラリのラベルの下にある［**Select**］ボタンをクリックし、表示されるポップアップで、該当する各カテゴリの横にあるチェックボックスをオンにします。
1. ［**完了**］ をクリックします。

これで、カテゴリが商品に関連付けられました。

![カテゴリを選択](./organizing-your-catalog-with-product-categories/images/04.png)

このカテゴリに該当する可能性のある他のすべての商品について、必要に応じて繰り返します。

<a name="additional-information" />

## 追加情報

* [新しい商品カテゴリの作成](./creating-a-new-product-category.md)
