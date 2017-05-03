# HTTPStatusCode

typedef NS_ENUM(NSInteger, HTTPStatusCode) {
    HTTPStatusCodeZero                              =   0, // デフォルト値
    
    // 1xx Informational 情報 : リクエストは受け取られた. 処理は継続される
    HTTPStatusCodeContinue                          = 100, // 継続
    HTTPStatusCodeSwitchingProtocols                = 101, // プロトコル切替え
    HTTPStatusCodeProcessing                        = 102, // 処理中
    
    // 2xx Success 成功 : リクエストは受け取られ、理解され、受理された
    HTTPStatusCodeOK                                = 200, // OK
    HTTPStatusCodeCreated                           = 201, // 作成
    HTTPStatusCodeAccepted                          = 202, // 受理
    HTTPStatusCodeNonAuthoritativeInformation       = 203, // 信頼できない情報
    HTTPStatusCodeNoContent                         = 204, // 内容なし
    HTTPStatusCodeResetContent                      = 205, // 内容のリセット
    HTTPStatusCodePartialContent                    = 206, // 部分的内容
    HTTPStatusCodeMultiStatus                       = 207, // 複数のステータス
    HTTPStatusCodeAlreadyReported                   = 208, // 既に報告
    HTTPStatusCodeIMUsed                            = 226, // IM使用
    
    // 3xx Redirection リダイレクション : リクエストを完了させるために、追加的な処理が必要
    HTTPStatusCodeMultipleChoices                   = 300, // 複数の選択
    HTTPStatusCodeMovedPermanently                  = 301, // 恒久的に移動した
    HTTPStatusCodeFound                             = 302, // 発見した
    HTTPStatusCodeSeeOther                          = 303, // 他を参照せよ
    HTTPStatusCodeNotModified                       = 304, // 未更新
    HTTPStatusCodeUseProxy                          = 305, // プロキシを使用せよ
    HTTPStatusCodeUnused                            = 306, // 将来のために予約されている
    HTTPStatusCodeTemporaryRedirect                 = 307, // 一時的リダイレクト
    HTTPStatusCodePermanentRedirect                 = 308, // 恒久的リダイレクト
    
    // 4xx Client Error クライアントエラー : クライアントからのリクエストに誤りがあった
    HTTPStatusCodeBadRequest                        = 400, // リクエストが不正である
    HTTPStatusCodeUnauthorized                      = 401, // 認証が必要である
    HTTPStatusCodePaymentRequired                   = 402, // 支払いが必要である
    HTTPStatusCodeForbidden                         = 403, // 禁止されている
    HTTPStatusCodeNotFound                          = 404, // 未検出
    HTTPStatusCodeMethodNotAllowed                  = 405, // 許可されていないメソッド
    HTTPStatusCodeNotAcceptable                     = 406, // 受理できない
    HTTPStatusCodeProxyAuthenticationRequired       = 407, // プロキシ認証が必要である
    HTTPStatusCodeRequestTimeout                    = 408, // リクエストタイムアウト
    HTTPStatusCodeConflict                          = 409, // 競合
    HTTPStatusCodeGone                              = 410, // 消滅した
    HTTPStatusCodeLengthRequired                    = 411, // 長さが必要
    HTTPStatusCodePreconditionFailed                = 412, // 前提条件で失敗した
    HTTPStatusCodePayloadTooLarge                   = 413, // ペイロードが大きすぎる
    HTTPStatusCodeURITooLong                        = 414, // URIが大きすぎる
    HTTPStatusCodeUnsupportedMediaType              = 415, // サポートしていないメディアタイプ
    HTTPStatusCodeRangeNotSatisfiable               = 416, // レンジは範囲外にある
    HTTPStatusCodeExpectationFailed                 = 417, // Expectヘッダによる拡張が失敗
    HTTPStatusCodeIamATeapot                        = 418, // 私はティーポット
    HTTPStatusCodeMisdirectedRequest                = 421, // 誤ったリクエスト
    HTTPStatusCodeUnprocessableEntity               = 422, // 処理できないエンティティ
    HTTPStatusCodeLocked                            = 423, // ロックされている
    HTTPStatusCodeFailedDependency                  = 424, // 依存関係で失敗
    HTTPStatusCodeUpgradeRequired                   = 426, // アップグレード要求
    HTTPStatusCodeUnavailableForLegalReasons        = 451, // 法的理由により利用不可
    
    // 5xx Server Error サーバエラー : サーバがリクエストの処理に失敗した
    HTTPStatusCodeInternalServerError               = 500, // サーバ内部エラー
    HTTPStatusCodeNotImplemented                    = 501, // 実装されていない
    HTTPStatusCodeBadGateway                        = 502, // 不正なゲートウェイ
    HTTPStatusCodeServiceUnavailable                = 503, // サービス利用不可
    HTTPStatusCodeGatewayTimeout                    = 504, // ゲートウェイタイムアウト
    HTTPStatusCodeHTTPVersionNotSupported           = 505, // サポートしていないHTTPバージョン
    HTTPStatusCodeVariantAlsoNegotiates             = 506,
    HTTPStatusCodeInsufficientStorage               = 507, // 容量不足
    HTTPStatusCodeLoopDetected                      = 508, // ループを検出
    HTTPStatusCodeBandwidthLimitExceeded            = 509, // 帯域幅制限超過
    HTTPStatusCodeNotExtended                       = 510  // 拡張できない
};
