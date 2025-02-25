# ロール変更リクエストアプリの作成

> **サブスクライバー**

ロール変更リクエストアプリは、従業員がリクエストフォームを送信することから始まります。 次に、現在のマネージャー、受信マネージャー、最後に人事へと処理が進みます。 各ステップで異なるフォームが表示され、オブジェクトはデータを蓄積します。 プロセスの終わりまでに、データオブジェクト全体が完成します。

![ロール変更リクエストオブジェクトは、このワークフロー対応アプリのいくつかのステップを通過します。](./creating-the-role-change-request-object/images/01.png)

先に進む前に、バッキングオブジェクト、フォームビュー、およびテーブルビューを作成します。 詳細は、[ロール変更リクエストオブジェクトの作成](./creating-the-role-change-request-object.md)を参照してください。 ここでは、そこに表示されているバッキングオブジェクトに基づいてワークフロー対応アプリを作成します。

標準アプリは、オブジェクトコントロールパネルエントリ内から作成できますが、ワークフロー対応アプリは作成できません。 代わりに、*Apps*コントロールパネルエントリを使用します。

1.  グローバルメニュー（![Applications Menu](../../images/icon-applications-menu.png)）を開き、[コントロールパネル] → [アプリビルダー] → [Apps]に移動します。

2.  *[ワークフロー対応]* タブをクリックします。 既存のワークフロー対応アプリが表示されます。

3.  追加ボタン（![Add](../../images/icon-add.png)）をクリックして、[新規ワークフロー対応アプリ]キャンバスを開きます。

    ![ワークフロー対応アプリが進行中です。](./creating-a-workflow-powered-application/images/01.png)

4.  ワークフローの最初のステップを実行する準備ができました。名前を「*ロールの変更をリクエスト*」に変更します。 最初のステップは、アプリケーションのプロセスを開始する最初のフォームの送信を表します。 ステップの名前を変更した後、データとビューを設定します。

      - メインデータオブジェクト：*ロール変更リクエスト*オブジェクトを選択します。
      - フォームビュー： *従業員リクエスト*フォームを選択します。
      - テーブルビュー：*ロール変更リクエストマスターリスト*を選択します（このテーブルビューはこのステップでは使用されません）。

    アクションを設定します。

      - 現在のアクションの名前を*マネージャーに送信する*に変更します。

    アプリケーションを保存します。

5.  アプリを再度開き、*プラス*アイコンをクリックしてワークフローにステップを追加します。

    「*レビュー：現在のマネージャー*」という名前を付けて、*管理者*ロールに割り当てます。 ロール変更リクエストアプリに追加する各ステップは、異なるフォームに対応しています。 一緒に、すべてのステップ/フォームからバッキングオブジェクトのすべてのフィールドが入力されます。

    次に、データとビューを設定します。

      - フォームビュー：*現在のマネージャーの評価*。 編集可能にします。

    [ステップ設定]画面に戻り、アクションを設定します。

      - アクションの名前を「*受信マネージャーに転送*」に変更します。

    アプリを保存します。 既存のアプリデータへの更新の適用に関する警告メッセージが表示された場合は、ダイアログボックスで*[保存]* をクリックします。 これは現在データレコードがない新しいアプリであり、警告は情報としてのものです。

6.  アプリを再度開き、追加された最後のステップをクリックし、 *プラス*アイコンをクリックして新しいステップを追加します。

    「*レビュー：受信マネージャー*」という名前を付けて、*管理者*ロールに割り当てます。

    次に、データとビューを設定します。

      - フォームビュー：*潜在的なマネージャーの評価*。 編集可能にします。

    [ステップ設定]画面に戻り、アクションを設定します。

      - 既存のアクションの名前を「*人事に転送*」に変更します。 ワークフローの次のステップに移行します。

      - *現在のマネージャーに送り返す*という名前の2番目のアクションを追加します。 前のワークフローステップに戻り、人事レビューの準備ができるまで2人のマネージャーが詳細について共同作業できるようにします。

