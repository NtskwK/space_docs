# 清理休眠文件

## hiberfil.sys

参考[Powercfg 命令行选项](https://learn.microsoft.com/zh-cn/windows-hardware/design/device-experiences/powercfg-command-line-options#option_hibernate) by Microsoft

关闭休眠

```powershell
powercfg -h off
```

开启休眠

```powershell
powercfg -h on
```

调整休眠文件大小（不能低于 50%）

```powershell
powercfg -h -size 50
```
