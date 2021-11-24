# インフラセキュリティ入門

## 【０】最初に
セキュリティはコストとトレードオフです。ビジネス的にペイする適切な水準があるので、セキュリティ責任者は、プロダクトオーナーとよく話し合い、合意する必要があります。

## 【１】攻撃種類、諸々復習

* サイバー攻撃とは？その種類・事例・対策を把握しよう｜サイバーセキュリティ.com
<br>https://cybersecurity-jp.com/column/14651

* Ｗｅｂでの騙し・攻撃の手口 | 「経営と情報」に関する教材と意見
<br>http://www.kogures.com/hitoshi/webtext/sec-damashi-teguchi/index.html

## 【２】対策

### （１）セキュアコーディング
<br>脆弱性のないソフトウェアを用意することが重要。だが、バグのないプログムはない。
* ソフトウェアを常に最新化
* 不要なアプリケーションの除外、不要な設定やサービスの無効化
* デフォルト(標準状態)のアカウントやパスの変更、無効化
* IPA 独立行政法人 情報処理推進機構：重要なセキュリティ情報一覧 
<br>https://www.ipa.go.jp/security/announce/alert.html

### （２）セキュリティアプライアンスの利用

* 暗号化　SSL/TLS
<br>SSLとTLSとは？意外に知らないSSLとTLSの違い（簡単編） | 常時SSL Lab. by クラウド型レンタルサーバー「Zenlogic」 
<br>https://www.idcf.jp/rentalserver/aossl/basic/ssl-tls/

* IPS（不正侵入防止システム）
<br>IPS（不正侵入防止システム） | サイバーセキュリティ情報局 
<br>https://eset-info.canon-its.jp/malware_info/term/detail/00124.html

* IDS（不正侵入検知システム）
<br>IDS（Intrusion Detection System）とは 
<br>https://atmarkit.itmedia.co.jp/ait/articles/0401/01/news055.html

* Firewall（Fw）
<br>「ファイアウォール」とは | サイバーセキュリティ情報局 
<br>https://atmarkit.itmedia.co.jp/ait/articles/0401/01/news062.html
* ファイアウォールiptablesを簡単解説～初心者でもよくわかる！VPSによるWebサーバー運用講座(4) | さくらのナレッジ
<br>https://knowledge.sakura.ad.jp/4048/
* AWS Network Firewall
<br>https://aws.amazon.com/jp/network-firewall/?whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc

* ゲートウェイ型アンチウィルス
<br>製品 ゲートウェイアンチウイルス (Gateway AntiVirus) ｜ウォッチガード・テクノロジー 
<br>https://www.watchguard.co.jp/products/security-services/gateway-antivirus

* コンテンツフィルタリング　プロキシ
<br>プロキシサーバ／コンテンツフィルタ――ポリシーに合致しないアクセスの防止技術：セキュリティ・テクノロジー・マップ（6） - ＠IT 
<br>https://atmarkit.itmedia.co.jp/ait/articles/1608/31/news002.html

以上等の多層防御

そもそも、自分でシステムを抱え込まない
SaaS/PaaSを活用

## 【３】運用：セキュリティログ分析

### (1)ログに記録すべきこと
* いつ：日時
* 誰が：ユーザーID
* 何処から：IPアドレス
* 何を用いて：ユーザーエージェント
* 何をして：リクエストURL
* どうなった：結果
* 利用者の導線：Referer
* 一連の操作：セッションID

### (2)ログ解析基盤

* Fluentd＋Elasticsearch＋Kibanaで作るログ基盤の概要と構築方法 | ＠IT 
<br>https://atmarkit.itmedia.co.jp/ait/articles/1704/06/news013.html

* Kinesis Firehoseを使ってCloudWatch Logをs3へ出力してみた | CCI TECH BLOG
<br>https://tech-cci.io/archives/3561

* AWSでガッチリログ解析 | Oitta
<br>https://qiita.com/Naggi-Goishi/items/9d68b822c413b87a6bb6

## 【4】AWS セキュリティ

* サーバーワークス【AWSセキュリティ】
<br>https://www.youtube.com/watch?v=DTEMwx7b_No&list=PLCRz5JqTKzfnGpAKqwXlLMWwAAZW2xs43

* AWS環境における脅威検知と対応
<br>https://www.youtube.com/watch?v=e_Cf-aPBLtM

以上となります。
