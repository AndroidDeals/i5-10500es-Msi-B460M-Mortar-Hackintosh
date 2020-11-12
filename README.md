# i5-10500es-Msi-B460M-Mortar-Hackintosh

日常自用EFI，有时候也直接搬运大佬的EFI用🤣，和我的配置一样使用就木有问题。🤣




<details>
  <summary>支持的系统版本</summary>
  
- macOS Catalina 10.15.7   
- ~~macOS Big Sur 11 Beta~~ 因退回10.15.x系统，暂不测试  


</details>


<hr>


## 硬件列表

|  配置     | 型号    |
|  :----:  | :----:  |
| CPU  | i5-10500ES |
| 主板  | 微星B460M 迫击炮 |
| 内存  | 阿斯加德 8G*2 |
| 固态  | 海力士啥型号叫不上 256G  |
| 显卡  | 映泰RX470独显 Intel UHD630核显  |
| 网卡  | 板载有线网卡+博通943602CS免驱网卡  |
| 电源  | 海盗船CX430（垃圾）  |


起初主板用的是昂达B460SD4，性价比超高。现换成微星B460M迫击炮😁，原因是昂达的BIOS太复杂，设置之后它自杀了，直接黑屏。所以千万不要去胡乱设置昂达的BIOS，以免造成不必要的麻烦。

[EFI下载地址](https://github.com/AndroidDeals/EFI/releases/)

1. 如果你的显示器是高分辨率，那么NVRAM→UIScale 数值改为02 开机苹果logo就会正常比例显示，否则很小很小。1080p值为01。
2. 跑码模式 NVRAM→boot-args 里面 加 -v即可，根据需要调整。


- 测试可用的功能

```diff
- 如果你使用了免驱网卡，切记一定一定一定要关闭BIOS里面的USB唤醒,否则睡眠秒唤醒。
```
 - [x] 睡眠/唤醒 `唤醒需要按电源键`  
 - [x] 核显硬件加速 `完全支持，不行请调整自己的缓冲帧`
 - [x] 板载声卡 `测试可用`
 - [x] 板载USB端口 `板载USB端口测试都可以用，机箱USB接口最好自己定制`
 
- 未测试的功能 
 - [ ] 板载网卡 `因为用的免驱无线网卡，就没有测试板载有线网卡`





## 部分图片仅供参考

* 关于本机
![关于本机](https://raw.githubusercontent.com/AndroidDeals/i510500es-MSIB460m-Mortar-Hackintosh/master/screenshots/1.png)

* 双显卡识别
![双显卡识别](https://raw.githubusercontent.com/AndroidDeals/i510500es-MSIB460m-Mortar-Hackintosh/master/screenshots/2.png)

* 硬件加速ok的
![硬件加速ok的](https://raw.githubusercontent.com/AndroidDeals/i510500es-MSIB460m-Mortar-Hackintosh/master/screenshots/3.png)

* 各硬件信息
![各硬件信息](https://raw.githubusercontent.com/AndroidDeals/i510500es-MSIB460m-Mortar-Hackintosh/master/screenshots/4.png)


* CPU跑分
![CPU跑分](https://raw.githubusercontent.com/AndroidDeals/i510500es-MSIB460m-Mortar-Hackintosh/master/screenshots/cpu.png)

* LuxMark跑分
![LuxMark跑分](https://raw.githubusercontent.com/AndroidDeals/i510500es-MSIB460m-Mortar-Hackintosh/master/screenshots/lux.png)
