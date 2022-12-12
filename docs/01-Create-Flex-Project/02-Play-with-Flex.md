#  手順2: Flexを試してみる

この手順ではこれから設定するFlexの使用方法を学びます。

## ステータスをオンラインに変更

Flex画面の右上に表示されている自分自身のステータスを`Available`に変更します。

![Flex - Status](../assets/01-Flex-Status.jpg)

## 電話番号を確認

Flexを初期化した際に着信を受け付ける番号として米国番号が自動的に割り当てられます。今回のハンズオンではこの番号に電話をかけて動作を確認します。そのため、番号を控えてください。この番号は[`Phone Numbers`](https://www.twilio.com/console/phone-numbers/incoming)コンソールから設定を変更できます。


![Flex - US number](../assets/01-Flex-Admin-Number.png)


この番号に電話をかけるとFlexの担当者に接続することができます。

トライアルアカウントを利用している場合は最初にトライアルである旨のメッセージが流れます。このメッセージはスキップできません。

> You have a trial account. You can remove this message at anytime by upgrading to full account. Press any to execute your code.


メッセージを最後まで聞いたあとに数字キーを押すと、`Agent Desktop`に着信番号を持つタスクが1つ増えます。

![Flex - incoming calls](../assets/01-Incoming-Call.png)


このタスクをクリックするとブラウザーと電話がつながります。

通話を終えたのち、`Complete`ボタンをクリックするとタスクが消えます。

![Flex - agent - complete call](../assets/01-Task-complete.png)

Flexは標準で`音声`、`SMS`、`Webチャット`の3つに対応します。音声とSMSは携帯電話の通話料、メッセージ送信料金がかかります。

次のハンズオンでは音声問い合わせのフローをカスタマイズします。

## 次のハンズオン

- [ハンズオン: 問い合わせフローをカスタマイズ](../02-Customize-Flow/00-Overview.md)