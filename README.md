# Grey 一键多开脚本(Windows)
#### ■ 使用说明：  
##### 1.下载并解压缩[Grey-windows-auto.zip](https://github.com/topmininglabs/Grey/raw/main/Grey-windows-auto.zip)文件包,将解压缩完成的文件夹“Grey-windows-auto”移动到C盘根目录下
##### 2.下载最新版的[Grey](https://greycloud.oss-accelerate.aliyuncs.com/Grey/WindowsGrey0.0.7.zip)执行程序并将其解压缩到步骤1下载并解压完成的”C:\Grey-windows-auto\Grey01\01“文件夹里
##### 3.复制粘贴”C:\Grey-windows-auto\Grey01\“目录下的”01“文件夹并修改名称为02~50（每个文件夹对应一个Grey节点，根据要多开的节点数创建文件夹数量，确保所有文件夹都有Grey执行程序）
##### 4.安装步骤1下载并解压完成的”C:\Grey-windows-auto\1.Install-Sandboxie-Plus-x64-v0.8.2.exe“沙盒程序
##### 5.打开步骤1下载并解压完成的”C:\Grey-windows-auto\02.Config-Sandbox-confing-50box.txt“文件，Ctrl+A选中所有内容，Ctrl+C复制所有内容
##### 6.打开沙盒程序，点击”Option->Edit ini file“，跳出记事本后Ctrl+A选中所有内容，按删除键删除所有内容，Ctrl+V将步骤5复制的内容全部粘贴到该文件，Ctrl+S保存并关闭（此时沙盒程序会自动生成50个沙盒，如未出现请重复步骤4-6）
##### 7.双击下载并解压完成的”C:\Grey-windows-auto\03.Run-Grey_Script.bat“脚本文件自动启动运行50个Grey节点
#### ■ 注意事项：  
##### 1.此脚本仅适用于未安装和执行过Grey程序的Windows系统，运行此脚本之前若单独运行过Grey程序则生成的所有节点将使用同一个地址且仅一个节点运行有效
##### 2.为防止Grey节点掉线超过12小时导致收益清零，此脚本每4个小时会自动重启Grey节点
##### 3.此脚本运行后将无限循环执行，若要退出需手动关闭”Grey-windows-auto/03.Run-Grey_Script.bat“脚本的cmd窗口，与启动中的沙盒程序
##### 4.请根据自身系统配置合理选择多开节点数，此脚本默认多开50节点（8核16G内存），如需修改节点数，请修改以下两个文件后再执行此教程的所有操作
```
・文件：”C:\Grey-windows-auto\02.Config-Sandbox-confing-50box.txt”
  第七行：“BoxDisplayOrder=”后面删除或添加相应沙盒数字” 
  文件末尾：删除或添加相应沙盒配置
・文件：”C:\Grey-windows-auto\100.Run50Grey.txt”`  
  文件末尾：删除或添加相应节点运行命令  
```
##### ・以下为添加第51号节点的操作:  
```
・打开文件：”C:\Grey-windows-auto\02.Config-Sandbox-confing-50box.txt” 
  于第七行：“BoxDisplayOrder=”末尾添加数字51，添加后显示如下：
BoxDisplayOrder=01,02,03,04,05,06,07,08,09,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51 

  于文件末尾添加以下51号沙盒配置并保存文件： 
[50]

Enabled=y
AutoRecover=n
BlockNetworkFiles=y
RecoverFolder=%{374DE290-123F-4565-9164-39C4925E467B}%
RecoverFolder=%Personal%
RecoverFolder=%Desktop%
BorderColor=#00FFFF,ttl
Template=OpenBluetooth
Template=SkipHook
Template=FileCopy
Template=qWave
Template=BlockPorts
Template=LingerPrograms
Template=Chrome_Phishing_DirectAccess
Template=Firefox_Phishing_DirectAccess
Template=AutoRecoverIgnore
ConfigLevel=9
DropAdminRights=y
ClosePrintSpooler=y

・打开文件：”C:\Grey-windows-auto\100.Run50Grey.txt” 
  于文件末尾pause之前添加以下51号节点的运行命令并保存文件：
  
start "Grey51" "C:\Program Files\Sandboxie-Plus\Start.exe" /box:51 /silent /nosbiectrl "C:\Grey-windows-auto\Grey01\51\grey.exe"
timeout 10

・双击下载并解压完成的”C:\Grey-windows-auto\03.Run-Grey_Script.bat“脚本文件自动启动运行51个Grey节点

```

##### 5.此脚本仅在Windows10系统执行测试过，不过Windows7系统应该也可以执行
##### 6.多开节点运行的节点收益有被官方清零的风险，请自行承担该风险
##### 7.激活节点需要至少一个GBR代币，可通过官方水龙头[官方水龙头](https://faucet.ethgrey.com/)申请一个代币，也可到各微信群/QQ群找水商买水
#### ■ 常用链接：  
##### 1.Grey官网：https://ethgrey.org/
##### 2.Grey区块浏览器：https://www.ethgrey.com/
##### 3.Grey官方水龙头：https://faucet.ethgrey.com/
##### 4.Sandbox沙盒程序官网：https://sandboxie-plus.com/

