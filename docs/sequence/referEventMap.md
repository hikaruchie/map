# 処理フロー：マップ表示

## 凡例
- 実線： リクエスト を表します。
- 破線： レスポンス を表します。
- par： 並列処理 を表します。
- alt： 分岐処理 を表します。

----

```mermaid
sequenceDiagram
  autonumber
  actor ブラウザ

  ブラウザ ->> Static Web Apps: /(ルート) の呼び出し
  Note right of ブラウザ: GET /index.html<br>クエリパラメータ無し

  par マップ情報取得
    Static Web Apps->>Google Maps API: Hello guys!
    Google Maps API-->>Static Web Apps: Hello guys!
  and イベント情報取得
    Static Web Apps ->> Cosmos DB: イベント情報の呼び出し
    Note right of Static Web Apps: GET /events<br>クエリパラメータ無し
    Cosmos DB -->> Static Web Apps: イベント情報の返却
    Note right of Cosmos DB: データ項目<br>eventDataFormat.md
  end

  Static Web Apps -->> ブラウザ: イベント情報付き<br>マップ情報 (html,js) を返却
```