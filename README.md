# これは何

[情報特別演習](https://www.coins.tsukuba.ac.jp/special-seminar/index1.html)の成果物

# 何ができる

動的にキャッシュ対象を変更できるWebプロキシ

Cloudflareの(稚拙な)サブセット

![デモ](https://user-images.githubusercontent.com/17472875/72378902-a9e00480-3755-11ea-9def-981172433522.gif)


HTTPヘッダに`Surrogate-Control: max-age=(time in seconds)`を追加することでキャッシュ制御出来る

## ソースコード

[special-seminar-surrogate](https://github.com/KoyamaSohei/special-seminar-surrogate)

[special-seminar-lazy-ns](https://github.com/KoyamaSohei/special-seminar-lazy-ns)

[special-seminar-api](https://github.com/KoyamaSohei/special-seminar-api)

[special-seminar-web](https://github.com/KoyamaSohei/special-seminar-web)