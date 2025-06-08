## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
  * エンドポイント`https://zipcloud.ibsnet.co.jp/api/search`
  * 機能　日本の7桁の郵便番号を入力として受け取り、対応する住所情報を返します。
* リクエストとレスポンスのフォーマット
  * GET `https://zipcloud.ibsnet.co.jp/api/search?zipcode=2991162`
{"status": 200,"message": null,"results": [{"zipcode": "2991162","prefcode": "12","address1": "千葉県","address2": "君津市","address3": "南子安","kana1": "ﾁﾊﾞｹﾝ","kana2": "ｷﾐﾂｼ","kana3": "ﾐﾅﾐｺﾔｽ"}]}
### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
  * 名称　The Cat API
  * 参照URL　[https://docs.thecatapi.com/](https://docs.thecatapi.com/)
* エンドポイントと機能
  * エンドポイント　`https://api.thecatapi.com/v1/images/search`
  * 機能　 ランダムな猫の画像を取得します。
* リクエストとレスポンスのフォーマット
  * メソッド: GET クエリパラメータ: `breed_ids`（品種ID、例: `bengal`, 省略可）フォーマット: JSON
### Q3-3. 感想
* 今回の課題で苦労したこと
  * 内容を理解することに時間がかかった
* 演習を通して理解できたこと
  * APIのドキュメントを読む重要性を理解した
* Web APIの利便性や課題など
  * 利便性：APIを使えば、住所や画像のようなデータを簡単に取得でき、Webページを動的にできる
  * 課題：APIごとのレスポンス形式の違いに慣れる必要がある
