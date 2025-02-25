# 商品表示ページの作成

Liferay Commerceを使用すると、ストア商品を個別のサイトページに紐付けて、商品ごとに専用の表示ページを作成できます。 既成のウィジェットやカスタムウィジェット、フラグメントを使用して、レイアウトを短時間でデザインし、商品の詳細を表示できます。

以下の手順で、商品の表示ページを設定します。

1. ストアで新しいサイトページを作成し、 **商品詳細** ウィジェットを他の必要なページ要素と一緒に追加します。 詳細は、 [コンテンツページの構築](https://learn.liferay.com/dxp/latest/ja/site-building/creating-pages/building_and_managing_content_pages.html) を参照してください。 このページで、リンクされた商品を表示する際のレイアウトを決定します。

1. ［**グローバルメニュー**］(![Global Menu](../images/icon-applications-menu.png))を開き、［**Commerce**］タブをクリックし、 ［**Store Management**］ &rarr;［**Channels**］へ移動する。

1. 必要な ［**チャネル**］を選択し、 ［**商品表示ページ**］ タブをクリックし、 ［**追加**］ ボタン（![Add Button](../images/icon-add.png)）をクリックします。

   ![商品表示ページタブで［追加］をクリックします。](./creating-product-display-pages/images/02.png)

1. ［**商品を選択**］をクリックし、新規タイトルのページにリンクさせたい商品を **選択** します。

1. ［**商品表示ページ**］の［**Choose**］をクリックし、新規タイトルのページを選択し、［**完了**］をクリックします。

   ![新しいページを選択します。](./creating-product-display-pages/images/03.png)

1. 完了したら、 ［**保存**］ をクリックします。

これにより、商品と選択したページが即座に関連付けられます。 これで、ユーザーがストアで商品をクリックすると、商品の表示ページにリダイレクトされるようになります。

保存済みのすべての設定は、商品表示ページタブで確認・管理できます。

![保存済みのすべての設定は、商品表示ページタブで確認・管理できます。](./creating-product-display-pages/images/04.png)

```note::
   商品詳細やカテゴリーコンテンツのウィジェットが配置されたレイアウトが2つある場合、Liferayはレイアウトリストに記載された最初のレイアウトをデフォルトとします。
```

<a name="additional-information" />

## 追加情報

* [ストアフロントの作成](./creating-your-storefront.md)
* [カタログページの作成](./creating-a-catalog-page.md)
