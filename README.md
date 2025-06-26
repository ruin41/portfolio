# Portfolio_Rematch_WorX_ENGINEER-CLASS

## アプリ概要
Next.jsとSupabaseを用いたSE用のマッチングアプリ風転職サイトです。  

## サイトイメージ

![アプリ画像](https://github.com/ruin41/portfolio/blob/288cd74d999e799ba55fbfe26f04f14dbac1854c/docs/%E3%82%A2%E3%83%95%E3%82%9A%E3%83%AA%E3%81%AE%E3%83%A1%E3%82%A4%E3%83%B3%E3%83%98%E3%82%9A%E3%83%BC%E3%82%B7%E3%82%99%E7%94%BB%E5%83%8F.png)

## サイトURL
 
[https://blogapp-forlecture.vercel.app/](https://job-matching-app.vercel.app/)


## 使用技術
- フロントエンド：Next.js 15.3
- バックエンド：Next.js 15.3、~Python 3.13.3（FastAPI0.115.12）~
- データベース：Supabase
- デプロイ：Vercel
- バージョン管理：Git、GitHub
- テスト・デバッグ：DevTools（Chrome）
- CI/CD：GitHub Actions（ESLint）

## 設計ドキュメント
[要件定義・基本設計・詳細設計の一覧_Googleスプレッドシート][([https://docs.google.com/spreadsheets/d/1yBssPgoUI_8TMwVZA2hWOLQj3-l7oirLB2FQ1YJgCww/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1YHzkrmUaLCRMExcWm0qv2Yr_Px2eHnPCH-5-jPPW9BE/edit?gid=983827669#gid=983827669))](https://docs.google.com/spreadsheets/d/1YHzkrmUaLCRMExcWm0qv2Yr_Px2eHnPCH-5-jPPW9BE/edit?gid=74722085#gid=74722085)

詳細設計時のワイヤーフレーム、ER図、ワークフロー図の画像はdocsディレクトリに格納しています。（[こちらからアクセス](./docs)）

## 機能一覧
🌟ユーザー側
- プロフィール登録
- プロフィール編集
- 検索機能
- マッチング企業一覧表示

🌟企業側
- 求人登録
- 求人編集
- マッチング求職者一覧を取得・表示
- 検索機能

🌟共通機能
- パスワードリセット
- アカウント登録
- アカウント削除(退会)
- ログイン
- ログアウト
- マッチング機能
- いいね送信
- いいね取得

## テスト・修正の設計及び実施書
[テスト・修正の設計及び実施書_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1FvDvHquW-M33XrAGH0t1HMZPw9Mdp7hiY1oATilu3Y0/edit?gid=0#gid=0)

## アプリの改善案
[アプリの改善案_Googleスプレッドシート](https://docs.google.com/spreadsheets/d/1P5C5et2X4FSdpowBbhluUjMu7Lu0RZ84VsPR9geTYJc/edit?gid=482600378#gid=482600378)

## 備考
[ESLintの実行結果_GitHub Actions](https://github.com/aihat9161/PortfolioExample_Next.js_BlogAppWorX_ENGINEER-CLASS/actions/runs/14956271682/job/42012343864)

- 活用した生成AIとその用途
  - ChatGPT：要件定義、設計、各種リサーチ
  - v0：アプリのモック作成
  - GitHub Copilot Chat：ローカル環境でのコードの修正相談

- リファクタリングの規則
  - 2つ以上のファイルで使う、行数が10以上のUIコンポーネントはcomponentsフォルダに移行
  - 2つ以上のファイルで使う、行数が10以上の関数はlibフォルダに移行
  - 変数名で2つ以上の単語が入る場合は、「isPublished」のように二つ目以降の単語の頭を大文字とする
