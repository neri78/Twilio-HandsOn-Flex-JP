#  手順1: キューを作成する

この手順ではTwilioコンソールに用意されているTaskRouter画面に遷移し、Flex用にセールス、サポートそれぞれのキューを作成します。

## TaskRouterを表示

[TaskRouter](https://www.twilio.com/console/taskrouter)コンソールを開くと、`Flex Task Assignment`ワークスペースが定義されていることを確認できます。このワークスペースをクリックします。

![Flex Admin Console](../assets/04-Console-TaskRouter.png)

Workspaceではキューの一覧が表示されます。標準ではすべての担当者が属する`Everyone`が表示されています。
![Flex TaskQueues](../assets/04-TaskQueues.png)

この画面で`View all Task Queues`リンクをクリックします。

遷移先の画面で`+`ボタンをクリックしサポートキューを作成します。
下記のテーブルの設定値を参考にしてください。

|設定値|値|
|:----|:----|
|Task Queue Name| support |
|Reservation Activity| Offline |
|Assignment Activity| Offline |
|Target Worker expression| routing.skills HAS \"support\"|

保存後、作成したsupportキューを開きます。この際、`Target Worker expression`が正しく設定されていれば、`Matching Workers`に管理者エージェントが表示されます。

![support queue](../assets/04-Support-Queue.png)

`Save`ボタンをクリックし保存します。

同じように `sales`キューを作成します。

|設定値|値|
|:----|:----|
|TASKQUEUE NAME| sales |
|Reservation Activity| Offline |
|Assignment Activity| Offline |
|Target Worker expression| routing.skills HAS "sales"|

これでサポート、営業向けキューが追加されました。

## 次のハンズオン

- [ハンズオン: タスクルーティング - タスクフローを設定](../05-Task-Routing-Workflow/00-Overview.md)
