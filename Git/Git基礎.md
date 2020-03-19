# Git でのチーム開発の注意点

- 使うファイルを事前にチームに伝えておくこと
- コンフリクトは絶対起こるものなので過剰に気を使わないこと

## gint init の取り消し

- `rm -rf .git`

## git 基本コマンド

```ruby
git add [ファイル名] //追加
git commit -a -m "任意のコメント"  //コミット (-aオプションは変更を自動検出してくれる)
git push origin master  //masterを更新
```
