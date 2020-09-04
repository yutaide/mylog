# Git submodule

#### submoduleの登録を解除

```text
git submodule deinit -f <サブモジュールのパス>
git rm -f <サブモジュールのパス>

# .git/modules/の中身は、上記コマンド実行後も消されないgitの仕様。
# 消えていない中身の影響でコマンドが上手く実行できない場合は、
# .git/modules/の中身を手動で削除する。
[参考]('To completely remove a submodule'で検索すると良い)
https://git-scm.com/docs/gitsubmodules

# 以下で新たなsubmoduleを登録できる。
git add submodule <リポジトリURL>
```

