# For MicroPyhton

安裝好python3的環境

如果還沒有安裝 USB to UART 驅動程式的請先看 Arduino的使用



#### 1. 安裝燒錄工具

https://github.com/espressif/esptool



`pip3 install esptool` 

完畢後檢視 Python 安裝目錄的 Scripts 資料夾, 會發現多了幾個 esp 開頭的檔案, 其中的 esptool.py 或 esptool.exe 就是我們要用來清除 flash 以及燒錄韌體的程式. 如果安裝 Python 時有勾選自動加入 path 環境變數, 那麼在任何目錄下都可執行 esptool.exe



#### 2. 燒錄ESP32 micropython的韌體

http://micropython.org/download/esp32/



COM埠請依照 裝置管理員 的訊息設定比如 com8

先把整個Flash 清空

`esptool.exe --chip esp32 --port com8 erase_flash`

再燒錄你選擇的韌體比如 esp32-idf3-20191220-v1.12.bin

`esptool.exe --chip esp32 --port COM8 --baud 460800 write_flash -z 0x1000 esp32-idf3-20191220-v1.12.bin`



#### 3. ESP32 micropython 基本指令操作

ESP32 micropython的基本指令操作(英文)

https://docs.micropython.org/en/latest/esp32/quickref.html

ESP32 micropython的基本指令操作(簡體中文)

http://docs.micropython.01studio.org/zh_CN/latest/esp32/quickref.html

