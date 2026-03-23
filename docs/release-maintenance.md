# clawlink-pilot-docs 发布维护说明

Last updated: 2026-03-23

这份文档给维护者 / agent 使用，不面向普通用户。

## 这仓负责什么

- 创建 public GitHub release/tag
- 托管 macOS ZIP 下载入口
- 托管 public host bundle（`clawlink-host-bundle.tar.gz`）
- 提供对外 README / 使用说明 / 排障文档

## 发版硬规则

1. 新 tag / release、macOS ZIP、host bundle 资产没准备好前，不要修改 public 文档里的版本号和下载链接。
2. `README.md`、`docs/pilot.md`、`docs/troubleshooting.md` 三处必须一起更新。
3. 版本号、下载 URL、release page、源码提交号必须保持一致。
4. 历史 release 不覆盖，只新增。

## 每次发版至少要改的文件

- `/Users/wangyipeng/.openclaw/workspace/clawlink-pilot-docs/README.md`
- `/Users/wangyipeng/.openclaw/workspace/clawlink-pilot-docs/docs/pilot.md`
- `/Users/wangyipeng/.openclaw/workspace/clawlink-pilot-docs/docs/troubleshooting.md`

## 推荐顺序

1. 确认新版本号，例如 `v0.1.0-beta.8`
2. 从源码仓拿到：
   - 源码 commit hash
   - ZIP 文件名
   - host bundle 文件名
   - 对外功能范围
   - 已知风险 / 未验证项
3. 在 GitHub 创建对应 release/tag
4. 上传 ZIP
5. 上传 `clawlink-host-bundle.tar.gz`
6. 实测下载 URL 可访问
   - `ClawLinkMac-macos.zip`
   - `clawlink-host-bundle.tar.gz`
7. 再更新本仓三份文档
8. 提交并 push

## 文案检查项

- README 的“当前版本”
- README 的 direct download / release page
- 历史版本列表
- `docs/pilot.md` 里的当前版本、下载链接、Remote 流程
- `docs/troubleshooting.md` 里的对照版本号和常见报错说明
- Remote 文案里不要再暗示用户需要私有源码仓权限

## 不要做的事

- 不要提前把 public README 切到一个还不存在的 release
- 不要只改 README，不改 `docs/pilot.md` / `docs/troubleshooting.md`
- 不要把“待验证项”写成“已完成”
