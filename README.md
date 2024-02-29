## 大雕 QWRT 月经问题汇总备忘

---
**Q：QWRT的默认登陆地址和帐号密码是多少？**

A：默认登陆地址是`http://192.168.1.1`，默认帐号密码是`admin`/`password`

---

**Q：为什么我刷了QWRT看不到那些东方神秘插件？**

A：在ssh输入以下命令，然后刷新web界面就显示了
```bash
echo 0xDEADBEEF > /etc/config/google_fu_mode
```
---
**Q: 固件文件名中带**factory**固件和带**sysupgrade**固件分别用在什么地方？**

A：文件名中带**factory**固件一般是通过uboot web刷入；文件名中带**sysupgrade**固件一般是在QWRT系统内升级适用，有些uboot也可以使用**sysupgrade**刷机具体看机型。

---
**Q：我能自己安装缺失的kmod依赖包吗？**

A：一般情况下是不能的，kmod的包需要和内核匹配才行，开源固件一般可以通过自行编译加入需要的kmod，闭源需要大雕提供固件对应的kmod文件才能手动安装。

---
**Q：如何进入uboot（不死）web界面？**

A：路由器断电，用卡针按住reset通电开机保持5-10s，然后松开，电脑配置如IP地址：192.168.1.10 掩码：255.255.255.0，打开浏览器访问http://192.168.1.1。

---
**Q：大雕的QWRT固件在哪里下载？**

A：QQ QWRT VIP群付费50，找大雕拉进固件群，如果固件群没有的历史固件，只能寻求群友看看有没有存货。

---
**Q：QWRT万兆设备固件和Wi-Fi 7（BE）设备固件在哪里下？**

A：如果你在固件群找不到，那大概率是需要额外DLC付费型号，联系大雕。
