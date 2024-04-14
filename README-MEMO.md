# Visual Studio Code 便利機能

## ショートカットキー

| キー | 説明 |
| ---- | ---- |
| Ctrl + D | 同じテキストを追加選択 |
| Ctrl + Shift + L | 同じテキストをすべて選択 |
| Alt + ↑ or ↓ | 行単位移動 |
| Shift + Alt + ドラッグ | 矩形選択 |
| Alt + 複数箇所クリック | 選択したところを選択 |
| Alt + Shift + ↑ or ↓ | 選択エリアを複製 |
| Ctrl + Alt + ↑ or ↓ | カーソルを複数箇所に置く |
|  |  |
|  |  |

## Markdown

https://learn.microsoft.com/ja-jp/contribute/content/markdown-reference

## 設定ファイル

環境変数

`%APPDATA%` : `C:\Users\【ユーザー名】\AppData\Roaming\`

`%USERPROFILE%` : `C:\Users\【ユーザー名】\`

settings.json
- ユーザー設定用の設定ファイル
- 保存先
  - `%APPDATA%\Code\User\`
  - `~/Library/Application Support/Code/User/`

.code-workspaceファイル
- ワークスペース設定用の設定ファイル
- 保存先
  - ワークスペースとして保存される
  - 中身はsettings.jsonで、先に優先される

keybindings.json
- キーボードショートカットのカスタマイズやオーバーライドを行うファイル。
- 保存先
  - `%APPDATA%\Code\User\`
  - `~/Library/Application Support/Code/User/`

launch.json
- デバッグ設定を管理するファイル。  デバッガの起動設定やデバッグ環境変数の設定などを行います。
- 保存先
  - `%USERPROFILE%\.vscode\`
  - `~/.vscode/`

tasks.json
- ビルド、テストなどのタスク実行設定を管理するファイル。  ターミナルでの実行コマンドやタスクの自動化を設定できます。
- 保存先
  - `%USERPROFILE%\.vscode\`
  - `~/.vscode/`

extensions.json
- インストール済みの拡張機能の一覧とその設定を管理するファイル。
- 保存先
  - `%USERPROFILE%\.vscode\`
  - `~/.vscode/`

snippets.json
- スニペットの定義とカスタマイズを行うファイル。  よく使うコード断片をショートカットとして登録できます。
- 保存先
  - ユーザースニペット: `%USERPROFILE%\.vscode\snippets\{言語ID}.json`
    - `~/.vscode/snippets/{言語ID}.json`
  - ワークスペーススニペット: `{ワークスペースフォルダ}\.vscode\snippets\{言語ID}.json`

これらのJSONファイルは、ユーザーフォルダ(.vscode)やワークスペースフォルダ直下の.vscodeフォルダに保存されます。

プロジェクト単位でカスタマイズしたい設定は、ワークスペースの設定ファイルを編集します。