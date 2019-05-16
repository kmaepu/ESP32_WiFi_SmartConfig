# ESP32_WiFi_SmartConfig

# 概要 
ESP32のWiFiクライアント（STA）にはSmartConfigという関数があり、これを使用するとスマートフォンの専用アプリからSSIDとパスワード設定ができます。

スマートフォンの専用アプリはいくつかあるようですが、今回はIoT SmartConfig(Android用)というアプリを使用しています。
![image.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/183282/3bd9415e-bfa3-ee28-9112-36e69c7866f0.png)
https://play.google.com/store/apps/details?id=com.iotmaker


# 環境
・スマートフォン：Android  
・対象デバイス：ESP32-DevkitC  
・IDE：Arduino IDE  

# 使い方
１．ESP32_WiFi_SmartConfig.inoをESP32に書き込む  
　　※シリアルコンソールを開いておく  
２．スマートフォンに「IoT SmartConfig」をインストールする  
３．ESP32が動作している状態で、IoT SmartConfigを起動する  
　↓起動後の画面  
<img width="187" alt="Screenshot_20190514-180252_IoT Smartconfig.jpg" src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/183282/cbb8cc0e-cd10-1a11-a7cc-687923b6b8ad.jpeg">

４．SSIDとパスワードを入力する  
 "unknown ssid"を消してSSIDを入力。  
　Password欄にパスワードを入力。  

５．Submitボタンを押す  
　ESP32のSSIDとパスワードの設定が開始されます。  

６．設定完了  
　設定が完了すると、IoT SmartConfigの画面に、ESP32のIPアドレスが表示されます。  

<img width="189" alt="Screenshot_20190515-124542_IoT Smartconfig.jpg" src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/183282/413614a8-f51e-0587-bc26-4bd24424d7a8.jpeg">

ESP32のシリアルコンソールに接続ログが表示されます。  
<img width="243" alt="シリアルコンソール画面.PNG" src="https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/183282/a05b0ad9-25a8-5e92-58a1-5ab72c69c2da.png">

# ライセンス
フリーライセンスです。  
