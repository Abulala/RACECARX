# RACECAR/X
1:10 autonomous RC robocar that is controlled by NVIDIA AGX Xavier.

Inspired by
* [MIT racecar](https://mit-racecar.github.io/)
* [Hypha-ROS racecar](https://github.com/Hypha-ROS/hypharos_racecar)
* [Racecar/J](https://racecarj.com/)
* [F1/10 Autonomous Racing Competition](http://f1tenth.org/)
* [Jetson racecar](https://www.jetsonhacks.com/category/robotics/jetson-racecar/)
* [eagleMK4](https://github.com/r7vme/eagleMK4)
* 


# Components

| Component | Where to buy | Specifications | Comments |
| --------- | ----- | -------- |
| 1:10 Race Car chassis | 499,95€ [TRAXXAS Slash 4x4 Platinum](http://mobil.rc-race-shop.de/item/5452583638303452)  | [TRAXXAS Slash 4x4 Platinum, Model 6804R](https://traxxas.com/sites/default/files/6804RAD-EN-R01-Slash%204x4%20Platinum.pdf) | only chassis and brushless motor are used.|
| 2 x LiPo battery 3S | 2 x 23,28 €  [ZIPPY Flightmax 5000mAh 3S1P 20C](https://hobbyking.com/de_de/zippy-flightmax-5000mah-3s1p-20c.html) | [ZIPPY Flightmax 5000mAh 3S1P 20C](https://hobbyking.com/de_de/zippy-flightmax-5000mah-3s1p-20c.html) | One for car, one for Jetson |
| 2 x LiPo voltage checker | 2 x 1,86€ [lipo voltage checker](https://hobbyking.com/de_de/hobbykingtm-lipo-voltage-checker-2s-8s.html) | |
| Compute module  | 1349,00€ [Nvidia Jetson AGX Xavier Development Kit](https://developer.nvidia.com/embedded/buy/jetson-xavier-devkit) | [User Guide](https://developer.download.nvidia.com/assets/embedded/secure/jetson/xavier/docs/jetson_agx_xavier_developer_kit_user_guide.pdf?w6FwPGkCOGk8zmp_TtxbrB3NlTQe9kdVe754dWbLbU_RVjNUNoRRqd41lYs033mXuYb3zYRBxpd2hchWrMdkXRWqkMgYo9I8DGAO5at5-wlfPvd2gKjvjbHEVQpHcmbL5-IhftVEo0Lqn10rXsUPy_jAqJsH-NmbfH_lUGC7367K1er-FVnDjCkQZ7xR6X_SX8EM3mclng) [Nvidia Forum](https://devtalk.nvidia.com/default/topic/1039020/jetson-agx-xavier/links-to-jetson-xavier-resources-amp-wiki/) [Documentation](https://developer.nvidia.com/embedded/downloads#?search=Jetson%20AGX%20Xavier) [FAQ](https://developer.nvidia.com/embedded/faq#xavier-faq) [Technical Blog](https://devblogs.nvidia.com/nvidia-jetson-agx-xavier-32-teraops-ai-robotics/?ncid=so-fac-mdjngxxrmllhml-69163)| register for the Nvidia developmenter program for special discount. |
| ESC | 159,00€ [Enertion FOCBOX](https://electricboardsolutions.com/products/enertion-focbox)| [VESC Project](https://vesc-project.com/documentation) | alternative: [Turnigy SK8-ESC V4.12](https://hobbyking.com/de_de/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html)|
| Battery adapter | 3,60€ [HXT 4mm bis XT-60 Batterie-Adapter](https://hobbyking.com/de_de/hxt-4mm-to-xt-60-battery-adapter-2pcs-bag.html) | | required to connect FOCBOX with Zippy Lipo |
| SSD |  134,86€  [Samsung 970 EVO 500GB, M2 2280](https://www.amazon.de/dp/B07CGGP7SV/ref=pe_3044161_189395811_TE_SCE_dp_1)| [Samsung 970 EVO NVMe M.2 SSD, 500GB](https://www.samsung.com/de/memory-storage/970-evo-nvme-m-2-ssd/MZ-V7E500BW/) |  M.2 Key M HDD|
| USB Wifi | 9,9€ [TP-Link TL-WN823N N300 Mini WLAN USB Adapter](https://www.amazon.de/gp/product/B0088TKTY2) | | can run in Access Point mode|
| 10x USB 3.0 hub | 32,99€ [ORICO 40W 10 Ports USB 3.0 hub](https://www.amazon.de/gp/product/B075QZ88DM) | | |
| usb c to usb b adapter | [USB 3.1 Type C (USB-C) auf Type B (USB-B) Kable](https://www.amazon.de/gp/product/B00UXKTJE0) | | |
| 2D Lidar | 99,90€ [Slamtec RPLidar A1M8](https://www.exp-tech.de/sensoren/entfernungnaeherung/8946/rplidar-a1m8-360-degree-laser-scanner-kit-12m) | [Introduction and Datasheet](http://bucket.download.slamtec.com/e9e096e9d9f30205d665260abe2cfb0c2dd62efa/LD108_SLAMTEC_rplidar_datasheet_A1M8_v1.0_en.pdf) | |
| IMU | 34,95€ [SparkFun MPU-9250 9DoF Razor IMU M0](https://eckstein-shop.de/SparkFun-9DoF-Razor-IMU-M0-MPU-9250) | [Hookup Guide](https://learn.sparkfun.com/tutorials/9dof-razor-imu-m0-hookup-guide?_ga=1.59377581.1661814591.1474882863) [Datasheet MPU-9250](https://cdn.sparkfun.com/assets/learn_tutorials/5/5/0/MPU9250REV1.0.pdf) [Datasheet SAMD21](https://cdn.sparkfun.com/datasheets/Dev/Arduino/Boards/Atmel-42181-SAM-D21_Datasheet.pdf) | |
| Camera | [OpenMV Cam M7](https://www.mybotshop.de/OpenMV-Cam-M7) with [fesheye lens](https://www.mybotshop.de/OpenMV-Kameraobjektiv-Ultra-Wide-Angle-Objektiv)| [OpenMV Cam M7](https://openmv.io/products/openmv-cam-m7) | |
| | ~250€ [Intel realsense D435i](https://click.intel.com/intel-realsense-depth-camera-d435i-imu.html) | [Intel Realsense D400 DatSheet](https://www.intel.com/content/dam/support/us/en/documents/emerging-technologies/intel-realsense-technology/Intel-RealSense-D400-Series-Datasheet.pdf)| |
| 2 x Hobby glass | 2 x ~6,00€ [25cm x 50cm x 4mm](https://www.hornbach.de/shop/Hobbyglas-4x250x500-mm-Glatt-klar/1477845/artikel.html?WT.mc_ag=41053541180&gclid=EAIaIQobChMImYKWxoXb3gIV67DtCh0h6gKkEAQYASABEgITS_D_BwE&WT.srch=1&WT.mc_id=DE_P_BS_AW_766103971) | | |
| M3 standoffs/nuts/etc. | [M3 Nylon Black Hex Screw Nut Spacer Standoff (260 pieces)](https://www.amazon.de/gp/product/B01MFF5XIC) | | | 
| controller | 66,90€ [DualShock 4 USB Wireless Adaptor](https://www.amazon.de/gp/product/B01KHFIO82) and 60,13€ [PlayStation 4 - DualShock 4 Wireless Controller](https://www.amazon.de/gp/product/B01GVQUX3U)| | |


# Tools
* [iFixit Pro Tech Toolkit](https://www.amazon.de/gp/product/B01GF0KV6G) (59,95€)
* [iFixit Tragbar Elektroschocks Matte](https://www.amazon.de/gp/product/B01BLPBOS4) (29,95€)
* [IMax B6AC V2 Balance Charger](https://www.amazon.de/VINGO®ORIGINAL-Netzteil-Batterie-Balance-Ladegerät/dp/B01AXVI6YW/ref=sr_1_1?ie=UTF8&qid=1540673676&sr=8-1&keywords=IMAX+Balance+Charger) (48,99€)



