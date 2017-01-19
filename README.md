ここにメモをしておく。

・commonフォルダ
　・header.jsp
　　…常にヘッダーに表示されるファイル。
　　　追加機能として、ロゴ画像を永井君が1か月かけて作ってくれました。
　　　それと、平塚君がロゴ画像にトップページのリンクをつけて、検索機能をつけました。
　・footer.jsp
　　…常にフッターに表示されるファイル。
・errorフォルダ
　・error.jsp
　　…予想外のエラーが発生した場合に表示されるファイル。
　・sqlerror.jsp
　　…SQLのエラーが発生した場合に表示されるファイル。
・imgフォルダ
　・logo.gif
　　…永井君が一か月かけて作ってくれました。
・WEB-INFフォルダ
　・classesフォルダ
　　…srcフォルダのファイルをコンパイルしたクラスファイルを入れているフォルダ。
　・libフォルダ
　　…jstlなどを使用するためのjarファイルを入れているフォルダ。
　・srcフォルダ
　　・ex
　　　・AppException.java
　　　　…アプリケーション例外
　　　・LogicException.java
　　　　…システム例外
　　　・NoContentException.java
　　　　…詳細例外
　　・fw
　　　・DBManager.java
　　　　…コネクションの取得、SQL文を実行、記事一覧を取得を行う。
　　　・EncodingFilter.java
　　　　…Filterを使って遷移するたびにエンコードをセットする。
　　　・ResultSetBeanMapping.java
　　　　…受け取った結果セットからすべての値を受け取りWikiPageにセットして返す。
　　・wiki
　　　…サーブレット、Bean、不正文字列の訂正ロジック
　　　　共通メソッドのファイルが入っているフォルダ。
　　　・CreateServlet.java
　　　　…記事作成用のクラス。
　　　・ListServlet.java
　　　　…記事一覧を取得するためのクラス。
　　　・ReferServlet.java
　　　　…記事内容を取得するクラス。
　　　・RequestUtils.java
　　　　…ヘッダーのメッセージを表示するためのクラス。
　　　・SearchServlet.java
　　　　…追加機能のクラス。実は、ListServletを利用して少し改良しただけだったり。
　　　　　検索結果がない場合などを作るのに最初は表示されなくて少し悩みました。
　　　・UpdateServlet.java
　　　　…アップデートを行うクラス。
　　　・WikiFormater.java
　　　　…不正な文字列を変換するクラス。
　　　・WikiPage.java
　　　　…Bean。
　　　・WikiPageDAO.java
　　　　…DAO。
　・web.xml
　　…web.xml。
・create.jsp
　…記事名を記入するためのページ。
・create2.jsp
　…記事内容を記入するためのページ。
・index.jsp
　…indexという名のwelcomeという記事に送るページ。
・list.jsp
　…記事一覧を表示させるページ。
・refer.jsp
　…記事を表示させるページ。
・search.jsp
　…追加機能の検索結果を表示させるページ。
　　検索機能をつけるにあたって苦労したことは、オラクルで取得した値を表示するところです。
・update.jsp
　…記事内容を変更、削除を行うページ
