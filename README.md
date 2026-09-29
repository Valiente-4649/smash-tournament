# Smash Tournament Site

大学eスポーツサークル向けスマブラ大会サイトのベースです。

## 重要
このZIPの index.html はそのままブラウザで動作するデモです。
ただし、参加者・観戦者の端末間でリアルタイムに同じ大会情報を共有するには、
Firebase / Supabaseなどの無料クラウドDBへの接続が必要です。

## GitHub Pagesで公開する場合
1. GitHubで新しいPublicリポジトリを作成
2. index.htmlをアップロード
3. Settings → Pages → Deploy from a branch → main / root
4. 数分後に発行されたURLを参加者へ共有

## 本番化について
現在のindex.htmlは「UIと大会進行ロジックのプロトタイプ」です。
本番ではFirebase Authentication + Firestore等を接続し、
- 管理者だけ開始・結果変更可能
- 参加者登録を全員で共有
- 試合状態をリアルタイム同期
- ダブルエリミネーションの勝者側/敗者側を完全管理
- Switch台の自動割り当て
を実装するのがおすすめです。
