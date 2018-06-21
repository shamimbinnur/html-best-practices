# `title`要素を書く

`title`要素の中身は、ブラウザーに限らず、様々なアプリケーションにより利用されます。

悪い例:

    <head>
      <meta charset="UTF-8">
    </head>

良い例:

    <head>
      <meta charset="UTF-8">
      <title>HTML Best Practices</title>
    </head>


## 解説

`title`要素は場合によっては省略することも可能とされています。タイトルが必要とされないような文書の場合がそれにあたります。具体的な例として、仕様では`head`要素の項で以下のように言及されています。

> 上位プロトコルがタイトル情報、たとえばHTMLが電子メールのオーサリング形式として使用されるときの電子メールの件名が提供される場合、title要素は省略できる。

この場合は電子メールの件名として既に`title`相当の情報が提供されているため必要とされません。他にも`iframe`要素の`srcdoc`属性で指定されるドキュメントでも省略可能となっています。どちらもかなり特別なケースだと言え、何かしらのソフトウェアが適切に取り扱う分野です。HTML文書においては`title`要素を省略することはできないと考えておきましょう。

また`title`要素によって提供される文書のタイトルはブラウザーや検索エンジンを始めとした様々なソフトウェアやサービスから利用されます。そういった観点からも省略することは望ましくありません。