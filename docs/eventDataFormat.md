# イベントデータフォーマット
イベントデータのフォーマットを規定しています。

> **NOTE**: [全国イベント情報データベースAPIサービス] のデータ項目に準拠しています。（[サンプルデータ取得API]）

## データ項目

| 項目名称(ja) | 項目名称(en) | サンプルデータ |
|---|---|---|
|id|id|XXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX(UUIDv4)|
|タイトル|title|第１回目黒カレーフェスティバル|
|内容詳細|description|目黒の人気カレー屋４店舗が大集合！イベント限定メニューもご用意してお待ちしています。<br>開催時間は11時～20時です！ご家族でどうぞ！|
|カテゴリ|categories|グルメ、ファミリー|
|開催日程|eventDates|2020-04-4,2020-04-5,2020-4-11,2020-4-12|
|会場|site|Impact HUB Tokyo|
|住所|address|東京都目黒区目黒二丁目11-3|
|都道府県|prefecture|Tokyo|
|市区町村|municipality|目黒区|
|緯度|lat|35.6338465|
|経度|lng|139.7082072|
|画像URL|imgUrl|https://infomotion.co.jp/wp-content/uploads/2020/04/curry.jpg|
|参照URL|refUrl|https://infomotion.co.jp/sample-event|

## JSON フォーマット

```json
{
    "id": "A0E7CA6D-E568-4FED-8562-318E0620F47F",
    "title": "第１回目黒カレーフェスティバル",
    "description": "目黒の人気カレー屋４店舗が大集合！イベント限定メニューもご用意してお待ちしています。<br>開催時間は11時～20時です！ご家族でどうぞ！",
    "categories": [
        "グルメ",
        "ファミリー"
    ],
    "eventDates": [
        "2020-04-4",
        "2020-04-5",
        "2020-4-11",
        "2020-4-12"
    ],
    "site": "Impact HUB Tokyo",
    "address": "東京都目黒区目黒二丁目11-3",
    "prefecture": "Tokyo",
    "municipality": "目黒区",
    "lat": "35.6338465",
    "lng": "139.7082072",
    "imgUrl": "https://infomotion.co.jp/wp-content/uploads/2020/04/curry.jpg",
    "refUrl": "https://infomotion.co.jp/sample-event"
}
```


[全国イベント情報データベースAPIサービス]: https://infomotion.co.jp/event-api/
[サンプルデータ取得API]: https://rg-eventmap-func001.azurewebsites.net/api/event
