# ClawLink Pilot Docs

Last updated: 2026-03-27

这个仓库只放：
- 内测使用说明
- 下载链接

> 不包含项目源码，也不包含敏感配置。

## Current Public Version
- 当前公开下载版本：`v0.1.0-beta.8`
- 直接下载（推荐）：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/download/v0.1.0-beta.8/ClawLinkMac-macos.zip
- Release 页面（下载异常时再用）：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.8
- 当前包对应主仓库提交：`619bf7d`（`main`）
- 官网：
  https://clawlinksite.wypchill.work/

## Pilot Access
- 当前 ClawLink 仍处于邀请码内测阶段。
- 如需邀请码，请直接联系我本人获取。

## 历史版本下载
- `v0.1.0-beta.8`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.8
- `v0.1.0-beta.7`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.7
- `v0.1.0-beta.6`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.6
- `v0.1.0-beta.5`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.5
- `v0.1.0-beta.4`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.4
- `v0.1.0-beta.3`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.3
- `v0.1.0-beta.2`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.2
- `v0.1.0-beta.1`：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.1

## 快速开始
看这里：`docs/pilot.md`

核心流程：**设备 → Agent → 会话 → 聊天**

模式说明：
- Local：本机直连（不需要扫码/配对 code）
- Remote：远程主机（默认是 one-command setup；connect code 仅作为 fallback）
  - 当前 `beta.8` 的宿主机命令会使用 public `clawlink-host-bundle.tar.gz`，不需要源码仓权限

## 当前功能范围（重要）
- ✅ 目前对外可用：
  - macOS 客户端下载与 Local 模式使用
  - Local 模式
  - Remote 入口、登录、Add Device、远程聊天主链路
  - Remote one-command setup 使用 public host bundle 分发，不再要求宿主机访问私有源码仓
- ⚠️ 当前仍需操作者准备：
  - 宿主机侧 Bridge 安装与在线
  - 在宿主机执行客户端提供的 one-command setup
  - setup token 不可用时再走 connect code fallback
- ⚠️ 规划中：
  - iOS 客户端

## 常见问题
看这里：`docs/troubleshooting.md`

## Notes
- 当前公开下载版本为 `v0.1.0-beta.8`
- 新一轮内测与体验打磨仍在继续
- 若站内页面提到 Beta 9，请理解为当前内测迭代状态，不等同于公开下载版本
- 如遇说明冲突，请优先以本仓库 release 与使用文档为准

## 版本维护规则
每次发布新版本，必须同步更新：
- `README.md`（版本号 + 下载链接 + 功能范围）
- `docs/pilot.md`（步骤变化 + 限制说明）
- `docs/troubleshooting.md`（新增问题与处理）
- GitHub Releases（新增版本入口，不覆盖旧版本）

## 维护者说明
发布时请同时参考：`docs/release-maintenance.md`
