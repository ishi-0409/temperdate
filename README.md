# temperdate
raspberrypiで取得した気温データをfirebaseに保存できる

またfirebaseに保存した気温データをスプレッドシートに送ることができる

スプレッドシート上でグラフを作成し、データの可視化が可能

## デモ動画

[![Temperate Demo](https://img.youtube.com/vi/ChFbGno3DfQ/0.jpg)](https://www.youtube.com/watch?v=ChFbGno3DfQ)


動画内では気温データを取得→firebaseにデータが保存されている様子→スプレッドシートに蓄積したデータを送る→送ったデータが反映される様子が確認できる

## 気温データのグラフ

![説明文](images/https://github.com/ishi-0409/temperdate/blob/main/Temperature%20%E3%81%A8%20Humidity.png)


## メモ

データを取得してfirebaseにおくるのはtemperdate.py  

firebaseのデータをスプレッドシートに出力するのはtempergraph.py

tempeartureに入る

firebaseの鍵はtemperIot3.json

スプレッドシートの鍵はtempergraph.json

temperdate.py と tempergraph.py　は別のターミナルで実行　

temperslack.py　を別のターミナルで実行することでslackからの通知も可能
