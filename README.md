# macOS 多用户机制深度调研

> 在线阅读：<https://chsdsunkissed-ux.github.io/macos-multiuser-research/>

## 内容

macOS 多用户机制的完整深度调研报告，覆盖两大主题：

- **场景 A｜保密性与安全性**：文件隔离、钥匙串、应用沙箱、TCC、FileVault、Secure Token
- **场景 B｜后台进程行为**：Fast User Switching（FUS，快速用户切换） vs 登出再登录 的差异，launchd 体系，App Nap，DAS-CTS

## 信源

- Apple 官方：Platform Security Guide、TN2083（Bootstrap Namespaces）、launchd.plist(5)、App Nap、ProcessInfo、Sandbox
- 第三方实测：Howard Oakley（eclecticlight.co）、Der Flounder（rtrouton）

## 调研产物

- `index.html` — 自包含 HTML 网页（含 CSS、暗色模式、TOC 锚点、Pygments 代码高亮）
- `macos-multiuser-CN-final.md` — 中文完整版 markdown（getnote note_id: 1914629028226306456）

## 调研工具链

由 Hermes Agent 在 Android Termux 环境生成，使用 `research-orchestration` skill 编排两个并发 subagent 拉取信源 + 中文塑形 + 上传 getnote。

调研日期：2026-07-04