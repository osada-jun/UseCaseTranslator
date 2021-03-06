# シナリオセット - テストスイートExcelファイル

テストスイートExcelファイル生成ユースケース。

## アクター

### 主アクター

ユーザー

### 副アクター

(なし)

## シナリオ

### 組みこみのテンプレートファイルを利用したテストスイートExcelファイルの生成

正しく記述されたユースケースカタログYAMLファイルの指定で、組みこみテンプレートファイルを利用したテストスイートExcelファイルを生成する。

#### 事前条件

指定の形式で正しく記述したユースケースカタログYAMLファイルとユースケースシナリオYAMLファイルを用意

#### アクション

1. コマンドラインプロンプトまたはPowserShellコンソールを起動
    * コマンドラインプロンプトまたはPowserShellコンソールが開く
2. UseCaseTranslator.exeの存在するディレクトリにパスを変更(存在ディレクトリは事前に確認)
    * パスがUseCaseTranslator.exeの存在するディレクトリに移動
3. 次をタイプして実行する: UseCaseTranslator -i [ユースケースカタログYAMLファイルのパス]
    * プログラムが正常に終了する(プロンプト・コンソールには情報は表示されない)
    * ユースケースカタログYAMLファイルの存在するディレクトリにテストスイートExcelファイルが作成される。ファイル名は"[ユースケースカタログYAMLファイルで指定したタイトル]-テストスイート.xslx"

### 出力ディレクトリを指定したテストスイートExcelファイルの生成

出力ディレクトリを指定してテストスイートExcelファイルを生成する。

ベースシナリオは「組みこみのテンプレートファイルを利用したテストスイートExcelファイルの生成」。

#### 事前条件

* 指定の形式で正しく記述したユースケースカタログYAMLファイルとユースケースシナリオYAMLファイルを用意
* テストスイートExcelファイル出力ディレクトリを用意。既存のテストスイートExcelファイルが存在するときは削除

#### アクション

1. コマンドラインプロンプトまたはPowserShellコンソールを起動
    * コマンドラインプロンプトまたはPowserShellコンソールが開く
2. UseCaseTranslator.exeの存在するディレクトリにパスを変更(存在ディレクトリは事前に確認)
    * パスがUseCaseTranslator.exeの存在するディレクトリに移動
3. 次をタイプして実行する: UseCaseTranslator -i [ユースケースカタログYAMLファイルのパス] -o [テストスイートExcelファイル出力ディレクトリ]
    * プログラムが正常に終了する(プロンプト・コンソールには情報は表示されない)
    * 引数-oで指定したディレクトリにテストスイートExcelファイルが作成される。ファイル名は"[ユースケースカタログYAMLファイルで指定したタイトル]-テストスイート.xslx"

### 出力形式指定によるテストスイートExcelファイルの生成

出力形式を明示的に指定してテストスイートExcelファイルを生成する。

ベースシナリオは「組みこみのテンプレートファイルを利用したテストスイートExcelファイルの生成」。

#### 事前条件

指定の形式で正しく記述したユースケースカタログYAMLファイルとユースケースシナリオYAMLファイルを用意

#### アクション

1. コマンドラインプロンプトまたはPowserShellコンソールを起動
    * コマンドラインプロンプトまたはPowserShellコンソールが開く
2. UseCaseTranslator.exeの存在するディレクトリにパスを変更(存在ディレクトリは事前に確認)
    * パスがUseCaseTranslator.exeの存在するディレクトリに移動
3. 次をタイプして実行する: UseCaseTranslator -t TestSuite -i [ユースケースカタログYAMLファイルのパス]
    * プログラムが正常に終了する(プロンプト・コンソールには情報は表示されない)
    * ユースケースカタログYAMLファイルの存在するディレクトリにテストスイートExcelファイルが作成される。ファイル名は"[ユースケースカタログYAMLファイルで指定したタイトル]-テストスイート.xslx"

### 指定テストスイートテンプレートExcelファイルを利用したテストスイートExcelファイルの生成

正しく記述されたユースケースカタログYAMLファイルの指定で、指定テストスイートテンプレートExcelファイルを利用したテストスイートExcelファイルを生成する。

ベースシナリオは「組みこみのテンプレートファイルを利用したテストスイートExcelファイルの生成」。

#### 事前条件

* 指定の形式で正しく記述したユースケースカタログYAMLファイルとユースケースシナリオYAMLファイルを用意
* 指定の形式で正しく記述したテストスイートテンプレートExcelファイルを用意

#### アクション

1. コマンドラインプロンプトまたはPowserShellコンソールを起動
    * コマンドラインプロンプトまたはPowserShellコンソールが開く
2. UseCaseTranslator.exeの存在するディレクトリにパスを変更(存在ディレクトリは事前に確認)
    * パスがUseCaseTranslator.exeの存在するディレクトリに移動
3. 次をタイプして実行する: UseCaseTranslator -i [ユースケースカタログYAMLファイルのパス] -a [テストスイートテンプレートExcelファイル]
    * プログラムが正常に終了する(プロンプト・コンソールには情報は表示されない)
    * ユースケースカタログYAMLファイルの存在するディレクトリにテストスイートExcelファイルが作成される。ファイル名は"[ユースケースカタログYAMLファイルで指定したタイトル]-テストスイート.xslx"
    * テストスイートExcelファイルには引数で指定したテストスイートテンプレートExcelファイルの書式他が反映される

### 存在しないユースケースカタログYAMLファイルの指定

存在しないユースケースカタログYAMLファイルが指定されたときはエラーが報告される。

ベースシナリオは「組みこみのテンプレートファイルを利用したテストスイートExcelファイルの生成」。

#### 事前条件

テストスイートExcelファイル出力ディレクトリを用意。既存のテストスイートExcelファイルが存在するときは削除

#### アクション

1. コマンドラインプロンプトまたはPowserShellコンソールを起動
    * コマンドラインプロンプトまたはPowserShellコンソールが開く
2. UseCaseTranslator.exeの存在するディレクトリにパスを変更(存在ディレクトリは事前に確認)
    * パスがUseCaseTranslator.exeの存在するディレクトリに移動
3. 次をタイプして実行する: UseCaseTranslator -i C:\not-exist-usecase-catalog.yaml -o C:\
    * プロンプト・コンソールにユースケースカタログYAMLファイルが存在しない旨のメッセージが表示される
    * プログラムは正常に終了する
    * 引数-oで指定したディレクトリにテストスイートExcelファイルが作成されない

## 更新履歴

### 第一版(2016-07-27)

作成。

### 第二版(2016-07-29)

ユースケース「指定テストスイートテンプレートExcelファイルを利用したテストスイートExcelファイルの生成」を追加。

### 第三版(2016-08-19)

機能追加・シナリオセット整理にあわせて内容を更新。
