ESP-IDF template app
====================

This is a template application to be used with [Espressif IoT Development Framework](https://github.com/espressif/esp-idf).

Please check [ESP-IDF docs](https://docs.espressif.com/projects/esp-idf/en/latest/get-started/index.html) for getting started instructions.

*Code in this repository is in the Public Domain (or CC0 licensed, at your option.)
Unless required by applicable law or agreed to in writing, this
software is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
CONDITIONS OF ANY KIND, either express or implied.*

#OUTPLAY

â†�[0;33m--- idf_monitor on \\.\COM3 115200 ---â†�[0m
--- Quit: Ctrl+] | Menu: Ctrl+T | Help: Ctrl+T followed by Ctrl+H ---
ets Jul 29 2019 12:21:46

rst:0x1 (POWERON_RESET),boot:0x13 (SPI_FAST_FLASH_BOOT)
configsip: 0, SPIWP:0xee
clk_drv:0x00,q_drv:0x00,d_drv:0x00,cs0_drv:0x00,hd_drv:0x00,wp_drv:0x00
mode:DIO, clock div:2
load:0x3fff0030,len:6668
ho 0 tail 12 room 4
load:0x40078000,len:14944
load:0x40080400,len:3816
0x40080400: _init at ??:?

entry 0x40080698
I (29) boot: ESP-IDF v4.4.4-dirty 2nd stage bootloader
I (29) boot: compile time 12:00:39
I (29) boot: chip revision: v3.0
I (33) boot_comm: chip revision: 3, min. bootloader chip revision: 0
I (40) boot.esp32: SPI Speed      : 40MHz
I (44) boot.esp32: SPI Mode       : DIO
I (49) boot.esp32: SPI Flash Size : 2MB
I (54) boot: Enabling RNG early entropy source...
I (59) boot: Partition Table:
I (62) boot: ## Label            Usage          Type ST Offset   Length
I (70) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (77) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (85) boot:  2 factory          factory app      00 00 00010000 00100000
I (92) boot: End of partition table
I (96) boot_comm: chip revision: 3, min. application chip revision: 0
I (103) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=12e10h ( 77328) map
I (140) esp_image: segment 1: paddr=00022e38 vaddr=3ffb0000 size=0389ch ( 14492) load
I (146) esp_image: segment 2: paddr=000266dc vaddr=40080000 size=0993ch ( 39228) load
I (162) esp_image: segment 3: paddr=00030020 vaddr=400d0020 size=6f420h (455712) map
I (328) esp_image: segment 4: paddr=0009f448 vaddr=4008993c size=0b2f8h ( 45816) load
I (357) boot: Loaded app from partition at offset 0x10000
I (357) boot: Disabling RNG early entropy source...
I (368) cpu_start: Pro cpu up.
I (369) cpu_start: Starting app cpu, entry point is 0x400811c4
0x400811c4: call_start_cpu1 at C:/Espressif/frameworks/esp-idf-v4.4.4/components/esp_system/port/cpu_start.c:148

I (0) cpu_start: App cpu up.
I (383) cpu_start: Pro cpu start user code
I (383) cpu_start: cpu freq: 160000000
I (383) cpu_start: Application information:
I (387) cpu_start: Project name:     app-template
I (393) cpu_start: App version:      1
I (397) cpu_start: Compile time:     Nov  7 2023 11:59:22
I (403) cpu_start: ELF file SHA256:  7e1d326b6354b2a6...
I (409) cpu_start: ESP-IDF:          v4.4.4-dirty
I (415) heap_init: Initializing. RAM available for dynamic allocation:
I (422) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (428) heap_init: At 3FFB7278 len 00028D88 (163 KiB): DRAM
I (434) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (440) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (447) heap_init: At 40094C34 len 0000B3CC (44 KiB): IRAM
I (454) spi_flash: detected chip: generic
I (458) spi_flash: flash io: dio
W (462) spi_flash: Detected size(4096k) larger than the size in the binary image header(2048k). Using the size in the binary image header.
I (476) cpu_start: Starting scheduler on PRO CPU.
I (0) cpu_start: Starting scheduler on APP CPU.
I (561) wifi station: ESP_WIFI_MODE_STA
I (571) wifi:wifi driver task: 3ffbf814, prio:23, stack:6656, core=0
I (571) system_api: Base MAC address is not set
I (571) system_api: read default base MAC address from EFUSE
I (591) wifi:wifi firmware version: 6567a16
I (591) wifi:wifi certification version: v7.0
I (591) wifi:config NVS flash: enabled
I (591) wifi:config nano formating: disabled
I (601) wifi:Init data frame dynamic rx buffer num: 32
I (601) wifi:Init management frame dynamic rx buffer num: 32
I (611) wifi:Init management short buffer num: 32
I (611) wifi:Init dynamic tx buffer num: 32
I (611) wifi:Init static rx buffer size: 1600
I (621) wifi:Init static rx buffer num: 10
I (621) wifi:Init dynamic rx buffer num: 32
I (631) wifi_init: rx ba win: 6
I (631) wifi_init: tcpip mbox: 32
I (631) wifi_init: udp mbox: 6
I (641) wifi_init: tcp mbox: 6
I (641) wifi_init: tcp tx win: 5744
I (651) wifi_init: tcp rx win: 5744
I (651) wifi_init: tcp mss: 1440
I (651) wifi_init: WiFi IRAM OP enabled
I (661) wifi_init: WiFi RX IRAM OP enabled
I (671) phy_init: phy_version 4670,719f9f6,Feb 18 2021,17:07:07
I (771) wifi:mode : sta (94:b5:55:f8:2d:6c)
I (771) wifi:enable tsf
I (781) wifi station: wifi_init_sta finished.
I (791) wifi:new:<6,0>, old:<1,0>, ap:<255,255>, sta:<6,0>, prof:1
I (791) wifi:state: init -> auth (b0)
I (801) wifi:state: auth -> assoc (0)
I (801) wifi:state: assoc -> run (10)
I (10801) wifi:state: run -> init (cc00)
I (10811) wifi:new:<6,0>, old:<6,0>, ap:<255,255>, sta:<6,0>, prof:1
I (10811) wifi station: retry to connect to the AP
I (10811) wifi station: connect to the AP fail
I (13221) wifi station: retry to connect to the AP
I (13221) wifi station: connect to the AP fail
I (13231) wifi:new:<6,0>, old:<6,0>, ap:<255,255>, sta:<6,0>, prof:1
I (13231) wifi:state: init -> auth (b0)
I (13231) wifi:state: auth -> assoc (0)
I (13241) wifi:state: assoc -> run (10)
I (13341) wifi:connected with Areenaï¿½ï¿½ï¿½s iphone, aid = 2, channel 6, BW20, bssid = e2:5d:e7:97:c2:ed
I (13341) wifi:security: WPA2-PSK, phy: bgn, rssi: -85
I (13351) wifi:pm start, type: 1

I (13361) wifi:<ba-add>idx:0 (ifx:0, e2:5d:e7:97:c2:ed), tid:0, ssn:2, winSize:64
I (13381) wifi:AP's beacon interval = 102400 us, DTIM period = 3
I (14351) esp_netif_handlers: sta ip: 172.20.10.5, mask: 255.255.255.240, gw: 172.20.10.1
I (14351) wifi station: got ip:172.20.10.5
I (14351) wifi station: connected to ap SSID:Areenaï¿½ï¿½ï¿½s iphone password:Treasure12

