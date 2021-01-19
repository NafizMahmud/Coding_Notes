#### OpenAPI Object
OpenAPI ドキュメントのルートオブジェクトです。

- openapi：この文字列は OpenAPI 仕様バージョンの番号です。例："openapi": "3.0.0"

- info：APIに関するメタデータを提供します。[Info Object]
- servers：サーバー オブジェクトの配列で、ターゲット サーバーへの接続情報を提供します。[Server Object]
- paths：APIで利用可能なパスとオペレーション。[Paths Object]
- components：OASのさまざまな側面のための再利用可能なオブジェクトのセットを保持します。[Components Object]
- security：どのセキュリティメカニズムがAPI全体で使用できるかの宣言。[Security Requirement Object]
- tags：仕様で使用されるタグのリスト[Tag Object]
-  ー externalDocs：追加の外部文書[External Documentation Object] なし（非表示）
　・description, url

#### Info Object

- title：固定タイトル『ViewCreator Query Execute API』を表示
- description：ルーティング定義の備考を表示
- ーtermsOfService：APIの利用規約へのURL。URLの形式でなければなりません
- ーcontact：ContactObject（なし）
- name, url, email
- ーlicense：LicenseObject（なし）
　- name, url
- version：ViewCreatorバージョンを表示（例：8.0.26）

#### Server Object
- url：ターゲットホストへのURL（例："http://localhost:8080/imart"）
- description：URLで指定されたホストを記述する文字列（例：http server）
- ーvariables：ServerVariableObject (なし)
　- サーバーURLテンプレート置換用のサーバー変数を表すオブジェクト
　- enum, default, description

#### TagObject
- url：タグの名前です（ユーザ毎のロケールで表示）（例："テストルーティング-１"）
- description : タグの簡単な説明。ルーティング備考（ユーザ毎のロケールで表示）を設定
-  ーexternalDocs : [External Documentation Object] （なし）

#### PathsObject
- /{path}：個々のエンドポイントへの相対パス。[Path Item Object]

#### PathItemObject
1つのパスで利用可能な操作について説明

- $ref：パス項目の外部定義
- ーsummary：パスのすべてのオペレーションに適用される文字列の要約(省略可能)(未使用）
- ーdescription : なし(未使用）
- ・get : このパスのGETオペレーションの定義 [Operation Object]
- ーput : このパスのPUTオペレーションの定義 [Operation Object] (未使用）
- ・post : このパスのPOSTオペレーションの定義 [Operation Object]
- ーdelete : このパスのDELETEオペレーションの定義 [Operation Object] (未使用）
- ーoptions : このパスのOPTIONSオペレーションの定義 [Operation Object] (未使用）
- ーhead : このパスのHEADオペレーションの定義 [Operation Object] (未使用）
- ーpatch : このパスのPATCHオペレーションの定義 [Operation Object] (未使用）
- ーtrace : このパスのTRACEオペレーションの定義 [Operation Object] (未使用）
- ーservers : パスのすべてのオペレーションを処理するための代替サーバ配列[Server Object](未使用）
- ーparameters : パスで説明されているすべてのオペレーションに適用されるパラメータのリスト[Parameter Object](省略可能)(未使用）
