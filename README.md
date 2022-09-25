# IoT_camera

Motivation
　自分が住んでいるアパートのセキュリティに不安を感じ、外出先や家の中からも玄関に不審者がいないかを確認できるシステムが欲しいと考え開発した。

purpose
　　ーRaspberryPi3 とライブラリにあるOpenCV、Webカメラを使用し、撮影している映像に変化があった場合に検知される、動体検知カメラを作成する。
 ー撮影された映像がインターネットを軽有して（LINE Notify）を使用し,LINEに通知が来るようにする。

Functional spec
　　ーモニターには撮影した映像と時刻を表示。また、動きを検知した場合のピクセル値を表示 
 ー OpenCVを使い物体が検知されればJPEG形式で保存 
 ー 保存されLINE上に送信される画像にも日付、時刻、ピクセル値を表示

Creative points in My work
　　ー 画像の閾値に輪郭線を入れることで変化がわかりやすく見やすくした。 
 ー 保存される画像が容量いっぱいにならないようPCのローカルディスクは上書きされるようにした点、しかしLINE上で送信される画像は物体が動き保存された画像全てを通知する点
 
 モニターの映像
 
 　　


![図1](https://user-images.githubusercontent.com/87026230/192127961-3b32e536-ea7b-41ea-8c0e-e24f05f2fea4.jpg)
![図1 (1)](https://user-images.githubusercontent.com/87026230/192127973-3c128ac9-e6b3-425a-ab02-7013b6349083.jpg)
