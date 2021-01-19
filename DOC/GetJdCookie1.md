## 电脑浏览器获取京东cookie教程

**内容引用于[@lxk0301](https://github.com/lxk0301)**

**以下浏览器都行**

 - Chrome浏览器
 - 新版Edge浏览器
 - 国产360，QQ浏览器切换到极速模式

### 操作步骤

1. 电脑浏览器打开京东网址 [https://m.jd.com/](https://m.jd.com/)
2. 按键盘F12键打开开发者工具，然后点下图中的图标
 ![切换到手机模式](../img/jd1.jpg)
3. 此时是未登录状态(使用手机短信验证码登录)，如已登录请忽略此步骤
     - 使用手机短信验证码登录(此方式cookie有效时长大概31天，其他登录方式比较短)
4. 登录后，选择Network,有很多链接的话点箭头这里清空下
    ![清空](../img/jd2.jpg)
5. 然后再点我的，链接就变少了
    ![再次点击我的](../img/jd3.jpg)
6. 点第一个链接(log.gif)进去，找到cookie，复制出来，新建一个TXT文本临时保存一下，下面需要用到
- **这里注意一下：快捷指令支持填入整个Cookie，第7步可以忽略**
 ![寻找log.gi](../img/jd4.jpg)
~~7. 第6步复制出来的cookie比较长，我们只需要`pt_pin=xxxx;`和 `pt_key=xxxx;`部分的内容即可(注:英文引号`;`是必要的)。可以用下面的脚本，在Chrome浏览器按F12，console里面输入下面脚本按enter回~~
    ``` javascript
    // 快捷指令可忽略此步
    var CV = '单引号里面放第六步拿到的cookie';
    var CookieValue = CV.match(/pt_pin=.+?;/) + CV.match(/pt_key=.+?;/);
    copy(CookieValue);
    ```
8. 这样子整理出关键的cookie已经在你的剪贴板上，可直接粘贴

9. 如果需获取第二个京东账号的cookie,不要在刚才的浏览器上面退出登录账号一(否则刚才获取的cookie会失效),需另外换一个浏览器(Chrome浏览器 `ctr+shift+n` 打开无痕模式也行),然后继续按上面步骤操作即可
