# ClawLink 内测文档（Beta）

Last updated: 2026-03-14

这个仓库只放：
- 内测使用说明
- 下载链接

> 不包含项目源码，也不包含敏感配置。

## 下载（macOS）
- **直接下载（推荐）：**
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/download/v0.1.0-beta.5/ClawLinkMac-macos.zip
- 当前版本：`v0.1.0-beta.5`
- 当前包对应主仓库提交：`cb8787d`（`main`）
- 备用页（下载异常时再用）：
  https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.5

## 历史版本下载
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
- Remote：远程主机（macOS 输入 connect code；扫码发生在手机端）

## 当前功能范围（重要）
- ✅ 目前对外可用：
  - macOS 客户端下载与 Local 模式使用
  - 新版桌面壳层与图标
- ⚠️ 当前不对外开放：
  - Remote 绑定流程（仅内部测试可用）
  - 原因：主机侧配对码生成仍依赖私有项目脚本环境（项目仓库为 private）
- ⚠️ 规划中：
  - iOS 客户端

## 常见问题
看这里：`docs/troubleshooting.md`

## 版本维护规则
每次发布新版本，必须同步更新：
- `README.md`（版本号 + 下载链接 + 功能范围）
- `docs/pilot.md`（步骤变化 + 限制说明）
- `docs/troubleshooting.md`（新增问题与处理）
- GitHub Releases（新增版本入口，不覆盖旧版本）
