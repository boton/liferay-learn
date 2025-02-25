# 測定単位

Liferay Commerceには、多くの共通の測定単位が既に定義されていますが、ユーザーまたは配送業者が異なる単位を使用している場合は、デフォルト設定を変更する必要があります。

Liferay Commerceには、寸法と重量の2つの測定単位が定義されています。 測定単位ごとに、基本単位を指定する必要があります。 Liferay Commerceでは、 **基本単位** によって、ストアで使用される測定システムと、カタログに表示されるデフォルトの測定値が決まります。 デフォルトでは、寸法と重量の基本単位はそれぞれインチとポンドです。 基本単位として設定されている単位が、カタログおよび変動レートの配送方法で使用されます。

<a name="adding-a-new-measurement-unit" />

## 新しい測定単位の追加

場合によって、新しい測定単位を追加する必要があります。 たとえば、センチメートルは、 ［**寸法**］ ページにデフォルトの測定単位としてリストされていません。 同様に、出荷される商品が、キログラムではなくメートルトン（トン）などのより大きな増分で測定される場合があります。

新しい寸法測定単位（センチメートルなど）を入力するには：

1. ［**コントロールパネル**］ → ［**コマース**］ → ［**設定**］ に移動します。
1. ［**計量単位**］ をクリックします。
1. （+）ボタンをクリックして、新しい寸法を追加します。
1. 次のように入力します：
    ***Name** ：センチメートル
    ***Key** ：cm
    ***Primary** ： **No**
    ***Ratio to inches** ：2.54
    ***Priority** ：4.0

    ![測定単位の追加](./measurement-units/images/01.png)

1. ［**保存**］ をクリックします。

**センチメートル** が寸法のリストに追加されました。

**注** ：キーは［Name］フィールドに基づいて生成されますが、代わりに **cm** などの測定単位で使用できる省略表現に置き換えることをお勧めします。

<a name="additional-information" />

## 追加情報

運送業者の配送方法を使用して、配送料の計算を配送業者のシステムと統合する場合は、業者の単位も定義する必要があります。 業者が基本単位とは異なる単位を使用している場合、変換は自動的に処理されます。
