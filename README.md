# Java EE Webアプリケーションサンプル

これは基本的なServlet/JSPによるHello Worldウェブアプリケーションです。

## 必要条件

- Java 8 以上
- Gradle 7.0 以上（または付属のGradleラッパーを使用）
- インターネット接続（依存関係のダウンロードのため）

## ビルドと実行方法

### Gradleを使う場合

1. プロジェクトのルートディレクトリで以下のコマンドを実行してビルドします：

_Linux/Macの場合_ 
```bash
./gradlew clean build
```

_Windowsの場合_
```bash
gradlew.bat clean build
```

2. 内蔵のTomcatサーバーでアプリケーションを実行するには：

_Linux/Macの場合_
```bash
./gradlew appRun
```

_Windowsの場合_
```bash
gradlew.bat appRun
```

3. ブラウザで以下のURLにアクセスします：

- トップページ: [http://localhost:8080/](http://localhost:8080/)
- Hello World ページ: [http://localhost:8080/hello](http://localhost:8080/hello)

## プロジェクト構造

```
src/main/java/        - Javaソースコード
  └── com/example/servlet/
      └── IndexServlet.java - トップページのServlet
src/main/webapp/      - Webリソース
  └── WEB-INF/
      └── jsp/
          └── index.jsp - トップページのJSP
``` 