# Visual Studio Code

## インストールの手順

### ダウンロード

下記リンク先からVisual Studio Codeをダウンロードする  
https://code.visualstudio.com/download

![](images/001.png)

`ダウンロード`フォルダに保存する  
![](images/002.png)

### インストール

ダウンロードしたファイルを実行  
![](images/003.png)

`同意する`にチェックを入れて`次へ`をクリック    
![](images/005.png)

`次へ`をクリック  
![](images/006.png)

`次へ`をクリック  
![](images/007.png)

下記にチェックを入れて`次へ`をクリック  
 - `デスクトップ上にアイコンを作成する`
 - `エクスプローラーのディレクトリコンテキストメニューに[Codeで開く]アクションを追加する`

![](images/009.png)

`インストール`をクリック  
![](images/010.png)

インストールされるので少し待つ  
![](images/011.png)

`完了`をクリック  
![](images/012.png)

## 初期設定

`< Welcome`の`<`の部分をクリック  
![](images/013.png)

`Show welcome page on startup`のチェックを外して、`Welcome`タブの`✕`ボタンをクリックして閉じる    
![](images/015.png)

## 日本語化

`拡張機能`ボタンをクリック  
![](images/016.png)

検索エリアに`japanese`と入力して、  `Japanese Language Pack for Visual Studio Code`の`Install`ボタンをクリックする  
![](images/018.png)

インストール完了後、右下の`Change Language and Restart`をクリックする
![](images/019.png)

日本語化完了  
![](images/020.png)

## 便利設定

### 自動保存を有効化

メニューバーから`ファイル`→`自動保存`をクリック  
![](images/021.png)

自動保存が有効化される  
![](images/022.png)

### フォントの拡大縮小有効化

メニューバーから`ファイル`→`ユーザー設定`→`設定`  
![](images/023.png)

`設定の検索`エリアに`Mouse Wheel Zoom`と入力して、下記項目にチェックを入れる  
 - `Editor: Mouse Wheel Zoom`
 - `Terminal › Integrated: Mouse Wheel Zoom`

![](images/025.png)

設定タブの`✕`ボタンをクリックして閉じる  
![](images/026.png)

## 個人メモ

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
