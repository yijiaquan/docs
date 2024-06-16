## 1.内核替换

### 下载内核

打开最新的 mihomo 的项目下载地址：https://github.com/MetaCubeX/mihomo/releases，这里我使用的是预发布版本 [Prerelease-Alpha](https://github.com/MetaCubeX/mihomo/releases/download/Prerelease-Alpha/mihomo-windows-amd64-alpha-50d60cb.zip)

### 替换

1. 打开`Clash for Windows`安装目录的 `resources\static\files\win\x64`， 备份默认的Clash Premium内核 `clash-win64.exe` ，将第一步解压的mihomo内核程序复制进来， 并重命名为 `clash-win64.exe`

2. 打开`Clash for Windows`，提示： **无法连接到 Clash core 核心**

3. 解决无法连接到核心

   - 退出`Clash for Windows`，打开自带的文件资源管理器，在地址栏输入 `%USERPROFILE%/.config/mihomo` 进入文件夹

   - 删除`mihomo`目录

   - 打开 **powershell** ，执行以下命令

      ```shell
      cmd /c mklink /d "%USERPROFILE%\.config\mihomo" "%USERPROFILE%\.config\clash"
      ```

4. 重新打开`Clash for Windows`内核，主页Clash 核心版本显示 **UnKnown** 就是替换完毕了

## 2.Clash for Windows替换成Clash Verge（其他默认Clash Meta内核也行）

https://github.com/clash-verge-rev/clash-verge-rev.git
