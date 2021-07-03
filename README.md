# Grey 一键多开脚本(Windows)
### ・使用说明：  
####  1.下载并解压缩
####  2.下载最新版的Grey执行程序并将其解压缩到步骤1下载并解压的Grey/Grey01/01文件夹
####  3.复制粘贴Grey/Grey01/01文件夹并修改名称为02~50（每个文件夹对应一个Grey节点，根据要开的节点创建文件夹数量，确保所有文件夹都有Grey执行程序）
####  4.安装步骤1下载并解压的Grey/沙盒程序
####  5.执行沙盒程序，点击

# zkTube 一键多开脚本
##### ・一键脚本运行方法(整行复制粘贴执行)：
###### ・Ubuntu：
##### ___`sudo apt update && sudo apt-get install wget curl`___
##### ___`wget https://raw.githubusercontent.com/topmininglabs/zktube/main/topmining_zktube.sh && chmod +x ./topmining_zktube.sh && sudo ./topmining_zktube.sh`___
###### ・CentOS：
##### ___`sudo yum update && sudo yum install wget curl`___
##### ___`wget https://raw.githubusercontent.com/topmininglabs/zktube/main/topmining_zktube.sh && chmod +x ./topmining_zktube.sh && sudo ./topmining_zktube.sh`___

##### ・注意事项1：此脚本仅支持Ubuntu系统和CentOS系统
##### ・注意事项2：此脚本虽可实现一地址多节点，鉴于官方尚未明确指出是否支持一个地址多开节点，使用此脚本多开的需自行承担风险（可能会有无收益或收益被清零的风险）
##### ・注意事项3：关于系统配置要求，请参照下面官方说明：
###### zkTube矿机配置是建议32核64G（该配置上考虑了部分弹性预留，主要是为了避免复杂证明的计算可能带来的计算消耗溢出，引发Prover异常，从而触发prover挖矿惩罚机制，造成不必要的损失）。我们所采用的是当网络有使用的时候才会有区块产生，也就是当一个交易或者是一个任务抛出的时候需要带宽去抢任务，带宽越高抢到任务的概率越高，当任务抢到并计算完成的时候才会有奖励。真正做到了没有垃圾数据而且不会一直高消耗的空跑CPU。
##### ・注意事项4：本脚本可无限制多开节点，请根据自身系统配置自行决定多开节点数量，操作选项（5）若输入1节点则只部署一个节点
##### ・注意事项5：多开节点数量过多有可能导致系统奔溃或无法运行，请自行承担风险
