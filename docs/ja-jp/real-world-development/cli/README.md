---
slug: ja-jp/real-world-development/cli
title: "GitHub Copilot CLI"
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** は、ターミナルで GitHub Copilot をエージェント型のコーディング アシスタントとして利用できるようにします。コードベースを探索し、コードを生成し、コマンドを実行し、外部ツールに接続できます。すべてコマンド ラインから行えるため、グラフィカル エディターに切り替えずに作業の流れを保てます。

このワークショップでは、Tailspin Toys の一連のワークフローに沿って進めます。GitHub Codespaces でプロジェクトを準備し、Copilot CLI をインストールして、星評価の小さな変更を加えた後、最初のプル リクエストを作成します。続いてフィルターの Issue を起点に、アプローチを計画し、機能を実装してレビューします。リポジトリの指示を更新し、品質チェック用のスキルをカスタマイズし、Playwright MCP で動作をテストして、QA エージェントを作成します。最後に、変更全体をレビューし、フィルターのプル リクエストで Agent Merge を使い、便利なスラッシュ コマンドを確認します。[GitHub Copilot CLI と Foundry を使う 3 モジュールのオプション シリーズ][foundry]で、モデルを準備し、ホスト型エージェントを構築・デプロイしてサイトに接続することもできます。

プル リクエストは 2 つ作成します。1 つ目は星評価、2 つ目は指示、スキル、QA プロファイル、テストの更新を含むフィルター機能です。フィルターと品質に関する作業は同じ会話とブランチで進めるため、各ツールを学びながら作業を積み重ねられます。

## レッスン

| 演習 | トピック | 説明 |
|----------|-------|-------------|
| [0. 前提条件][ex0] | セットアップ | リポジトリと Codespace を準備する |
| [1. Copilot CLI をインストールする][ex1] | インストール | Copilot CLI をインストールして認証し、基本操作を確認する |
| [2. 星評価を追加する: 小さな改善][ex2] | 最初の変更 | 既存の評価と null の場合の表示を追加し、最初の PR をマージする |
| [3. エージェント モード: Plan と Autopilot][ex3] | エージェント モード | Issue から機能を計画し、Autopilot で実装して Interactive でレビューする |
| [4. カスタム指示で Copilot をガイドする][ex4] | コンテキスト | 指示を確認・更新し、フィルター作業に適用する |
| [5. quality-checks スキルをカスタマイズして使用する][ex5] | 繰り返し可能なチェック | 既存のスキルを確認し、レポート形式を変更して実行する |
| [6. Playwright MCP で機能を検証する][ex6] | ブラウザーでの確認 | CLI で MCP を設定し、フィルターの動作を調べる |
| [7. QA エージェントを作成して使用する][ex7] | 要件とカバレッジ | 専門プロファイルを作成・選択し、最終検証の証拠を集める |
| [8. 機能のプル リクエストを作成してマージする][ex8] | レビューとマージ | 変更全体を確認し、PR を作成して Agent Merge を使用する |
| [9. GitHub Copilot CLI のスラッシュ コマンド][ex9] | CLI 機能 | コンテキスト、モデル、共有、クラウド エージェントへの任意の委任を確認する |
| [10. まとめと次のステップ][ex10] | まとめ | ワークフロー、再利用可能なカスタマイズ、追加リソースを確認する |
| [オプション: Foundry を組み込む][foundry] | ホスト型エージェント | モデルを準備し、カタログに基づくエージェントをデプロイして Web サイトに接続する |

## 前提条件

このワークショップに参加する前に、次を準備してください。

- [ ] **Copilot Student、Pro、Pro+、Business、Enterprise** のいずれかの有効なプランがある GitHub アカウント
- [ ] リポジトリと Codespace を作成する権限
- [ ] ターミナルまたはコマンド ラインの基本的な知識

> [!TIP]
> 有料プランがありませんか。認証済みの学生は [GitHub Education][callout-student-plan-education] を通じて GitHub Copilot を無料で利用できます。**Copilot Student** プランには、このワークショップで使用する agent、MCP、code review、Copilot CLI の機能が含まれています。

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> Copilot Business または Copilot Enterprise を使用している場合は、管理者が Copilot CLI を有効にしていることを確認してください。

## はじめる

**[演習 0: 前提条件から始める →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
