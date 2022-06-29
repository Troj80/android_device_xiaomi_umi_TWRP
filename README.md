![TWRP](https://i.ibb.co/BfQqn97/TWRP-logo-banner-1.jpg "TWRP")

TeamWin Recovery Project (TWRP) R12 for Xiaomi Mi 10 5G (umi)
======================================

Kernel and all blobs are extracted from [miui_CMI_21.9.17_1c6ed0daa1_11.0.zip](https://hugeota.d.miui.com/21.9.17/miui_CMI_21.9.17_1c6ed0daa1_11.0.zip) firmware.

# How to build
Download TWRP's source and umi's repos. Your local manifest(.repo/manifest.xml) should be something like:

```bash
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

<!-- Device tree -->
    <project name="alextroj/android_device_xiaomi_umi_TWRP" path="device/xiaomi/umi" remote="github" revision="android-12.1" />

<!-- QCOM decryption -->
  <project name="TeamWin/android_device_qcom_twrp-common" path="device/qcom/twrp-common" remote="github" revision="android-12.1"/>
</manifest>
```

Then go to the source folder and run:

```bash
. build/envsetup.sh && lunch omni_umi-eng && mka recoveryimage
```

Device configuration for Xiaomi Mi 10 5G
=========================================

The Xiaomi MI 10 (codenamed _"umi"_) is a high-end smartphone from Xiaomi.

It was announced on February 2020. Release date was February 2020.

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
SoC     | Qualcomm SDM865 Snapdragon 865
CPU     | Octa-core (2.84 GHz Kryo 485 & 2.42GHz Kryo 485 & 1.8GHz Kryo 485)
GPU     | Adreno 650
Memory  | 6/8 GB RAM
Shipped Android Version | 10.0 with MIUI 11
Storage | 128/256 GB
Battery | Non-removable Li-Po 4500 mAh battery
Display | 1080 x 2340 pixels, 19.5:9 ratio, 6.67 inches, AMOLED HDR10+
Camera  | 108MP(Primary) 20MP(Ultra-wide) 12MP(Telephoto 2x Optical Zoom) 8MP(Telephoto 5x Hybrid zoom)

## Device picture

![Xiaomi MI 10 5G ](https://fdn2.gsmarena.com/vv/pics/xiaomi/xiaomi-mi-10-pro-5g-1.jpg "Xiaomi MI 10 5G")
