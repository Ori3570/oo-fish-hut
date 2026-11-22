# 来源与第三方许可

大肥鱼小屋从已有的养鱼工作流发展成独立应用。Windows 公开版沿用项目的 0.7.1 纯净聊天版。Android 0.2.3-a1 将手机界面封装成可本地安装的应用。作者署名为「哦哦是鲸鲸」。

| 内容 | 来源与许可 |
| --- | --- |
| 暗蓝鲸鱼娘图片与桌宠动画 | Windows 沿用 `PC2005-cloud/dsh-pet` 的暗蓝素材，包含五组共 1205 帧 WebP 动画。Android 随包保留角色 MIT 原许可。上游版权归 PC2005-cloud。 [取材版本](https://github.com/PC2005-cloud/dsh-pet/commit/549fff2ea33c2acfb16612c76912c6137da4a758) |
| 桌宠状态模型 | Windows 沿用 `dsh-dafeiyu` 0.1.18 的纯 Python AnimationModel，MIT 声明随包保留。 [上游代码](https://github.com/QCYTSN/dsh-dafeiyu) |
| Windows 运行库 | Python 3.12、PySide6/Qt 6.11.1、PyInstaller 6.21.0。各库版本和许可证放在 Windows 压缩包的 `licenses/`。构建采用独立、可替换的 Qt 动态库。 [Qt 的 LGPL 说明](https://www.qt.io/development/open-source-lgpl-obligations) |
| 安卓运行库 | Capacitor 8.3.2、AndroidX 与 Cordova 相关组件。APK 的 `assets/public/assets/` 随附角色、MIT、Apache-2.0 和二维码组件声明。 |
| 封面 | 来自项目已有的 2026 年 11 月 22 日宣传图，以已采用的 OO 形象与手机版界面为参考。 |

## Windows 对应源码

- 应用的 Python 源码、构建脚本、用例和素材说明见 [Windows 源码 ZIP](https://github.com/Ori3570/oo-fish-hut/releases/download/v2026.11.22/oo-fish-hut-windows-0.7.1-clean-source.zip)。构建入口和环境版本见包内的 README 与 `requirements-build.txt`。
- 应用随包使用未修改的 Qt 6.11.1 和 PySide6/Shiboken 6.11.1，对应完整源码由 Qt 提供。 [Qt 6.11.1 源码](https://download.qt.io/official_releases/qt/6.11/6.11.1/single/) · [PySide6/Shiboken 6.11.1 源码](https://download.qt.io/official_releases/QtForPython/pyside6/PySide6-6.11.1-src/)
- Windows 将 PySide6 的 Qt 库和插件作为独立文件随 `_internal` 提供。按 LGPL 的条款，可以调试和替换这些库。要试用修改版本，可先通过上述源码构建与原包 ABI 兼容的 Windows x64 版本，保留原文件备份，再将对应的库和插件按原相对路径替换。许可全文与各包元数据见 `licenses/`。
