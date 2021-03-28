最近有项目用到ESP32，顺便记录一下。  
首先在电脑上安装arduino、Git和python等工具，安装软件部分就不再过多阐述。  

1\. 给Arduino IDE添加开发板网址  
打开IDE，打开文件-\>首选项，如图  

在这里插入图片描述  
找到==附加开发板管理器网址，在新弹出的窗口中添加以下网址：  
https://git.oschina.net/dfrobot/FireBeetle-ESP32/raw/master/package_esp32_index.json

https://dl.espressif.com/dl/package_esp32_index.json  

或者到以下网址中找到对应的开发板网址，自行添加  
https://github.com/arduino/Arduino/wiki/Unofficial-list-of-3rd-party-boards-support-urls


如图：  
在这里插入图片描述  

2.更新开发板列表  
我们将ESP32开发板的网址添加到IDE后，还需要更新以下开发板列表，让IDE下载相应的支持库和文件。


打开工具-\>开发板-\>开发板管理  

在这里插入图片描述  

在打开开发板管理器之后，管理器会自动加载更新开发板列表，找到对应的ESP32开发板点击安装即可


3.使用IDE编译和下载固件  
找到对应的开发板，根据开发板设置对应的参数  

在这里插入图片描述  

打开文件-\>示例-\>ESP32-\>xxx找个自己感兴趣的项目并打开  
by the
way:一定要按照以上流程先安装ESP32开发板的支持库，不然你是找不到ESP32例程和开发板设置的


在这里插入图片描述  
在这里插入图片描述  

点击上传，然后按照指示
点击开发板的BOOT按键进行下载，点击串口监视器，打印出ESP32芯片的ID
