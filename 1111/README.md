# 天猫双 11 喵果总动员自动任务

## 功能说明

- 支持 ios13-16 ipad 自动化
- 实现简单的淘宝双 11 喵果总动员自动任务
- ⚠️ 注意:因各种权限原因，本快捷指令只能完成部分任务，剩余任务与自己看情况手动，作者会尽力往全自动更新，请关注新版本。

TG 频道:https://t.me/xuehuashe

## 版本日志

### 2022-11-08 v2.0

- 修复 AutoBox，自动化会运行到普通模式去的 bug

https://www.icloud.com/shortcuts/3206a1b0cda242a092222f9d28e4560d

### 2022-11-05 v1.9

- 修复 部分账号 cookie 编码错误问题（强化）
- 优化 15.0-15.2 系统 改为手动输入 cookie

https://www.icloud.com/shortcuts/f95f75e5c16e42d1b3500064e0c56b8d

### 2022-11-05 v1.8

- 修复 因 Scriptable App 造成的 UTF-8 编码错误问题
- 修复 自动化，AutoBox 会弹出菜单问题，目前自动化只支持运行账号 1
- 优化 Cookie 获取引导
- 新增 秒登录获取 Cookie

https://www.icloud.com/shortcuts/7e82bbbdfa594e1c9377c9cea744318c

💡 如需重复运行指令，可以只选“赚喵果”任务，其他任务已经做完
💡 有剩余任务没有做的很正常，指令一直都是只能做部分任务，请手动做剩余任务
💡 请不要擅自修改指令名字，请保持原名字，否则会出错

免登陆获取 Cookie

- 视频教程
  https://szd55vqajl.feishu.cn/docx/DX6gdWJRhoLsRqxriLHcfkDwndX#YiEUdI4AMoiGUcxIfShcjyxUn8d

- 文字教程
  1. 提前准备好 Stream App，并安装描述文件，信任 CA 证书
  2. 退出淘宝，打开 Stream 开始抓包
  3. 运行快捷指令-指令设置-授权账号-登录账号 n-跳转 App 抓包页
  4. 返回 Stream 停止，查询抓包历史
  5. 找到链接以 h5api 开头的记录，右上角分享，选择快捷指令-登录账号 n，保存完毕
  6. 观察 iCloud 云盘 ▸ Shortcuts ▸ Leeco ▸ tb ▸ cookie 下面的 cookie 文件是否是刚刚的时间，已确保所有步骤的成功
  7. 开始任务~

### 2022-11-02 v1.7

- 修复 ios 13 弹错问题
- 修复 任务递归弹窗问题
- 修复 多账号授权 cookie 保存失败问题

https://www.icloud.com/shortcuts/4736a72a4f634b408bc82deb3760c0fa

### 2022-11-02 v1.6

- 增加 多账号授权存储功能，做任务只能选一个账号
- 优化 兼容 ios13 系统，将每次继续手动输入 cookie
- 优化 互相助力算法，修复助力错误，排除重复发口令者，一律进入黑名单
- 更新 云端任务数据，增加两个支付宝里的任务

https://www.icloud.com/shortcuts/37c3cfaa5665453e80b252861daa1edf

⚠️ 此版本先测试中，将在 3 号强制更新。
💡 喵果总动员想要升满级，基本需要完成每天互助的，强烈推荐没有时间参与活动的人，通过指令随机助力他人，助力他人也有很多奖励。大家参与进来才能让互助功能更健康，按目前的优化算法，如果都相互互助，发一次口令能接受到 5 个助力。
👥 关于助力大厅：需要先注册 github 账号，然后用 github 账号登录，如果无法注册成功可以尝试使用 matrix/element 进入助力大厅。如果发现消息发不出去，可以尝试下载 gitter app，从那发消息。

### 2022-10-30 v1.5

- 增加 自动刷新 Cookie 功能，只要没有 Session 过期就不用再次抓包，可以直接开始任务。完美实现自动化，目前只支持一个账号。
- 增加 指令第一次使用新版本判断功能，优化版本过渡机制
- 更新 授权登录功能移入到「指令设置」当中

https://www.icloud.com/shortcuts/6402c3bb97b14ebeb032cae73809da39

⚠️ 更新后第一次运行有"非常多"的授权弹窗，请全程看护，并点击"全部始终同意"。忽略则无法正常运行任务，需要重启手机再次运行指令，才会重新弹窗。 全部授权完毕后，往后运行无需再次授权。

⚠️ 本指令可能无法兼容 ios13.x , ios15.0-15.2，请升级你的系统至兼容版本。

⚠️ 本次指令功能有较大变动，需要先去往「指令设置」授权登录，Cookie 将持久化存入到 iCloud 文件中，今后将与淘宝系其他指令共享数据。

💡 此次发布的新版本，由于较大变动，暂不强制更新，先测试一段时间。本指令强制需要安装 Scriptable App，ios 13 无法下载，将在下个版本 兼容 ios 13 每次手动输入 cookie

Scriptable App:
https://apps.apple.com/cn/app/scriptable/id1405459188

### 2022-10-24 v1.4

- 采用 最新的淘宝系框架
- 实现 喵果总动员部分任务，最后使用令牌模式
- 优化 线路判断功能
- 优化 递归运行逻辑
- 兼容 ios13-16

https://www.icloud.com/shortcuts/a28d108b69e3424688e9e1a837b46aeb

### 2021-11-05 v1.3

- 优化 小屏手机的显示效果
- 优化 令牌模式的使用引导和逻辑

https://www.icloud.com/shortcuts/a2c78b549662411a83184e094462a0d2

### 2021-10-31 v1.2

- 新增 令牌模式 专过强校验
- 兼容 ios15.1 版本（还是不建议你升级 15.1,运行时间是原来的 2 倍）

https://www.icloud.com/shortcuts/ffa746737bc242f8825888d03dbfe1f5

### 2021-10-22 v1.1

- 更新 数据源解决无奖励问题
- 更新 云端助力池开放

https://www.icloud.com/shortcuts/11c46d0b1cf849a8b773ad1bae6b4fbe

### 2020-12-16 v1.0

- 实现 双 11 喵糖的一些自动化任务
- 支持 AutoBox 和自动化
- 助力池建设中...

https://www.icloud.com/shortcuts/922845d547014277841c64f7d137e70f

## 免责申明

- 本快捷指令仅用于学习交流使用
- 切勿用于商业及非法用途
