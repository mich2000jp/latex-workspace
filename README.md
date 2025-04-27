# latex-workspace

## 導入方法

Mac ユーザ向けに記述します

1. Visual Studio Code を[ここ](https://code.visualstudio.com/download)からダウンロード・インストール
2. VSCode 用の拡張機能を入れる。LaTex Workshop は必須
3. TexLive を[ここ](https://www.tug.org/mactex/mactex-download.html)からダウンロード・インストール
4. [GitHub](https://github.com/)にアカウントを作る
5. Git リポジトリのクローン>GitHub から複製>https://github.com/mich2000jp/latex-workspace.git を選択。好きなフォルダを選んで「宛先として選択」する。このフォルダを開く。
6. document/main.tex ファイルを開き、右上の緑の再生ボタンを押す。すると main.pdf ができるはず。
7. エラーになる場合は main.log を確認。大抵は「パッケージがない」エラーだと思うので、log にある通りターミナルに打ってインストールする。.latexmkrc をすでに制作済みだったりする場合、それは消すかこのフォルダにある.latexmkrc で上書きする。

.vscode/settings.json から、色々な設定ができます。普段使わないファイルを vscode 上で非表示にできたりします。「command + ,」から設定を開き、「ワークスペース」を選んだ後右上の書類をひっくり返してるアイコンをクリックすることでも settings.json を開けます。
