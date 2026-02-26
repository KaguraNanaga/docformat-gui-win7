# DocFormat GUI — Windows 7 兼容版

> ⚠️ 这是 [docformat-gui](https://github.com/KaguraNanaga/docformat-gui) 的 **Windows 7 兼容构建仓库**，源代码完全相同，仅构建环境不同（Python 3.8）。

## 与主仓库的关系

| | 主仓库 docformat-gui | 本仓库 (Win7) |
|---|---|---|
| 源代码 | 相同 | 相同 |
| Python 版本 | 3.11 | 3.8 |
| 支持系统 | Win10+, macOS, Linux | **Win7 SP1+** |
| 构建产物 | docformat_windows.exe | docformat_windows_win7.exe |

## 下载

前往 [Releases](../../releases) 页面下载最新的 `docformat_windows_win7.exe`。

## 系统要求

- Windows 7 SP1 或更高版本
- 处理 `.doc` / `.wps` 格式需安装 Microsoft Office 或 WPS Office
- 推荐使用 `.docx` 格式以获得最佳兼容性

## 常见问题

**Q：双击后闪退怎么办？**

1. 确认已安装 Windows 7 SP1
2. 安装 [Visual C++ Redistributable 2015-2022](https://aka.ms/vs/17/release/vc_redist.x64.exe)
3. 用命令提示符运行 exe 查看详细报错

**Q：为什么单独开一个仓库？**

Python 3.9+ 已放弃 Windows 7 支持。本仓库使用 Python 3.8 构建，确保产物能在 Win7 上运行。源代码与主仓库保持同步。

## 同步主仓库代码

当主仓库有更新时，同步方法：

```bash
# 首次添加上游仓库
git remote add upstream https://github.com/KaguraNanaga/docformat-gui.git

# 拉取并合并
git fetch upstream
git merge upstream/main
git push origin main
```

## 注意事项

- Python 3.8 已于 2024 年 10 月 EOL，Win7 支持为尽力而为
- 功能与主仓库完全一致，bug 修复请提交到[主仓库](https://github.com/KaguraNanaga/docformat-gui/issues)
