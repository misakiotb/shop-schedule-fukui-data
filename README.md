# shop-schedule-fukui-data
福井のお店の営業時間データ
## データ
* 2024-25 年末年始営業時間データ :  [shop-schedule-fukui_2024-25.csv](./shop-schedule-fukui_2024-25.csv)
## ファイルフォーマット
UTF-8、BOMあり、改行コードCR+LF、csv
## スキーマ
```
店舗,URL,緯度経度,Geo3x3,2024/12/29 OPEN,2024/12/29 CLOSE,2024/12/30 OPEN,2024/12/30 CLOSE,2024/12/31 OPEN,2024/12/31 CLOSE,2025/1/1 OPEN,2025/1/1 CLOSE,2025/1/2 OPEN,2025/1/2 CLOSE,2025/1/3 OPEN,2025/1/3 CLOSE,2025/1/4 OPEN,2025/1/4 CLOSE
```
経度緯度、Geo3x3 はこちらを利用させていただきました https://fukuno.jig.jp/app/map/latlng/
### 課題
* OPENとCLOSEは時刻のみにしたかったが、通常営業を空欄で表した場合、休業はテキストがわかりやすかったためテキストにした
* 日付とOPEN/CLOSEがカラム方向に並び、DBとしては正規化していない
## 掲載基準
* 福井県嶺北エリア、特に福井市と丹南エリアを中心に
* 年末年始に人が集まりそうなショッピングモールを中心に
## データ収集方法
* 各社Webサイトより。出典はデータ内にURL記載
