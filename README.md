# usbcan-2a

There are different hardware versions.

I have a V10 (possibly V1.0)
- stm32f405rgt6
- ![image](https://user-images.githubusercontent.com/202906/206101957-122900dd-355b-4a2c-a94b-1589caf2a225.png)
![20221205_135431](https://user-images.githubusercontent.com/202906/206123658-cdc6560a-6f11-4b73-b314-c40d167faf52.jpg)

```

  Power LED - PA5 to VDD via 1K  

  - CAN1
    CAN1_RX  PB8(61) 
    CAN1_TX  PB9(62)
    CAN1_LED PC14 (3) to VDD via 1K  
 
  - CAN2
    CAN2_RX  PB12(33)   
    CAN2_TX  PB13(34)  
    CAN2_LED PC13 (2) to VDD via 1K  

  - USB   
    OTG_HS_DM (35)
    OTG_HS_DP (36)
    

2 pin header
  1  PB6 (58)
  2  PB7 (59)
  
5 Pin header 
    1 JTMS-SWDIO (46)
    2 JTCK-SWCLK (49) 
    3 NRST (7)
    4 VDD 3.3V (48,64) 
    5 GND (12) VSSA 
``` 
- VDD
  32/19/
  
- BOOTP (60) - pulled high R4 (1002) resistor  
  
` 
'
 
This is a differnet version:
file:///home/dan/Downloads/stm32f405rg.pdf

PA14/PA15  CAN2 RX/TX
BOOT0 - to 5V via 1002? 

![Canbox_pinout](https://user-images.githubusercontent.com/202906/206101834-f6d3da47-ff25-47eb-8c5c-5ccb53f401a9.png)

Fedora STMCube 

```
cd  /usr/lib64/
sudo ln -s libncurses.so.6 libncurses.so.5
sudo ln -s libtinfo.so.6 libtinfo.so.5
```

