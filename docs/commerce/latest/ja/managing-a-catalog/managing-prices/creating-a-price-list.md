# 価格表の作成

価格表は、特定のアカウントとチャネルを対象とするSKU価格エントリを作成および保存するためのエンティティです。 これらのエントリは、商品の単価を決定する際に使用され、対象となる顧客の基本価格表のエントリを上書きまたは修正します。 また、価格表ごとに、 [［価格修飾子］](./using-price-modifiers.md) を定義することもできます。

以下の手順に従って、新しい価格表を作成します：

1. ［**グローバルメニュー**］(![Applications Menu icon](../../images/icon-applications-menu.png))を開き、［**Commerce**］タブをクリックして、［**価格**］ &rarr; ［**価格表**］に移動します。

1. **追加** ボタン（![Add icon](../../images/icon-add.png)）をクリックします。

1. 新しい価格表の ［**名前**］ 、 ［**カタログ**］ 、 そして ［**通貨**］ を入力します。 名前と通貨は作成後いつでも変更できますが、カタログは変更できません。

   ```{note}
      価格表を作成するには、Commerceのインスタンスに少なくとも1つの` [カタログ](../catalogs/creating-a-new-catalog.html) が必要です。
   ```

1. ［**送信**］をクリックします 。

作成したら、 [［商品価格のエントリを追加］](./adding-products-to-a-price-list.md)したり、一般的な設定を行うことができます。 これらの設定には、リストの相対的な重要度、親価格リスト、および価格の種類（つまり、ネットまたはグロス）が含まれます。 また、アカウントとチャネルの適格性を判断し、必要に応じて [［価格修飾子を追加］](./using-price-modifiers.md)することもできます。

完了したら、 ［**公開**］ をクリックして変更を反映させるか、 ［**下書きとして保存**］ をクリックして後から公開することもできます。

```{note}
   カタログを最初に作成すると、各エントリの基本価格を保存するための基本価格表が自動的に作成されます。 これらの価格表では、詳細タブとエントリタブのみを使用できます。 適合性タブと価格修飾子タブは、その後に作成された価格表でのみ使用できます。
```

![新しく作成した価格表の設定をする。](./creating-a-price-list/images/02.png)

<a name="commerce-21-and-below" />

## Commerce 2.1以前

価格表を追加するには：

1. ［**コントロールパネル**］ → ［**コマース**］ → ［**価格表**］に移動します。
1. （![Add icon](../../images/icon-add.png)）ボタンをクリックします。
1. 以下のフィールドに入力します（値の例を次に示します）。
    ***カタログ** ：Sahara.com
    ***名前** ：VIP顧客
    ***店舗通貨** ：USD
    ***重要度** ：1.0
1. ［**アカウントグループ**］下で、［**選択**］をクリックします。
1. この価格表にアクセスする1つ以上のアカウントグループを選択します（アカウントグループの例を以下に示します）。
    ***一般**
    ***自動車修理店**
1. ［**追加**］をクリックします。
1. ［**アカウント**］下で、［**選択**］をクリックします。
1. この価格表にアクセスするアカウントを1つ以上選択します（アカウントの例を以下に示します）。
    * マイクの車の修理
    * ファウンテンバレーの洗車
1. ［**追加**］をクリックします。
1. 価格表のスケジュールを選択します。 （この例では、［**期限を設定しない**］ チェックボックスをオンのままにしておきます。 または、価格表がアクティブになる時期の日付範囲を設定できます。）

    ![価格表を追加する](./creating-a-price-list/images/01.png)

1. ［**公開**］をクリックします。

価格表（この例では **VIP Customers**）が作成され、選択したアカウントグループとアカウントに適用されました。 必要に応じて、手順を繰り返して他の価格表を作成します。

<a name="additional-information" />

## 追加情報

* [新規アカウントの作成](../../users-and-accounts/account-management/creating-a-new-account.md)
* [新規アカウントグループの作成](../../users-and-accounts/account-management/creating-a-new-account-group.md)
* [商品を価格表に追加する](./adding-products-to-a-price-list.md)
* [価格レートを使う](./using-price-tiers.md)
