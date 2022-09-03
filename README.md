# 8051_buck_converter
由於在碩一修讀電力電子這門課時，我發現DC to DC電源轉換器，很多是用類比的方式來進行控制。所以這個專案我是想嘗試，透過微處理器的方式來進行控制，是否也能有不錯的效果。這邊使用8051的MCU，來進行控制Buck converter，以及透過LCD顯示器顯示降壓後的輸出電壓、PWM Duty Cycle。
## Project Description
下方為此專案的硬體配置，使用8051對下方麵包版Buck converter電路進行控制，以及透過UART接收另外一台微處理器量測到的電壓資訊，並將電壓資訊、Duty cycle顯示在LCD顯示屏上。

![image](https://github.com/ZongWeiLin/8051_buck_converter/blob/main/Setup.png)

## Files
* Project.c
  * 中斷、計時器、UART初始化設定
  * PWM操作、UART通訊
* LCM.h
  * LCD顯示器函式庫
* regx51.h
  * 8051標準函式庫

  
