# 内测使用说明（macOS 客户端 + 主机）

Last updated: 2026-03-13

## 0）先选模式（最重要）

### Local（本机模式）
适合：只想在当前这台 Mac 上直接使用。
- 不需要扫码
- 不需要配对 code
- 打开应用后选 Local，连接本机 OpenClaw 即可

### Remote（远程模式）
适合：要连接远程主机。
- macOS 客户端侧：输入 connect code 完成绑定
- 扫码动作发生在手机端（用于打开 claim 页面并拿到 code）

---

## 1）下载 macOS 客户端
直接下载（推荐）：
https://github.com/Cchhiillll/clawlink-pilot-docs/releases/download/v0.1.0-beta.3/ClawLinkMac-macos.zip

备用页面（下载异常时）：
https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.3

当前版本：`v0.1.0-beta.3`
文件名：`ClawLinkMac-macos.zip`

安装：
1. 解压
2. 把 `ClawLinkMac.app` 拖到 Applications
3. 打开应用
4. 若被拦截，右键 `ClawLinkMac.app` → **打开**

如果提示“应用已损坏 / 无法打开”：
1. 再次右键 `ClawLinkMac.app` → **打开**
2. 系统设置 → 隐私与安全性 → 允许打开
3. 还不行再执行：
```bash
xattr -dr com.apple.quarantine /Applications/ClawLinkMac.app
```

## 2）配置 Base URL
应用内 Settings → Base URL：
- `https://clawlink.wypchill.work`

---

## 3）Local 路径（本机直连）
1. 打开应用
2. 选择 **Local**
3. 进入会话后直接聊天

> Local 不需要注册/登录，不需要 connect code。

---

## 4）Remote 路径（远程主机）

### 4.1 注册 / 登录
在登录页选择 **Register**，填写：
- 邮箱
- 密码
- 邀请码

邀请码请联系内测组织者。

### 4.2 主机侧准备（管理员执行）
在主机端安装 Bridge 服务并保持在线。

### 4.3 生成并获取 connect code
在主机端生成配对二维码。

手机扫码打开 claim 页面后，复制 **connect code**。

### 4.4 macOS 客户端绑定
在 macOS 客户端：
- Add Device → 粘贴 connect code

> 说明：macOS 客户端不承担扫码动作。
> 扫码用于手机端打开 claim 页面并取回 code。
>
> 下个版本计划：pairing 命令支持省略 `device_id` 时自动生成，减少人工输入。

---

## 5）开始聊天
- 选择 设备 → Agent → 会话
- 如有需要，在聊天头部切换 Provider / Model（影响下一条消息）
- 发送消息并确认收到回复
