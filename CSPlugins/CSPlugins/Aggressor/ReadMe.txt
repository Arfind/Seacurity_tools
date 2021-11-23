Cscan 5.4
Update 20191101
Author K8gege
===============================================================================================

@使用说明
https://github.com/k8gege/K8CScan/wiki
===============================================================================================

@程序简介
===============================================================================================
K8Cscan一款专用于大型内网渗透的高并发插件化扫描神器，包含信息收集、网络资产、漏洞扫描、密码爆破、漏洞利用，
支持批量A段/B段/C段以及跨网段扫描。5.4版本内置28个功能模块,通过各种协议以及方法快速获取目标网络存活主机IP、
计算机名、工作组、网络共享、网卡物理地址、操作系统版本、网站域名、Web中间件、路由器（Cisco）、数据库等网络资产信息,
内置MS17-010(SMB漏洞)、Weblogic、ActiveMQ漏洞检测，内置6种密码认证爆破3种数据库(Mysql、Oracle、MSSQL)、FTP密码爆破(文件服务器)、
SSH密码爆破(Linux主机)、IPC/WMI两种方式爆破Windows主机密码，Web指纹识别模块可识别62种Web应用。
高度自定义插件支持.NET程序集、DLL(C#/Delphi/VC)、PowerShell等语言编写的插件以及无编程功底通过配置INI加载任意程序命令
，可快速扩展扫描或利用能力。支持Cobalt Strike联动内存加载Cscan功能扫描内网或跳板扫描外网，可快速拓展内网进行横向移动。
===============================================================================================

@程序功能
===============================================================================================
支持指定IP扫描
支持指定C段扫描(ip/24)
支持指定B段扫描(ip/16)
支持指定A段扫描(ip/8)
支持指定URL扫描
支持批量IP扫描(ip.txt)
支持批量C段扫描(ip24.txt)
支持批量B段扫描(ip16.txt)
支持批量URL扫描(url.txt)
支持批量域名扫描(domain.txt)
支持批量主机扫描(host.txt)
支持批量字符串列表(str.txt)
支持指定范围C段扫描
支持参数加载自定义DLL（仅限C#）
支持参数加载自定义EXE（仅限C#）
支持自定义程序(系统命令或第三方程序即任意语言开发的程序或脚本)
支持自定义模块(支持多种语言编写的DLL/.NET程序集/PowerShell脚本)
支持Cobalt Strike(beacon命令行下扫描目标内网或跳板扫描外网目标)


@模块功能
===============================================================================================
模块插件 MS170101 		SMB漏洞扫描[5.0内置]
模块插件 UrlScan 		URL域名扫描[5.0内置]
模块插件 SameWeb 		同服域名扫描[5.0内置]
模块插件 CiscoScan 		Cisco思科设备扫描[5.0内置]
模块插件 WebScan 		Web信息扫描[5.0内置]
模块插件 WebScan2		Web信息扫描含CMS[5.0内置]
模块插件 WeblogicPoc	Weblogic漏洞检测[5.0内置]
模块插件 WeblogicExp	Weblogic漏洞利用[5.0内置]
模块插件 OSScan 		系统版本探测[5.0内置]
模块插件 FtpScan 		Ftp密码扫描[5.0内置]
模块插件 MysqlScan 		Mysql密码扫描[5.0内置]
模块插件 OnlinePC 		存活主机扫描[5.0内置]
模块插件 OnlineIP 		仅存活主机IP[5.0内置]
模块插件 WebBanner 		内网Web信息扫描[5.0内置]
模块插件 WmiScan 		Wmi爆破Windowns密码[5.0内置]
模块插件 SameWeb 		C段旁站扫描[5.0内置]
模块插件 PortScan.cs 	端口扫描插件源码
模块插件 HostIP 		域名解析/主机名转IP[5.0内置]
模块插件 C# netscan 	存活主机 & Web信息插件成品&源码
模块插件 Base64Enc(EXE) Base64加密(c#程序)
模块插件 Base64Dec(EXE) Base64解密(c#程序)
模块插件 HexDec(PSH)	Hex解密(PowerShell脚本)
模块插件 Base64Dec(PSH)	Base64解密(PowerShell脚本)
模块插件 MssqlScan 		Mssql数据库密码爆破[5.0内置]
模块插件 OracleScan 	Oracle数据库密码爆破[5.0内置]
模块插件 SSHscan 		SSH密码爆破(Linux)[5.0内置]
模块插件 EnumMssql 		枚举Mssql数据库主机[5.0内置]
模块插件 EnumShare 		枚举网络共享资源[5.0内置]
模块插件 IpcScan 		Ipc爆破Windows密码[5.0内置]
模块插件 SmbScan 		SMB爆破Windows密码[5.0内置]
模块插件 OracleScan 	Oracle数据库密码爆破[5.0内置]
模块插件 WhatCMS 		75种Web指纹识别[5.0内置]
模块插件 EnHex/DeHex 	批量Hex密码加密解密[5.0内置]
模块插件 EnBase64		批量Base64密码加密[5.0内置]
模块插件 DeBase64 		批量Base64密码解密[5.0内置]
模块插件 PhpStudyPoc 	PhpStudy后门检测[5.0内置]
模块插件 SubDomain 		子域名爆破[5.3内置]
模块插件 WebDir 		后台目录扫描[5.3内置]
模块插件 DomainIP 		批量域名解析[5.3内置]	
模块插件 ActiveMQPoc 	ActiveMQ漏洞检测[5.4内置]	
模块插件 TomcatPoc 		Tomcat漏洞检测[5.4内置]	

