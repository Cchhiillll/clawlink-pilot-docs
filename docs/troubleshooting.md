# 常见问题排查

Last updated: 2026-03-14

## 1）无法注册
- 确认 Base URL 是：`https://clawlink.wypchill.work`
- 邀请码可能无效/过期/已撤销，请联系组织者

## 2）设备一直离线
- 主机上的 Bridge 服务没启动
- 主机网络无法访问 Cloudflare

## 3）设备绑定失败（claim 不成功）
- connect code 过期（有效期较短）
- connect code 已被使用

## 4）macOS 应用打不开 / 提示“已损坏”
- 重新确认下载的是 `ClawLinkMac-macos.zip`
- 当前对照版本：`v0.1.0-beta.4`（主仓库提交 `c1456e1`）
- 先解压，再把 `ClawLinkMac.app` 拖到 Applications
- 右键 `ClawLinkMac.app`，选择 **打开**
- 系统设置 → 隐私与安全性 → 允许打开
- 仍失败可执行：
  ```bash
  xattr -dr com.apple.quarantine /Applications/ClawLinkMac.app
  ```

## 反馈时请附带
- 卡在哪一步（1～6）
- 报错截图
- 若是主机问题，附 Bridge 日志（如有）
  - macOS: `~/Library/Logs/ClawLink/bridge.log`
  - Linux: `sudo journalctl -u clawlink-bridge -n 200 --no-pager`
