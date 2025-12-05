
<div align="right">
  <details>
    <summary >🌐 Language</summary>
    <div>
      <div align="center">
        <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=en">English</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=zh-CN">简体中文</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=zh-TW">繁體中文</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=ja">日本語</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=ko">한국어</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=hi">हिन्दी</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=th">ไทย</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=fr">Français</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=de">Deutsch</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=es">Español</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=it">Italiano</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=ru">Русский</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=pt">Português</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=nl">Nederlands</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=pl">Polski</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=ar">العربية</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=fa">فارسی</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=tr">Türkçe</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=vi">Tiếng Việt</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=id">Bahasa Indonesia</a>
        | <a href="https://openaitx.github.io/view.html?user=xyzroe&project=ZigStarGW-MT&lang=as">অসমীয়া</
      </div>
    </div>
  </details>
</div>

# ZigStar GW Multi tool
[![Build](https://github.com/xyzroe/ZigStarGW-MT/actions/workflows/build.yml/badge.svg)](https://github.com/xyzroe/ZigStarGW-MT/actions/workflows/build.yml)
[![GitHub version](https://img.shields.io/github/release/xyzroe/ZigStarGW-MT.svg)](https://github.com/xyzroe/ZigStarGW-MT/releases)
[![GitHub download](https://img.shields.io/github/downloads/xyzroe/ZigStarGW-MT/total.svg)](https://github.com/xyzroe/ZigStarGW-MT/latest)
[![License](https://img.shields.io/github/license/xyzroe/ZigStarGW-MT.svg)](LICENSE.txt)


> ⚠️ **ARCHIVED / UNMAINTAINED**
>
> This project is now archived and will not receive further updates.
> 
> I kindly invite you to try the new web-based tool [XZG Multi-Tool](https://github.com/xyzroe/XZG-MT), which offers improved functionality and ongoing support. 🚀

  
is GUI wrapper firtsly designed for convenient service work with  Zig Star LAN GW  
but now supports any TI CC1352/CC2538/CC2652 based Zigbee sticks or gateways, regardless of the manufacturer. 

Multi tool is packed into single executable file.  
You can get started without installing Python and the required modules, and without using the terminal, - just download and run.

## Possibilities:
- Read / Write / Erase NVRAM memory of Zigbee module
- Write / Verify / Erase firmware of Zigbee module
- Backdoor Serial Loader turns on automatically
- Manual restart of  Zigbee module or ESP32 is available

#### Screenshots

<table>
<tr> 
<td width="50%">

##### Windows
<img src="https://github.com/xyzroe/ZigStarGW-MT/raw/main/images/win.png">
</td>
<td>

##### OS X
<img src="https://github.com/xyzroe/ZigStarGW-MT/raw/main/images/osx.png">
</td>
</tr>
</table>

## Instructions:
### 1. Identify Port
#### Network gateways:
If you are using ZigStar LAN GW, the IP address will be detected automatically, otherwise enter the IP:PORT of your gateway.
#### USB sticks:
Click the update button to identify the USB drive and select your device from the dropdown list.
<br>  
<div align="center"><img src="https://zig-star.com/images/radio-docs/multitool/multitool-1.png"></div>


### 2.A Firmware update
- Choose firmware *.hex file on your disk.
- Choose required options. Usually is Erase, Write and Verify.
- If you need to change the IEEE address, type it in and set checkbox Write IEEE.
- Press the "Start" button to begin the selected processes.

If any action is performed on the right side of the Multi Tool, the primary IEEE address is placed in the corresponding field. (Replacing manual entered or previously read one)

*For gateways or USB sticks other than ZigStar, you may need to manually enable BSL.  
Also, if you are using a non ZigStar gateway, you need to uncheck the Auto-BSL checkbox.*
<br>  
<div align="center"><img src="https://zig-star.com/images/radio-docs/multitool/multitool-2.png"></div>


### 2.B NVRAM Tools
If you have any troubles with Zigbee network NVRAM tool may help you.

- **Read** button saves *.json file on your disk with current NVRAM state of your Zigbee module for future restore.
- **Write** button reads *.json file from your disk with saved NVRAM state and write it to your Zigbee module.
- **Erase** button cleans your Zigbee module NVRAM for a fresh install.
<div align="center"><img src="https://zig-star.com/images/radio-docs/multitool/multitool-3.png"></div>

### Like ♥️?
[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/xyzroe)


### Based on
[zigpy/zigpy-znp](https://github.com/zigpy/zigpy-znp)  
[JelmerT/cc2538-bsl](https://github.com/JelmerT/cc2538-bsl)  

  

<br>  

xyzroe/ZigStarGW-MT is licensed under the  
##### [GNU General Public License v3.0](https://github.com/xyzroe/ZigStarGW-MT/blob/main/LICENSE)
