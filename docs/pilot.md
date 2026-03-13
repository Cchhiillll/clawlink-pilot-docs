# 内测使用说明（macOS 客户端 + 主机）

Last updated: 2026-03-13

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

## 3）注册 / 登录
在登录页选择 **Register**，填写：
- 邮箱
- 密码
- 邀请码

邀请码请联系内测组织者。

## 4）主机侧安装 Bridge（macOS 或 Linux）
如果你是“主机管理员”，需要在主机上安装 Bridge 服务并配置环境变量。
如果你只是普通用户，可以跳过第 4 步，直接看第 5 步。

## 5）主机配对（二维码 → connect code）
在主机端生成配对二维码。

手机扫码打开 claim 页面后，复制 **connect code**。

在 macOS 客户端：
- Add Device → 粘贴 connect code

> 说明：当前设计就是“手机端扫码 claim，macOS 客户端粘贴 connect code”流程。
> macOS 客户端不承担扫码职责。
>
> 下个版本计划：pairing 命令支持省略 `device_id` 时自动生成，减少人工输入。

## 6）开始聊天
- 选择 设备 → Agent → 会话
- 如有需要，在聊天头部切换 Provider / Model（影响下一条消息）
- 发送消息并确认收到回复
