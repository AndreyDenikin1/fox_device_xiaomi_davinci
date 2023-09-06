![OFRP](https://i.ibb.co/4WgF7pR/banner-2.png "OFRP")

OrangeFox Recovery Project (OFRP) R11.x for Xiaomi Redmi K20 / Mi 9T

# How to build
Check OFRP official guide https://wiki.orangefox.tech/en/dev/building

## Features

Works:

- ADB
- Screen brightness settings
- Correct screenshot color
- MTP
- Flashing (opengapps, roms, images and so on)
- Backup/Restore
- USB OTG
- Android T Support
- Vibration support
- Decryption of /data (policy V1)

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Dual-core 2.2 GHz Kryo 470 Gold & Hexa-core 1.8 GHz Kryo 470 Silver
Chipset | Qualcomm Snapdragon 730 (SM7150-AA)
GPU     | Adreno 618
Memory  | 6 GB RAM
Shipped Android Version | 9.0
Storage | 64/128 GB (UFS 2.0)
Battery | Non-removable Li-Po 4000 mAh
Display | 1080 x 2340 pixels, 6.39 inches (~428 ppi pixel density)
Camera  | 48MP wide camera, 8MP telephoto camera, 13MP ultra wide-angle camera

## Device picture

![Xiaomi Mi 9T/Redmi K20](https://i01.appmifile.com/webfile/globalimg/products/pc/redmik20/index_slider_1.png "Xiaomi Mi 9T/Redmi K20 in carbon black")

Finally execute these:

```
source build/envsetup.sh
lunch twrp_davinci-eng
mka adbd recoveryimage
```

To flash it:

```
fastboot flash recovery out/target/product/davinci/recovery.img
```

