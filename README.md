# latex-workspace

## 導入方法（Mac ユーザ向け）

github ページ　https://github.com/mich2000jp/latex-workspace

1. 「Visual Studio Code」を[ここ](https://code.visualstudio.com/download)からダウンロード・インストール
2. VSCode 用の拡張機能「LaTex Workshop」を入れます。
3. 「MacTex」または「TexLive」を[ここ](https://www.tug.org/mactex/mactex-download.html)からダウンロード・解凍してインストーラを起動、画面の指示にそってインストール（時間がかかります。すでにインストールしている場合は不要です）
4. 「latex-workspace」をこのページ右上の「code」から「Download ZIP」でインストール。好きな場所に解凍（icloud drive 上に置くと便利です）
5. VSCode を起動して、「開く」からダウンロードしたフォルダの場所を選ぶ。
6. document/main.tex または slide/main.tex を開きます。画面右上の緑の再生ボタンを押すとコンパイルができ、pdf が生成または更新されます。

## うまく pdf が生成できないとき

まず必要なものをインストールしているか確認してください。

1. VSCode の拡張機能「Latex Workshop」を導入していますか？
2. 「MacTex」または「TexLive」をダウンロード、インストールしていますか？

過去に latex の導入を試みた方は、「.latexmkrc」ファイルを作成しているかもしれません。その場合、過去に作成した「.latexmkrc」を消すか、このフォルダにある「.latexmkrc」で上書きしてください（ホームディレクトリに「.latexmkrc」を作成している場合が多いです。Finder アプリを開き、「Shift+Command+H」でホームディレクトリに移動し、「Shift+Command+ . 」で隠しファイルを表示して、「.latexmkrc」があるか確認してください）。

それでも解決しない場合、エラーメッセージまたは「.intermediates/main.log」を確認してください。

## 基本的な使い方

ルートフォルダの下に好きな名前のフォルダを作り、その中に xxxx.tex を作っても同じように使えます。授業やゼミごとにフォルダを変えて使ってみてください。ただしフォルダを入れ子式にすることはできません。

（良い例）
latex-workspace
┣ ミクロ経済学 I
┃ 　 ┣ homework1.tex
┃ 　 ┗ homework2.tex
┣ マクロ経済学 I
┃ 　 ┗ homework1.tex
┗ README.md

悪い例
latex-workspace
┣ 経済学
┃ 　 ┣ ミクロ経済学 I
┃ 　 ┃ 　 ┣ homework1.tex
┃ 　 ┃ 　 ┗ homework2.tex
┃ 　 ┣ マクロ経済学 I
┃ 　 ┗ homework1.tex
┗ README.md

使っていてエラーになる場合は「.intermediates/xxxx.log」を確認。大抵は「パッケージがない」エラーだと思うので、log にある通りターミナルに打ってインストールしてください。

ここでは「LaTeX」のうち「LuaTeX」という種類のエンジンを使っています。LuaLateX に対応していないパッケージや記法を使っていないか確認してください。

.vscode/settings.json から、色々な設定ができます。普段使わないファイルを vscode 上で非表示にできたりします。「command + ,」から設定を開き、「ワークスペース」を選んだ後右上の書類をひっくり返してるアイコンをクリックすることでも settings.json を開けます。
