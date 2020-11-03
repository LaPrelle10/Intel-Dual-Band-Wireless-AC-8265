[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/LaPrelle10/Intel-Dual-Band-Wireless-AC-8265)

# Intel-Dual-Band-Wireless-AC-8265
The Intel Dual Band Wireless-AC 8265 adapter supports Bluetooth 4.2 and 2x2 11ac Wi-Fi delivering up to 867Mbps including wave 2 features such as downlink MU-MIMO providing up to 3x increase in user speeds in dense deployments, supporting fast downloads and long battery life compared to legacy 11ac devices. Combined with Intel Core processsors and exceptional Intel wireless innovations, the Intel Dual Band Wireless-AC 8265 dramatically reshapes your connected experience at home, work, or on the go.

# Raspberry Intel Dual Band Wireless AC 8265
Can be used as a wifi montior system :

$ iw dev
$ iw phy phy0 info # should show all information about the device, including the "monitor" capability
$ sudo iw phy phy0 interface add mon0 type monitor
$ ip link
$ sudo iw dev wlan0 del # (I had to replace wlan0 by wlp2s0)
$ sudo ip link set mon0 up
$ iw dev mon0 info
$ sudo iw dev mon0 set freq 2437 # set it to the right channel
