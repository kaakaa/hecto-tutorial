## 感想

- 読みやすい英語
- 動かしながらわかりやすい文章構成
- GitHub 形式の Diff も編集しやすい
- 扱っているトピックも、出てくる順番がちょうどいい
- とにかく英語が読みやすい
- 何かプラットフォームがあればコーヒー代出すよ
- 2 章まで面白かったけど 3 章はターミナルの話が多かったな...長かったし...

- 気になった点
  - エディタ終了コマンドが`Ctrl + q`だけど、VS Code でやってるとショートカットでキーが奪われるな...
    - 個別事象だし報告するようなことじゃないか
- 3.
  - clippy を突然使うように言われるけど、インストールされていない。インストール手順があるといいかも。
    - https://github.com/rust-lang/rust-clippy#as-a-cargo-subcommand-cargo-clippy
  - pedantic でチェックすると、下記の warning が出る
    - その後すぐに self を使うようになるからか。（後で解消する旨、記述があると安心できる）

```
  warning: unused `self` argument
 --> src/editor.rs:9:16
  |
9 |     pub fn run(&self) {
  |                ^^^^^
  |
```

## chapter.1

- `rustup` の設定
- `cargo init` によるプロジェクトの新規作成
- Hello, World! の実行

## chapter.2

- stdin & print it
- use third-party crate (termion)
- ownership
- shadowing
- println
- bit operation
- error handling
- match

## chapter.3

- idiomic code
- separate files
- static analysis by clippy
- use escape sequences (VT100)
- get terminal windows size
- re-exporting struct at the top level (`pub use terminal::Terminal` in `main.rs`)
- overflow
- move cursor by arrow keys

## chapter. 4

- Vector
- #[derive(Default)]
- if statement as value
- command line arguments
- multi byte characters

## chapter.5

- Quit confirmation: duplicated semi-colon in editor.rs at l127?

## chapter.6

- closures (give callback function as an argument)
- Clone trait
- enum
- PartialEq, Copy trait
