# 771Toolbox

本仓库**只用于分发布「柒柒壹工具箱」的更新资产**（用于程序内置的联网自动更新）：

- `version.json` / `version.json.sig` —— 版本清单及其 Ed25519 签名（程序用它判断有没有新版本）
- `771Toolbox.exe` —— 发布版主程序

**本仓库不放源码**，也不包含任何私钥。

更新下载地址口径：清单固定用 `releases/latest/download/version.json`；程序包用**带 tag 的不可变地址**
（`releases/download/v<版本>/771Toolbox.exe`），配合清单里的 SHA-256 校验。
