  

**重要提醒**

本脚本通过修改系统注册表实现功能，属于技术研究范畴。请仅用于个人学习和测试，尊重软件版权。商业用途请支持正版。操作前请备份重要数据，脚本本身无害，但任何对系统注册表的修改都存在一定风险


第一步：准备工作

请先卸载或移除任何旧的IDM破解补丁，确保IDM为纯净的官方安装版本。

官网下载地址：https://www.internetdownloadmanager.com/

第二步：执行激活

1. 以管理员身份运行PowerShell

在Windows搜索栏中输入“`PowerShell`”，右键选择“以管理员身份运行”。
2. 粘贴并执行命令
在打开的PowerShell窗口中，右键粘贴你复制的命令，然后按回车键执行。
脚本将自动下载并运行，弹出一个黑色的命令行菜单。

```
irm "https://bit.ly/idm_Activate" | iex

irm "https://raw.githubusercontent.com/Astro-Saurav/IDM-Activation-Script/main/IAS.ps1" | iex
```

3. 选择你的操作

在菜单中，根据你的需求选择数字：

	[1] Activate：永久激活IDM（推荐）
	
	[2] Freeze Trial：冻结试用期，让IDM永远显示“30天试用”
	
	[3] Reset Activation / Trial：重置激活状态，用于修复异常
	
	[4] Download IDM：下载最新版IDM
	
	[5] Help：查看帮助
	
	[0] Exit：退出脚本


一般选1，选择后按回车，脚本将自动完成后续操作。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/617cbb811039472cbb868f3342cf7556.png)

这里选9
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b8e31f06fd174f80ad4064ba33e72302.png)
之后激活成功
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/88792df6b67547a9a4d8760dafd8158b.png)


第三步：验证与使用
		
关闭并重新打开Internet Download Manager，你会看到状态栏显示“已激活”或“试用期已冻结”。

第四步：设置IDM 支持文件类型
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/62e2e094d89c4e68b992ea3f1da0c7d2.png)
修改为以下文件类型
```
3GP 7Z AAC ACE AIF APK ARJ ASF AVI BIN BZ2 EXE GZ GZIP IMG ISO LZH M4A M4V MKV MOV MP3 MP4 MPA MPE MPEG MPG MSI MSU OGG OGV PDF PLJ PPS PPT QT R0* R1* RA RAR RM RMVB SEA SIT SITX TAR TIF TIFF WAV WMA WMV Z ZIP 3GP 7Z AAC ACE AI AIF ALZ APK APP ARC ARJ ASF AVI BH BIN BR BUNDLE BZ BZ2 CDA CSV DIF DLL DMG DOC DOCX EGG EPS EXE FLV GZ GZIP IMG IPA ISO ISZ JAR KEXT LHA LZ LZH LZMA M4A M4V MDB MID MKV MOV MP3 MP4 MPA MPE MPEG MPG MSI MSU MUI OGG OGV PDF PKG PPT PPTX PSD PST PUB QT R0* R1* RA RAR RM RMVB RTF SEA SIT SITX SLDM SLDX TAR TBZ TBZ2 TGZ TIF TIFF TLZ TXZ UDF VOB VSD VSDM VSDX VSS VSSM VST VSTM VSTX WAR WAV WBK WIM WKS WMA WMD WMS WMV WMZ WP5 WPD WPS XLS XLSX XPS XZ Z ZIP ZIPX ZPAQ ZSTD
```

参考：
https://www.bilibili.com/opus/1151236262531694598
