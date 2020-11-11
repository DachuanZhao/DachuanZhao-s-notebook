```
#以 管理员身份 打开 PowerShell 并运行
Enable-WindowsOptionalFeature -Online -FeatureName VirtualMachinePlatform

#查看现有地 WSL
wsl -l -v

#使用命令行将 WSL 1 的发行版转化为 WSL2、在 PowerShell 中运行
wsl --set-version 已经使用的WSL的名字 2

#设置WSL 2 成为你的默认体系结构
wsl --set-default-version 2

```

