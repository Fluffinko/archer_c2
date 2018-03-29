# archer_c2
archer c2 lede + huawei_e3372h-153

1. create directory image on desktop and copy ArcherC2V1_tp_recovery.bin to it
2. set ip on your LAN adapter to 192.168.0.66 and mask 255.255.255.0 press ok
3. start tftpd64.exe
4. set base directory C:\Users\{your_username}\Desktop\image
5. turn off archer c2
6. turn on archer c2 with pressed reset button
7. wait for transfer complete
8. change your LAN adapter to 192.168.1.xx or use dhcp
7. login to router on ip 192.168.1.1
8. go to system --> backup / flash firmware --> Flash new firmware image --> choose file lede-ramips-mt7620-ArcherC2-squashfs-sysupgrade.bin
9. flash image
10. wait for router to reboot
11. connect internet to WAN port
12. use putty to connect to ssh 192.168.1.1
13. use command "opkg update"
14. use command "opkg install liblua lua libuci-lua libubus libubus-lua uhttpd rpcd luci-base luci-lib-ip luci-lib-nixio luci-theme-bootstrap luci-mod-admin-full luci-lib-jsonc
15. reboot router with command reboot
16. enjoy :)
