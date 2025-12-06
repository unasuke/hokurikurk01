# QUIC(TLS 1.3)実装進捗

author
:   unasuke

content-source
:  RubyKaigi 2025 follow up

date
:  2025-08-30

theme
: theme

# 自己紹介

* Name: うなすけ
* Work: フリーランス
* Kaigi on Rails 2025オーガナイザー (09/26-27 開催)
* {::tag name='x-small'}GitHub <https://github.com/unasuke>{:/tag}
* {::tag name='x-small'}Fediverse <https://mstdn.unasuke.com/@unasuke>{:/tag}
* {::tag name='x-small'}X <https://twitter.com/yu_suke1994>{:/tag}
* {::tag name='x-small'}<https://unasuke.com>{:/tag}

![](img/icon.jpg){:relative_width='24' align='right' relative_margin_right='-8' relative_margin_top='20'}

# 元ネタない勢(1人)

![](img/timetable.png){:relative_width='100'}

# 経緯
1. QUICプロトコルをRubyで実装したい
2. 一旦Python実装のRuby移植は不完全ながらできた(これがGrantでの成果)
3. より"Rubyらしい"コードになるように実装し直している
4. *QUICを実装するためにはTLS 1.3を実装しないといけない* ← ｲﾏｺｺ

\\nずっとTLS 1.3の実装してる


# 進捗
実際にご覧いただこう

# 今のは何？
* `www.example.com` に対して (https) HTTP/1.1 でGET requestを飛ばしている
* TLS handshakeをする
* 返ってきた暗号化されたデータを解く
* 標準出力に表示しておしまい

# 取り組んでいたこと
* Client側Handshake flowのリファクタ
* そもそもHTTPSでreq/resをするサンプルクライアントの実装
* 色々不足していたものたちの実装&リファクタ

# 取り組んでいたことlist
* [QUIC実装月報 2025年3月 \| うなすけとあれこれ](https://blog.unasuke.com/2025/quic-impl-monthly-report-202503/)
  * 進捗らしい進捗があるのはここだけかも
* [QUIC実装月報 2025年4月 \| うなすけとあれこれ](https://blog.unasuke.com/2025/quic-impl-monthly-report-202504/)
* [QUIC実装月報 2025年5月 \| うなすけとあれこれ](https://blog.unasuke.com/2025/quic-impl-monthly-report-202505/)
* [QUIC実装月報 2025年6月 \| うなすけとあれこれ](https://blog.unasuke.com/2025/quic-impl-monthly-report-202506/)
* [QUIC実装月報 2025年7月 \| うなすけとあれこれ](https://blog.unasuke.com/2025/quic-impl-monthly-report-202507/)

# やってたよ
ruby-jp discordの `#weekly-shinchoku` で垂れ流しています

![](img/discord-log.png){:relative_width='60'}

# 実際にご覧いただこう2
実際にご覧いただこう

# HELP ME
会場にお越しのTLS有識者の方


# 今後の展望
* 明日からまた開発中断します
  * Kaigi on Rails 2025のため……
* 10月から復活！
  * したい……
