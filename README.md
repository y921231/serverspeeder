# serverspeeder锐速一键破解安装版


破解版锐速linux一键自动安装包在本贴持续更新，大家可以加收藏夹，以后有更新都会在这个文章同步。

本破解锐速是是无限带宽版的，破解版锐速的一些代码将逐步开源在github这里。

锐速破解版自动安装过程中有什么问题都可以留言，我尽量解答。

# 特别说明
另外：重要的事情说三遍！！！

锐速不支持Openvz！！！锐速不支持Openvz！！！锐速不支持Openvz！！！

### 你可能需要：
* 如果你不知道你的机子到底是不是Openvz，请食用[《教程：一键检测VPS是Openvz还是KVM还是Xen》](http://www.91yun.org/archives/836)
* 如果你的内核不对，是Centos的话请食用[《教程：CentOS更换内核，提供锐速可用的内核下载》](http://www.91yun.org/archives/795)。debian和ubuntu我不熟，暂时还没一键包，请自行百度google。。



# 锐速破解版安装方法：
    wget -N --no-check-certificate https://github.com/91yun/serverspeeder/raw/master/serverspeeder.sh && bash serverspeeder.sh
# 锐速破解版卸载方法：
    chattr -i /serverspeeder/etc/apx* && /serverspeeder/bin/serverSpeeder.sh uninstall -f


锐速破解版功能：
如果内核完全匹配就会自动下载安装。
如果没有完全匹配的内核，会在界面提示可选内核，可以手动选个最接近的尝试
自动下载授权文件
自动修改配置文件
已chattr +i /serverspeeder/etc/apx*禁止修改配置文件，可以不用加hosts了
目前只支持CentOS，ubuntu和debian。如果有其他系统支持，可以到[91yun.org我的博客](http://www.91yun.org/serverspeeder91yun)手动下载其他系统的安装包

service serverSpeeder start #启动
service serverSpeeder stop #停止
service serverSpeeder reload #重新加载配置
service serverSpeeder restart #重启
service serverSpeeder status #状态
service serverSpeeder stats #统计
service serverSpeeder renewLic #更新许可文件
service serverSpeeder update #更新
chattr -i /serverspeeder/etc/apx* && /serverspeeder/bin/serverSpeeder.sh uninstall -f #卸载
