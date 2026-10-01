# Bose 注入补丁

这里放 Melody Smali 注入补丁。

目标入口：

- `EarphoneControlProvider`：模式、CNC、空间音频
- `BatteryProvider`：左耳、右耳、充电盒电量
- `BluetoothService`：Bose BMAP RFCOMM channel 2

当前仓库只完成解码、入口验证、重打包和测试签名流程。正式注入前必须针对这份 Melody 17.6.3 APK 验证 Smali 方法签名，避免把旧版类名或寄存器布局直接套入新版本。
