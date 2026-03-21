# 内测使用说明（macOS 客户端 + 主机）

Last updated: 2026-03-21

## 0）先选模式（最重要）

### Local（本机模式）
适合：只想在当前这台 Mac 上直接使用。
- 不需要扫码
- 不需要配对 code
- 打开应用后选 Local，连接本机 OpenClaw 即可

### Remote（远程模式）
- 当前 public `beta.7` 已开放入口。
- 默认主路径已经切到 one-command host setup。
- 只有在 setup token 暂时不可用时，才需要退回 connect code fallback。

---

## 1）下载 macOS 客户端
直接下载（推荐）：
https://github.com/Cchhiillll/clawlink-pilot-docs/releases/download/v0.1.0-beta.7/ClawLinkMac-macos.zip

备用页面（下载异常时）：
https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.7

当前版本：`v0.1.0-beta.7`
文件名：`ClawLinkMac-macos.zip`
对应主仓库提交：`b3b0ef6`（`main`）

历史版本入口：
- https://github.com/Cchhiillll/clawlink-pilot-docs/releases

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
3. 等待应用完成本机 Gateway 检查
4. 进入会话后直接聊天

> Local 不需要注册/登录，不需要 connect code。

---

## 4）Remote 路径（远程主机）

### 4.1 注册 / 登录
在登录页选择 **Register**，填写：
- 邮箱
- 密码
- 邀请码

邀请码请联系内测组织者。

### 4.2 默认主路径：Add Device → one-command setup
在 macOS 客户端：
1. 打开 **Add Device**
2. 复制对应宿主机的命令
3. 在宿主机执行这条命令

客户端会展示两条命令：
- macOS Host Command
- Linux Host Command

宿主机命令会自动完成：
- 安装或更新 Bridge
- 绑定到当前账号
- 写入 bridge env
- 启动服务并尝试拉到 online

### 4.3 fallback：只有 setup token 不可用时才用 connect code
如果客户端没有展示 one-command setup，或明确提示需要 fallback：
1. 在主机端按管理员流程生成 connect code
2. 回到 macOS 客户端点 **Add Device**
3. 展开 **Have a Connect Code Already?**
4. 粘贴 connect code 并 claim

> 当前 public `beta.7` 构建已开放 **Remote** 默认主路径。
> connect code 仍保留，但已经退到 fallback / 兼容路径。

---

## 5）开始聊天
- 选择 设备 → Agent → 会话
- 如有需要，在聊天头部切换 Provider / Model（影响下一条消息）
- 发送消息并确认收到回复
