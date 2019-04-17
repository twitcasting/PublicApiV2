# Change Log

ツイキャスPublicApiの変更点をまとめています。

APIの仕様については、[公式ドキュメント](https://apiv2-doc.twitcasting.tv/)を御覧ください。

Twitter [@twitcasting_dev](https://twitter.com/twitcasting_dev) での情報発信も行っております。

## 2019-04-17
### Fixed
- [Movie Object](https://apiv2-doc.twitcasting.tv/#movie-object)
  - `hls_url` パラメータの URL を `http` から `https` に変更しました

## 2018-10-09
### Fixed
- [Get Comments](https://apiv2-doc.twitcasting.tv/#get-comments)
  - コメントオブジェクトの `message` フィールドの制御文字のエスケープについて[RFC4627](https://www.ietf.org/rfc/rfc4627.txt)準拠の方式へ変更しました
- [Post Comment](https://apiv2-doc.twitcasting.tv/#post-comment)
  - 同上


## 2018-09-27
### Changed
- [Incoming WebHook](https://apiv2-doc.twitcasting.tv/#incoming-webhook)
  - リクエストボディに `broadcaster` 追加されました

## 2018-09-03
### Changed
- [User Object](https://apiv2-doc.twitcasting.tv/#get-user-info)
  - `supporter_count`, `supporting_count` パラメータが固定値 `0` となり、非推奨になりました
- [Get User Info](https://apiv2-doc.twitcasting.tv/#get-user-info)
  - `supporter_count`, `supporting_count` パラメータが追加されました
- [Verify Credentials](https://apiv2-doc.twitcasting.tv/#verify-credentials)
  - `supporter_count`, `supporting_count` パラメータが追加されました

## 2018-08-28
### Changed
- [Get Movies by User](https://apiv2-doc.twitcasting.tv/#get-movies-by-user)
  - `offset` の値の上限が `1000` になりました
  - `slice_id` パラメータが追加されました
- [Get Comments](https://apiv2-doc.twitcasting.tv/#get-comments)
  - `slice_id` に指定可能な最小値が `1` になりました

## 2018-08-03
### Changed
- [Validation Error Code](https://apiv2-doc.twitcasting.tv/#validation-error-code-1001) が変更されました
- [User Object](https://apiv2-doc.twitcasting.tv/#get-user-info)
  - `created` パラメータが固定値 `0` となり、非推奨になりました

