# usn-asobi.jp

GitHub Pages で `usn-asobi.jp` を公開するための最小構成です。

## Files

- `index.html`: 公開される仮トップページ
- `CNAME`: GitHub Pages のカスタムドメイン指定
- `.nojekyll`: GitHub Pages の Jekyll 処理を無効化

## GitHub Pages settings

1. GitHub username または Organization owner を `Neo-Wellness` にします。
2. 表示名を `Neo Wellness` にします。
3. GitHub で `usn-asobi.jp` という名前の public repository を作成します。
4. このフォルダの内容を `main` ブランチへ push します。
5. Repository settings > Pages で Source を `Deploy from a branch`、Branch を `main` / `/root` にします。
6. Custom domain に `usn-asobi.jp` を設定します。
7. DNS が反映された後、`Enforce HTTPS` を有効にします。

## DNS records

DNS 管理画面で以下を設定します。

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| AAAA | @ | 2606:50c0:8000::153 |
| AAAA | @ | 2606:50c0:8001::153 |
| AAAA | @ | 2606:50c0:8002::153 |
| AAAA | @ | 2606:50c0:8003::153 |
| CNAME | www | Neo-Wellness.github.io |

`Neo-Wellness.github.io` は、公開に使う GitHub アカウントまたは Organization の GitHub Pages ドメインです。

## Push commands

GitHub 側で `usn-asobi.jp` repository を作ったあと、以下を実行します。

```sh
git remote add origin git@github.com:Neo-Wellness/usn-asobi.jp.git
git push -u origin main
```

GitHub のユーザー名には `.` を使えないため、`usn-asobi.jp` は repository 名として使います。

## Target configuration

- GitHub username: `Neo-Wellness`
- Repository Owner: `Neo-Wellness`
- Display name: `Neo Wellness`
- Repository name: `usn-asobi.jp`
- Public URL: `https://usn-asobi.jp`
