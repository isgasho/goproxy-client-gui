# goproxy-client-gui for windows
### 本gui程序基于https://github.com/snail007/goproxy 的客户端程序开发

### 快速使用

1、确保已配置好goproxy-client端【[下载](https://github.com/snail007/goproxy/releases)】的bootstrap.bat文件（即确保proxy可正常使用）

2、[下载gpclient](https://github.com/fuhuo/goproxy-client-gui/releases)的最新版zip压缩包

3、把gpclient压缩包解压到goproxy-client同目录

4、找到合适的pac.txt文件（可以直接拿ss客户端的，[参考这个](https://github.com/fuhuo/pac/blob/master/pac.txt)），放到goproxy-client目录

5、双击打开gpclient.exe小托盘->右键，点击【设置】-【端口】，proxy端口配置成与你boostrap.bat的-p参数的端口一致，pac服务端口随意配置，但不能与系统其他服务的端口（包括proxy的端口）重复，以免被占用导致不可用

6、通过gpclient.exe小托盘->右键，选择“关闭代理”、“pac模式”和“全局模式”等模式使用。

### 程序说明

1、本程序使用ahk和go开发，暂时只支持windows（只在win10的64位系统测试过）

2、本程序通过调用goproxy-client的start.vbs启用proxy.exe，安全退出时会关闭proxy.exe

### 已知问题

~~1、之前没考虑好端口的问题，目前只能是goproxy中使用1080端口作为代理端口，后续会优化~~

~~2、pac的http server端口也写死了1079，这两个端口如果有冲突，目前需要自己下载ahk脚本并用autohotkey进行重新编译成exe，后续会优化~~

~~3、有时候会出现系统代理配置不完整的情况，需要手动重新切换一下模式，待解决~~

4、目前仅支持单个服务配置

### 遇到问题

如果使用过程中遇到任何问题，欢迎在[issues](https://github.com/fuhuo/goproxy-client-gui/issues)提出

