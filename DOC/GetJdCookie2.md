## 手机Stream app获取Cookie

**内容引用于网络**

### 步骤

1. 首先我们先去App Store 下载【Stream】安装并使用

![v2-f0b8a31709402a919630856816d51bfa_1440w](http://img.cdn.80008800.xyz/v2-f0b8a31709402a919630856816d51bfa_1440w.jpg)

2. 首次打开需要安装信任证书，根据提示进行安装即可：点击“允许”添加，然后点击去安装证书。

![v2-c71681139583fe7e57f3b395a053d6d9_1440w](http://img.cdn.80008800.xyz/v2-c71681139583fe7e57f3b395a053d6d9_1440w.jpg)

3. 点击“步骤一：安装CA证书”，会自动跳转到Safari浏览器，点击“允许”下载配置文件。

![v2-b0740cfa44abf1dcc9765ceae71904aa_1440w](http://img.cdn.80008800.xyz/v2-b0740cfa44abf1dcc9765ceae71904aa_1440w.jpg)

4. 我们回到系统设置，点击已下载描述文件，然后根据提示安装。

![v2-f4de447f51404fb8eaf1d2dca689c677_1440w](http://img.cdn.80008800.xyz/v2-f4de447f51404fb8eaf1d2dca689c677_1440w.jpg)

5. 回到App，点击去信任证书，系统设置-通用-关于（最底部）信任CA证书

![v2-e7a5a5c14eec20b4a78ede723a470e44_1440w](http://img.cdn.80008800.xyz/v2-e7a5a5c14eec20b4a78ede723a470e44_1440w.jpg)

6. 回到App，点击清除HTTPS临时证书缓存。

![v2-82b3b9c0d7d5927d475443abad3fddb2_1440w](http://img.cdn.80008800.xyz/v2-82b3b9c0d7d5927d475443abad3fddb2_1440w.jpg)


好了，App已经配置完成了。

7. 接下来就是正戏了，请留意接下来的每一步哦

![v2-4f6dcdcb61a171930dc4feef00f80609_1440w](http://img.cdn.80008800.xyz/v2-4f6dcdcb61a171930dc4feef00f80609_1440w.jpg)

**具体步骤为：打开软件-点击开始抓包，使用系统自带Safari浏览器打开京东网页版链接：https://bean.m.jd.com/进入登录页面-登录账号-回到App停止抓包，找到带有截图中信息的记录并进入该记录-点击请求头下面的内容-进入请求头界面-选中Cookie里的所有内容-拷贝。注意红框圈出部分不要复制到了。**
