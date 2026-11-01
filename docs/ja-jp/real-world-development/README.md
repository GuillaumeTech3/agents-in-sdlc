---
slug: ja-jp/real-world-development
title: "実践的な開発"
authors:
  - geektrainer
lastUpdated: 2026-09-16
---

現実的なシナリオ、完成したアプリケーション、共有バックログを使って、ソフトウェア開発ライフサイクル全体で GitHub Copilot を活用します。変更の計画、コードの作成、動作のテスト、プル リクエストのレビュー、エージェントを使った作業管理を反復的に進めます。

## シナリオ

架空の企業 Tailspin Toys に新しく加わった開発者として作業します。同社は開発者をテーマにしたボードゲームのクラウドファンディングを提供しています。チームのバックログは GitHub Issue として登録済みで、すぐに着手できます。フィルターやページネーションなどの機能に加え、アクセシビリティやコーディング規約などの品質改善も含まれています。

## 環境を選択する

GitHub Copilot はさまざまな作業環境で利用できます。自分の開発スタイルに合った環境を選びます。各ワークショップは個別のセットアップから始まり、共通の Tailspin Toys シナリオを使用します。

### [GitHub Copilot CLI][cli]

ターミナルでエージェント型アシスタントを使います。Plan モードと Autopilot モード、指示、スキル、カスタム エージェント、Playwright MCP、Agent Merge、便利なスラッシュ コマンドを学びます。

### [GitHub Copilot app][app]

エージェント セッションを並行して実行し、セッション モードを切り替え、Canvas で共同作業を行い、デスクトップ アプリで GitHub Issue とプル リクエストを管理します。

### [GitHub Copilot cloud agent][cloud]

GitHub Issue を非同期エージェントに割り当て、作業をガイドし、進行状況を監視して、エージェントが作成したプル リクエストをレビューします。

### [Visual Studio Code][vscode]

Visual Studio Code と GitHub Codespaces で GitHub Copilot を使います。エディターを離れずに Copilot Chat のエージェント モード、MCP サーバー、カスタム エージェントを活用します。

[cli]: cli/
[app]: app/
[cloud]: cloud/
[vscode]: vscode/
