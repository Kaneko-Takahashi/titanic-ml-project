# 🛠️ 開発メモ

## Git ブランチ設定

### 問題
ローカルのブランチ名が `master` で、GitHubのデフォルトブランチが `main` のため、
SourceTreeから普通にプッシュするとGitHubに反映されない問題が発生。

### 解決方法
ターミナルで以下を実行して、master → main への自動プッシュを設定：

```bash
# プッシュのデフォルト設定を変更
git config push.default upstream

# masterブランチの追跡先をorigin/mainに設定
git branch --set-upstream-to=origin/main master