# temperdate
raspberrypiで取得した気温データをfirebaseに保存できる

またfirebaseに保存した気温データをスプレッドシートに送ることができる

スプレッドシート上でグラフを作成し、データの可視化が可能

## デモ動画

[![Temperate Demo](https://img.youtube.com/vi/ChFbGno3DfQ/0.jpg)](https://www.youtube.com/watch?v=ChFbGno3DfQ)


動画内では気温データを取得→firebaseにデータが保存されている様子→スプレッドシートに蓄積したデータを送る→送ったデータが反映される様子が確認できる

## 気温データのグラフ

![Temperature と Humidity グラフ](https://raw.githubusercontent.com/ishi-0409/temperdate/main/Temperature%20%E3%81%A8%20Humidity.png)

実際に数時間データを取り続け、スプレッドシートに出力されたデータをもとにグラフを作成し、データを可視化することができる

## メモ

データを取得してfirebaseにおくるのはtemperdate.py  

firebaseのデータをスプレッドシートに出力するのはtempergraph.py

tempeartureに入る

firebaseの鍵はtemperIot3.json

スプレッドシートの鍵はtempergraph.json

temperdate.py と tempergraph.py　は別のターミナルで実行　

temperslack.py　を別のターミナルで実行することでslackからの通知も可能

スプレッドシートに出力された日時は文字として出力されているので数値におきかえる関数を挟む必要がある

関数自体はちがうシートのa1に書かれているため、それをコピペしてd2のセルに張り付けると日時の詳細設定を反映させることができる
