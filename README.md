
![Release](https://img.shields.io/github/release/ryonakagami/byobu_setup.svg)
![License](https://img.shields.io/github/license/ryonakagami/byobu_setup.svg)
![Issues](https://img.shields.io/github/issues/ryonakagami/byobu_setup.svg)

---

## Scope

- `byobu`のセットアップ用レポジトリ
- `byobu_setup_ubuntu`は`~/.byobu`ディレクトリのうち特にユーザー側で変更したスクリプトを格納
- 基本的にはUbuntu OSを想定したセットアップを実施している

## How to use

1. OSに対応した`byobu`設定ディレクトリを選択（例: Ubuntuならば`byobu_setup_ubuntu`）
2. `status`など設定ファイルを`~/.byobu`にコピーする
3. `/bin`ディレクトリのファイルに関してはコピー時に実行権限を`chmod +x`で付与する

## Dependency

|プログラム|説明|インストール|
|---|---|---|
|`gpustat`|GPU使用状況計測プログラム|`pipx install gpustat`|

## Customization

### Editorの選択

`select-editor`を実行することで，printscreenの表示先など，`byobu`がデフォルトで開くエディタを選択することができる：

```zsh
% select-editor

Select an editor.  To change later, run 'select-editor'.
  1. /bin/nano        <---- easiest
  2. /usr/bin/vim.basic
  3. /usr/bin/nvim
  4. /usr/bin/vim.tiny
  5. /usr/bin/code
  6. /bin/ed
```
