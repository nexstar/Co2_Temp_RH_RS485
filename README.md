##Co2-Temp-RH(二氧化碳計)

# 介紹 #

### 二氧化碳是甚麼? ###

二氧化碳（IUPAC名：carbon dioxide，分子式：CO2）是空氣中常見的化合物，由兩個氧原子與一個碳原子通過共價鍵連接而成。空氣中有微量的二氧化碳，約佔0.04％。二氧化碳略溶於水中，形成碳酸，碳酸是一種弱酸。

二氧化碳是無色的。在低濃度時，二氧化碳氣體是無味的，但在較高濃度時會有酸性氣味，它可造成窒息和刺激。當吸入濃度比大氣層平常濃度高很多的二氧化碳時，它會產生一種酸的味道和鼻子和喉嚨產生刺痛感，氣體溶解在黏膜和唾液中，產生了碳酸。

### 為什麼要使用二氧化碳計? ###

因現代人待在室內的時間比外出時間較長,如再加上天氣的炎熱就更不可能外出,長時間的待在室內Co2就濃度慢慢提升(不通風下)。

Co2的濃度會影響人類的判斷,濃度低於1000PPM比較感受不到任何狀態,1000PPM以上就可能造成嗜睡、頭暈、精神不集中等狀態，如果PPM繼續往上突破2000或3000基本上可能造人類身體很大的狀況。

Co2嚴重可能造成人類的死亡(有可能的),所以預防此事情發生,**二氧化碳計**是偵測室內Co2與濕度和溫度三大指標,用於警示使用者,不然嚴重的情形可能造成無可避免的生命安全。

## 執行方式
1. 此程式採取多台使用,不管如何都要更改資料
2. 先安裝2007Access套件(AccessDatabaseEngine)<br>
3. 接下來進行Access的修改(1.ComPort,2.TabPosMap中DeviceID(機器上也要特定修改),3.TabSetting( ErrorLog 路徑位置))<br>
   如有需更改Timer Speed(TabSetting)
4. 修改機器中DeviceID與Access中ID相同<br>
5. 以上完成,可執行程式Exe<br>

##匯出資料
原始系統是匯出Json與html格式,ErrorLog,(如果不需要可以直接做刪除 )

##查看是否正常
1.下載Simply Modbus Master 8.0.3( 快速檢測 )<br>
2.觀看Access是否寫入TabEVO的Table中,有看到資料就表示成功

# 硬體設備 #

- 二氧化碳計(TE-701R) x 1 ( 多台執行也可 )
![1](https://github.com/nexstar/Co2_Temp_RH_RS485/raw/master/Picture/DevicePicture.PNG)
- RS485 x 1 ( 多台也需一條線 )

##Main

程式一執行就直接啟動(預設5秒會觸動Trigger)<br>
![1](https://github.com/nexstar/Co2_Temp_RH_RS485/raw/master/Picture/Main.PNG)

### 圖片: ###

### Access修改: ###
修改AccessPath<br>
![P4](https://github.com/nexstar/Co2_Temp_RH_RS485/raw/master/Picture/AccessPath.PNG)

修改Device<br>
![P4](https://github.com/nexstar/Co2_Temp_RH_RS485/raw/master/Picture/Device.PNG)

# Reference #

- [雙儀科技儀器-R1](http://www.twintex.com.tw/proimages/pic/IAQ_PHOTO/TE-701R.jpg)
- [CO2-Wiki](https://goo.gl/i36OWo)

# 製作者 #

NianBaoZou	( nexstar@gmail.com )<br>
6/15/2016 9:30:01 PM 