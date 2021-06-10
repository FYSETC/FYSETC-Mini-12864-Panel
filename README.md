# Mini-12864-Panel

## Product Introduction


![Mini12864](images/Mini12864.png)

这是一个便宜，带RGB指示灯，通用于marlin的显示屏，支持脱机打印，分辨率为12864，显示区域为2.4’‘，SD卡座可以为侧式或者立式，方便不同的安装场合，非常适用于小型3D打印机。

This is a opensouce, cheap, with RGB indicator, common to marlin's display, supports offline printing, resolution is 12864, display area is 2.4'', SD card holder can be side or vertical, convenient for different installation occasions Ideal for small 3D printers.

There are two versions, one with only two RGB LEDs around the encoder, the backlight is fixed color; the other one backlight is also RGB.

## Features

- 2.4" inch high contrast Graphic LCD
- Black-gray/black-green/white-black/white-blue/green-black, 5 display styles
- SPI communication to host micro-controller
- Support Vertical or side SD slot with card detect
- Rotary Encoder 
- Configurable RGB LED light
- Software configurable contrast setting
- 3D printable case and mount STL file 
- EXP1 & EXP2  RAMPS Compatible socket



## Application

3D printer，CNC machines ，Other micro controller projects



## Typical  Wiring
![](images/Mini12864-bottom.svg)

![](images/Mini12864-EXP1.svg)

![](images/Mini12864-EXP2.svg)



## 注意/NOTICE：

| SCH                                                | Description                                                  |
| -------------------------------------------------- | ------------------------------------------------------------ |
| <img src="images/notice.png" style="zoom:600%;" /> | 为了兼容某些主板，如RAMPS1.4，FYSETC mini12864 设置了 RST(R3) 和 KILL(R4) 的可选择电阻。目前，有些主板（S6/Spider）将 KILL 换成 5V，此时，请确认 mini12864 上 R4处于空贴状态，否则按下屏幕上的按钮会致使 5V 与 GND 短路，长时间操作会导致主板损坏。<br/>   In order to be compatible with some motherboards, such as RAMPS1.4, mini12864 is equipped with RST (R3) and KILL (R4) optional resistors. At present, some motherboards (S6/Spider) change the KILL to 5V. At this time, please make sure that R4 on the mini12864 is in the empty state, otherwise pressing the button on the screen will cause a short circuit between 5V and GND, and long-term operation will cause the motherboard to be damaged. |

## Firmware config

### Marlin

Uncomment the following define according to your panel version, you can check it at the back of the panel.

```
//
// FYSETC variant of the MINI12864 graphic controller with SD support
// https://wiki.fysetc.com/Mini12864_Panel/
//
//#define FYSETC_MINI_12864_X_X    // Type C/D/E/F. No tunable RGB Backlight by default
//#define FYSETC_MINI_12864_1_2    // Type C/D/E/F. Simple RGB Backlight (always on)
//#define FYSETC_MINI_12864_2_0    // Type A/B. Discreet RGB Backlight
//#define FYSETC_MINI_12864_2_1  // Type A/B. Neopixel RGB Backlight
//#define FYSETC_GENERIC_12864_1_1 // Larger display with basic ON/OFF backlight.
```

## Attention

-TBD-

## FAQ

-TBD-


## Attachments
### 1. Schematic

---------

![](images/mini12864_sch.png)



### 2. Dimensions

---------

![](images/mini12864_dim.png)

**For detailed dimensions please check dwg/step file on github.**

## Shop
---
- [LCD](  )

## Tech Support
---
Please submit any technical issue into our [forum](http://forum.fysetc.com/) 


```

```