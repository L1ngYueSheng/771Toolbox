# 771 Toolbox（柒柒壹工具箱）

**正式版 v2.0（Flutter 版）已发布**——界面与实现全部换成 Flutter，替代原 tkinter 版 v1.45。
五个主模块（**格式转换 / 批量改名 / 视频下载 / 压缩解压 / 截图**）+ 一页 **系统工具**
（文件哈希 / 重复文件 / 二维码 / 剪贴板历史 / 文件切割 / 大文件与空文件夹 / 文本小工具 / 图片取字），
全部为可用的真功能。注:该软件为100%AI

## 下载

到 [Releases](https://github.com/L1ngYueSheng/771Toolbox/releases) 页面：

| 文件 | 说明 |
| --- | --- |
| `QQYToolboxUI_v2.0_20261016.zip` | **v2.0 正式版**：解压后双击 `程序\qqy_toolbox_ui.exe`，免安装（约 13 MB） |
| `version.json` / `version.json.sig` | 更新清单及其 Ed25519 签名——仍指向 **v1.45**（见下"更新说明"） |
| 历史版本 v1.45 及更早 | 在 Releases 历史里，原 exe 形态仍可下载 |

> 资产名只能是 ASCII（GitHub 会把非 ASCII 字符剥掉）。
> 本仓库**只放发布版主程序与更新清单**：不放源码（源码随发布包内"源码"目录），也不含任何私钥。

## 全局热键（v2.0）

- `Ctrl+Alt+A` 区域截图（就地蒙层：拖框 / Enter 确认 / Esc 取消）
- `Ctrl+Alt+5` 全屏截图 · `Ctrl+Alt+6` 取色器 · `Ctrl+Alt+7` 贴图最近一张
- 旧版截图工具同时在跑时，A 键会被它占住——v2.0 如实显示"被占用"并让位，不抢键。

## 更新说明（重要）

- **旧版 v1.45 的联网自动更新不会把你带到 v2.0**（架构换代无法自动替换文件夹形态）。
  本 Release 里附的仍是 v1.45 的 `version.json`，旧版运行时会继续显示"已是最新"，不受打扰。
- **v2.0 请手动下载本包**；v2.0 自己的自动更新尚未接入，计划下一版补。

## 引擎与依赖（v2.0 为"借用本机引擎"形态）

视频下载用本机 Python 的 yt-dlp（`py -3 -m yt_dlp`）；音视频转换用本机散装 ffmpeg；
7z / rar 走旧版工具箱目录里的 `7z.exe`；图片取字用本机 winocr（Windows 自带离线 OCR）。
缺哪个，对应功能会在界面如实报错或置灰，不会假装能跑。包内 `使用说明.txt` 有完整清单与已知边界。

## 其他两个独立版

- **771 Screenshot Tool**（截图 + 录屏）——<https://github.com/L1ngYueSheng/771ScreenshotTool>
- **771 Format Factory**（格式转换 + PDF / 图片 / 音视频加工）——<https://github.com/L1ngYueSheng/771FormatFactory>
