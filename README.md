# Open APIの定義について

* 「[REST WebAPI サービス 設計](https://www.udemy.com/course/rest-webapi-development/)」のUdemyで学習した内容を記録する

## 導入手順
1. yamlファイルでAPI設計を記述する
   1. 記載方法は、`https://github.com/swagger-api/swagger-editor`のルートにある`index.html`を参照
1. VSCodeに`Swagger Viewer`の拡張を導入する
1. VSCodeで`Shift + Option + P`を押すと、プレビューが確認できる

## APIドキュメントツール

* Swagger
  * https://editor.swagger.io/

* ReDoc
  * https://redocly.github.io/redoc/

## その他
* SwaggerUIをGitHub Pagesでホスティングする方法
  * [SwaggerUIを簡単にGithub Pagesで公開する方法](https://qiita.com/youdays/items/38f15b90402d097fb13e)

* ReDocをGithub Pagesでホスティングする方法
  1. 以下の構造で、ディレクトリ構成する
      * `index.html` 
        * [ReDocリポジトリのTL;DR](https://github.com/Redocly/redoc#tldr)をコピペする
        * `spec-url`の値を`swagger.yaml`に書き換える（相対パスを記載する）
    ```
    .
    └── docs
        └── index.html
        └── swagger.yaml
    ```

  2. GithubリポジトリのSettings > Optionsの下にある、Github Pagesの設定を行う
    1. Sourceを、ブランチを公開したいページがあるブランチに設定し、フォルダを/(docs)に設定する（/(root)に設定しても良いが、ルート直下に公開したいファイルを直接置くことになる）
    2. Saveする
  3. `https://<username>.github.io/<repository>/`をブラウザで開く