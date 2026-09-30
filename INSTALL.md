# Vlai 小红书自动化安装说明

当前发布版本：0.5.24（现场验证版）。适用于 Windows 10/11 64 位，需要配合安卓设备使用。

1. 在 [Releases](../../releases) 中下载 `VlaiXhsAutomation-Setup-0.5.24.exe`；需要离线保存说明材料时，可下载 `VlaiXhsAutomation-Customer-Package-0.5.24.zip`。两种下载方式使用同一 EXE，无须重复安装。
2. 下载 `SHA256SUMS.txt`，在 PowerShell 中运行 `Get-FileHash -Algorithm SHA256 -LiteralPath '下载文件的完整路径'` 并比对校验值。
3. 运行安装程序，按安装向导和首次安装引导完成电脑端准备。
4. 连接安卓手机，在手机上手动开启开发者选项、USB 调试，确认 USB 调试授权，并开启 Portal 的无障碍服务。安装向导会使用内置组件完成手机端软件安装。
5. 按应用提示完成许可证、设备和任务配置。执行自动化任务前，先在受控设备上验证启动、停止和目标账号。

客户交付 ZIP 包含安装程序和使用指南，已排除 `03_安卓配套` 与 `04_Windows配套`。原有 0.5.3 使用指南提供功能操作参考；0.5.24 的变更以 ZIP 内的《0.5.24 修复与交付说明》为准。

安装包没有 Windows 发布者代码签名，系统可能提示“未知发布者”。请确认下载地址位于 `github.com/vlaipro/VlaiXhsAutomation-releases`，且文件校验值一致。0.5.24 已完成离线测试与打包校验，仍需在目标电脑和安卓设备上完成安装及长时间真机验证。
