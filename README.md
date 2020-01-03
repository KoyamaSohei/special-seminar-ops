# これは何

[情報特別演習](https://www.coins.tsukuba.ac.jp/special-seminar/index1.html)の成果物

# 何ができる

動的にキャッシュ対象を変更できるWebプロキシ

Cloudflareの(稚拙な)サブセット

![デモ](https://user-images.githubusercontent.com/17472875/71737493-28f05580-2e97-11ea-99f8-882fc8b0366f.gif)


HTTPヘッダに`Surrogate-Control: max-age=(time in seconds)`を追加することでキャッシュ制御出来る