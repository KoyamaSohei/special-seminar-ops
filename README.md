# これは何

[情報特別演習](https://www.coins.tsukuba.ac.jp/special-seminar/index1.html)の成果物

# 何ができる

動的にキャッシュ対象を変更できるWebプロキシ

- Web上の UI から自身が取得したドメインのDNSレコードを追加、変更、削除できる

  この前にはドメインのネームサーバーを移管しておく必要がある

- Aレコードを変更することで、オリジンサーバーを変更することが出来る

- このドメインにクライアントがhttpリクエストを発行した時、オリジンサーバーに直接リクエストが届くことはなく、プロキシサーバを通してコンテンツを得る

- プロキシサーバーはキャッシュ機能があり、これによってオリジンサーバーへのリクエスト数を削減できる。

![デモ](https://user-images.githubusercontent.com/17472875/72378902-a9e00480-3755-11ea-9def-981172433522.gif)


HTTPヘッダに`Surrogate-Control: max-age=(time in seconds)`を追加することでキャッシュ制御出来る

## ソースコード

[special-seminar-surrogate](https://github.com/KoyamaSohei/special-seminar-surrogate)

[special-seminar-lazy-ns](https://github.com/KoyamaSohei/special-seminar-lazy-ns)

[special-seminar-api](https://github.com/KoyamaSohei/special-seminar-api)

[special-seminar-web](https://github.com/KoyamaSohei/special-seminar-web)