7.  アプリを再度開き、追加された最後のステップをクリックし、 プラスアイコンをクリックして新しいステップを追加します。

    「*レビュー：人事*」という名前を付けて、*管理者*ロールに割り当てます。

    次に、データとビューを設定します。

      - フォームビュー：*人事の評価*。 編集可能にします。

    [ステップ設定]画面に戻り、アクションを設定します。

      - アクションの名前は「*送信*」のままにします。

### アプリのデプロイ

これで、アプリを使用する準備が整いました。 ユーザーがデータの送信を開始できるように、[デプロイ](./creating-a-standard-application.md#deploying-the-application)する必要があります。

ロール変更リクエストアプリは、専用リンクを備えたスタンドアロンアプリとしてデプロイできます。 このタイプのアプリを使用するには、事前に[Wiki](../../collaboration-and-social/collaboration-and-social-overview.md#wiki)または会社の従業員ハンドブック[ドキュメント](../../content-authoring-and-management/documents-and-media/publishing-and-sharing/managing-document-access/sharing-documents-with-other-users.md)でいくつかの手順について確認しておく必要があります。 そこにリンクを保持することで、従業員はロール変更リクエストを開始する前に適切なドキュメントを読むことができます。

### アプリの使用

他のワークフローアイテムと同様に、フォームに入力して送信するには、タスクをユーザーに割り当てる必要があります。 これを行う方法は、ワークフロータスクにアクセスする方法によって異なります。

従業員リクエストフォームが送信されると、次のステップに割り当てられたロールは[通知](../../collaboration-and-social/notifications-and-requests/user-guide/managing-notifications-and-requests.md)を受け取ります。 それをクリックすると、次のフォームビュー「レビュー：現在のマネージャー」が表示されます。 変更アイコン（![Change](../../images/icon-change.png)）をクリックして、タスクをユーザーに割り当てます。

![アプリの各フォームには、ユーザー通知を介してアクセスできます。](./creating-a-workflow-powered-application/images/03.png)

または、アプリのテーブルビューからアプリのエントリーのワークフロープロセスを管理することもできます。 アプリのデフォルトビューはテーブルビューであるため、ロール変更リクエストなどのスタンドアロンアプリの場合は、専用リンクを使用してアプリに移動します。 エントリーのアクションボタン（![Actions](../../images/icon-actions.png)）をクリックします。

![アプリの各フォームには、レコードのアクションメニューからアクセスできます。](./creating-the-role-change-request-app/images/04.png)

タスクをユーザーに割り当てるには、*[割り当て先]* メニュー項目を使用します。 その後、*[編集する]* メニューオプションを選択して、適切なフォームにアクセスできます。

```{note}
[マイワークフロータスク](../../process-automation/workflow/user-guide/reviewing-assets.md#assigning-the-review-task)_アプリを使用してワークフロー対応アプリのステップを管理することはできません。
```

### ロール変更リクエストアプリをさらに進化させる

ロール変更リクエストアプリを完全に機能させるための拡張機能を追加します。

1.  マネージャーと人事用の[ロールを作成](../../users-and-permissions/roles-and-permissions/understanding-roles-and-permissions.md)します。 管理者ロールを使用するのではなく、各ロールに適切な手順を割り当てます。

2.  標準アプリを作成して、適切な権限を持つユーザーがロール変更リクエストオブジェクトからマスターリストテーブルを表示できるようにします。 管理者は、最初のフォームである*従業員リクエスト*にアクセスできるので、従業員用のフォームを開始することもできます。

## 関連情報

  - [App Builder Overview](../app-builder.md)
  - [Creating a Standard Application](./creating-a-standard-application.md)
  - [Workflow](../../process-automation/workflow/introduction-to-workflow.md)
  - [ロールと権限](../../users-and-permissions/roles-and-permissions/understanding-roles-and-permissions.md)
