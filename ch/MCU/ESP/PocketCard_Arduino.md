#### 1. 先下載Arduino IDE工具： 

  請至 https://www.arduino.cc/en/Main/Software 網站下載

#### 2. 安裝USB to UART 驅動程式

  請至http://www.wch.cn/download/CH341SER_ZIP.html

  安裝完驅動程式插入PocketCard，在裝置管理員中會出現新的COM 埠

  <img src="images/00000.jpg" alt="00000" style="zoom:67%;" />

#### 3. 安裝ESP32核心檔案

  啟動 Arduino IDE 並點擊下拉功能表「File」>「Preferences」。

  <img src="images/00001.jpg" alt="00001" style="zoom: 50%;" />

  Additional Boards Manager URLs：

  輸入 https://dl.espressif.com/dl/package_esp32_index.json

  然後點擊「OK」鈕。

  <img src="images/00002.jpg" alt="00002" style="zoom: 67%;" />

  點擊下拉功能表「Tools」>「Board」>

  「Board Manager...」

  <img src="images/00003.jpg" alt="00003" style="zoom:67%;" />

  在 Type 右方空白欄位輸入「esp32」

  點擊「Install」，然後等待幾分鐘下載完畢後點擊右下角落的「Close」鈕關閉視窗。 

  <img src="images/00004.jpg" alt="00004" style="zoom: 67%;" />

#### 4. 複製 Libraries

  請至https://github.com/kaise-ksrobot/pocketcard_arduino_demo

  點選Download ZIP 下載檔案

![00006](images/00006.jpg)

  解壓後把 pocketcard_arduino_demo/libraries 目錄中的檔案Copy 到 Arduino IDE/libraries

  Arduino IDE/libraries 目錄中會多出5個目錄

  <img src="images/00007.jpg" alt="00007" style="zoom:67%;" />

#### 5. 選擇 開發板和連接埠

  點擊下拉功能表「Tools」>「Board」，

  選擇「NodeMCU-32s」

  <img src="images/00005.jpg" alt="00005" style="zoom:67%;" />

  然後再選擇連接埠

  <img src="images/00008.jpg" alt="00008" style="zoom:67%;" />

#### 6. 執行 Demo Code

  打開Arduino IDE/libraries/PocketCard/examples/pocketcard_demo/pocketcard_demo.ino

  <img src="images/00009.jpg" alt="00009" style="zoom:67%;" />

  下載成功後，會聽到蜂鳴器響一聲，Oled 面板會出現 “Hello, world” 再滅掉

  按A鍵 會出現Light Sensor(A) 和Light Sensor(B ) 和Temperature Sensor 的數值

  按B鍵 會出現MPU9250的偵測數值。

  <img src="images/00010.jpg" alt="00010" style="zoom:67%;" />

  <img src="images/00011.jpg" alt="00011" style="zoom:67%;" />