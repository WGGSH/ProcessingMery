# ProcessingMery
MeryでProcessingの開発を行うための拡張機能

## 作成するファイル一覧
* [ext/pde.txt](src/pde.txt)  
  pdeファイルを開いたときにProcessingの予約語を補完可能にする  
* [Processing.msy](src/Processing.msy)  
  Processing用の構文ファイル  
* [Processing-java](src/processing-java.txt)  
  Meryのメニューコマンドで，Processingをビルド，実行する  

## 導入方法
* pde.txt
  Meryの実行ディレクトリ内にある[Ext]ディレクトリの中にpde.txtを置くと，
	Processingのファイルを開いたときに補完できるようになります
* Processing.msy
  [表示]→[編集モード]→[編集モードの設定]→[新規作成]で新しく編集モードを作成し，名前をProcessingにします  
	[プロパティ]を選択し[インポート]でProcessing.msyを選択します  
	[関連付け]タブに移動し，[関連付けられた拡張子]に"pde"を指定することで，  
	Processingのファイルを起動すると自動的に色付けが行われるようになります
* Processing-java
  [ツール]→[外部ツール]→[外部ツールの設定]→[新規作成]で新しく外部ツールを作成し，
	名前をprocessing-javaにします  
	コマンド，引数をprocessing-java.txtに記されたように入力し，[ファイルを保存する]にチェックを入れます
