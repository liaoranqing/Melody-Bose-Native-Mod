# Melody Bose Native Mod

独立的 Melody 17.6.3 魔改工程，目标是在原生 `com.oplus.melody` 中加入 Bose QC Earbuds Ultra 2 控制支持。

## 目标

- 保留原 Melody 包名与原生界面结构
- 接入 Bose BMAP RFCOMM channel 2
- 支持关闭、降噪、通透、CNC 与空间音频
- 不加入不支持的抗风噪功能
- 优先使用 GitHub Actions 完成反编译、注入、重打包和构建

## 构建方式

1. 将 `original/original-melody.apk` 提交到私有仓库或通过安全的 Actions 输入提供。
2. 打开 GitHub Actions，运行 `Build Modded Melody`。
3. 等待构建完成后，从 Artifacts 下载修改版 APK。
4. 修改版 APK 需要在临时 root 测试机上验证签名、安装和系统兼容性。

## 当前限制

- 这是系统应用的重新打包版本，重新签名后可能无法覆盖原系统包。
- 不能保证 ColorOS 的签名校验、特权权限和系统更新兼容性。
- APK 魔改和现有 LSPosed 模块是两条独立路线，建议先保留原版 APK 备份。
