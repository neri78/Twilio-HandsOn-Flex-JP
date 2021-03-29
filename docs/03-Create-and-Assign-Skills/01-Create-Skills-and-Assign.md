#  手順1: スキルの作成と担当者への設定

この手順ではFlex管理者コンソールでスキルを作成し、担当者にスキルを設定する方法を学習します。

## スキルを作成

Flex管理者コンソールを開き、`SKILLS`ボタンをクリックします。

![Flex Admin Console](../assets/03-Flex-Admin-Console.png)

`NAME OF SKILL`ボックスに`sales`と名前を入力し、`ADD NEW SKILL`ボタンをクリックします。

![Flex add skill](../assets/03-Add-Skill.png)

続けて同じように`support`スキルを作成します。2つのスキルが作成されていることを確認してください。

![Flex skills](../assets/03-Flex-skills.png)

それぞれのスキルについて作成された`QUEUE EXPRESSIONS`と`WORKFLOW EXPRESSIONS`を控えておきます。

|LABEL|QUEUE EXPRESSIONS|WORKFLOW EXPRESSIONS|
|:----|:----|:-----|
|sales| routing.skills HAS "sales" | "sales" IN task.skillsNeeded |
|support| routing.skills HAS "support"| "support" IN task.skillsNeeded|

## スキルを担当者に設定

エージェント画面を表示し、フィルタリングを`All Agents`に設定します。

![Flex - agents](../assets/03-Agents.png)

表示されたエージェントを選択し、`support`スキルを追加します。`Save`ボタンを忘れないようにしましょう。スクリーンショットを参考にしてください。

![Flex - add skill to agent](../assets/03-Add-Skills.png)

これでサポートスキルが管理者エージェントに追加されました。

## 次のハンズオン

- [ハンズオン: タスクルーティング - 部門別問い合わせキューを作成](../04-Task-Routing-Queue/00-Overview.md)