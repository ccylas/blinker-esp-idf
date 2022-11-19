# blinker-esp-idf
An IoT Solution,Blinker library for embedded hardware. Works with ESP8266, ESP32 (idf)  

Supprot ESP-IDF

stable version support:  
- [ESP8266_RTOS_SDK v3.4](https://github.com/espressif/ESP8266_RTOS_SDK/releases/tag/v3.4)  
- [ESP_IDF v4.3/v4.4](https://dl.espressif.cn/dl/esp-idf/?idf=4.4)  

# TODO  
- BLINKER_PRO_ESP OTA support  

# Blinker hello example  

put the blinker componets into your projects.

make the project list like this  
```
Blinker_Hello
  |__components
  |  |__blinker
  |__main
```

override the esp_http_server components with we provide.

```
idf.py menuconfig
```

enter Blinker Config  

* set BLINKER DEVICE TYPE

* set BLINKER AUTH KEY  

* set Provisioning Type  

save and exit blinker config  

* Set Serial Flasher Options.  

enter components config  

* enable mDNS  

* disable Newlib  

* enable webSocket server support(http_server)  

save and exit

## Build and Flash  

Build the project and flash it to the board, then run monitor tool to view serial output:

```
idf.py -p PORT flash monitor
```  
