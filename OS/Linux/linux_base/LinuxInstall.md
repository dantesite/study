# Linux 系统介绍与安装

## 1、 Linux系统的简介

Linux是一套免费使用和自由传播的类Unix操作系统，是一个基于POSIX和UNIX的多用户、多任务、支持多线程和多CPU的操作系统。它能运行主要的UNIX工具软件、应用程序和网络协议。支持32位和64位硬件。Linux继承了Unix以网络为核心的设计思想，是一个性能稳定的多用户网络操作系统。

Linux存在着许多不同的Linux版本，但它们都使用了Linux内核。Linux可安装在各种计算机硬件设备中，比如手机、平板电脑、路由器、视频游戏控制台、台式计算机、大型机和超级计算机。

###  1.1、 Linux的发展历程

  (1)1984年，Andrew S.Tanenbaum 开发了用于教学的Unix系统，命名为Minux。

  (2)1989年，AndrewS.Tanenbaum 将MINIX系统运行于X86的PC计算机平台。

  (3)1990年，芬兰赫尔辛基大学学生Linus Torvalds首次接触MINIX系统。

  (4)1991年，Linus Torvalds开始在MINIX上編写各种驱动程序等操作系统内核组件。

  (5)1991年底，Linus Torvalds 公开了Linux 内核源码0.02 版。

  注意：这里公开的linux内核源码并不是现在我们使用的Linux系统全部，而仅仅是Linux内核kernel部分的代码。

  (6) 1993年，Linux 1.0版发行，Linux 转向GPL 版权协议。

  (7) 1994年，Linux 的第一个商业发行版Slackware 问世。

  (8) 1995年，Red Hat软件公司成立，同年发布了Red Hat Linux 2.0。

  (9) 1996年，美国国家标准技术局的计算机系统实验室确认Linux 版本1.2.13 (由Open Linux 公司打包)符合POSIX 标准。

  (10)1997年，Red Hat Linux 5.0 发布，它支持 Intel、alpha、Sparc平台和大多数的应用软件。极其简单易用的RPM模块化的安装、配置和卸载工具，使程序的安装可在15分钟内完成，软件升级也方便了。

  (11)1999年，Linux的简体中文发行版问世。

  (12)2003年4月，Red Hat Linux 9.0 发布。重点放在改善桌面应用方面，包括改进安装过程、更好的字体浏览、更好的打印服务等。2003年，Red Hat 的 Linux 市场份额为80%+。

  (13)2004年4月，Red Hat 公司正式停止对 Red Hat 9.0 版本的支持，标志着 Red Hat Linux 的正式完结。原本的桌面版 Red Hat Linux 发行包则与来自民间的 Fedora 计划合并，成为 Fedora Core 发行版本。Red Hat 公司不再开发桌面版的Linux发行包，而将全部力量集中在服务器版的开发上，也就是 Red Hat Enterprise Linux 版。

  (14)2005年10月，RHEL4发布。

  (15)2007年3月，主流版本RHEL5发布。CentOS系统开始在中国互联网公司流行。

  (16)2010年4月，RHEL6 beta 测试版发布。

  (17)2014年6月，RHEL7发布，RHEL7.0版本和RHEL6.0以前的版本有了较大的变化，例如，内核版本升级到3.10以上，系统启动和基本管理变化较大，文件系统也由ext改为xfs，同时在大数据、云计算、Docker方面做了很大的优化。

### 1.2、Linux发行版本介绍

![image-20210615145802252](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615145802.png)

### 1.3、特点

**==第一大特性：免费使用==**

任何个人和企业都可以免费拿来使用，因为他的源代码对所有人开放，通过自由的修改和发布，同时还遵循GNU许可证，内核的开放，造就了一大批开源软件，可以拿来供大家使用，方便个人和企业的使用，可以完成更高级的任务。

**==第二大特性：多用户、多任务==**

Linux能够同时支持多用户，各个用户能够对自己的文件设备和数据很好的管理权限，保证了各用户之间互不影响。多任务则是现在电脑最主要的一个特点，Linux可以使多个程序同时并独立地运行，互不干涉，协同完成更多的任务。

**==第三大特性：安全性及可靠性好==**

内核高效稳定。Linux内核的高效和稳定已在各个领域内得到了大量事实的验证。Linux中大量网络管理、网络服务等方面的功能，可使用户很方便地建立高效稳定的防火墙、路由器、工作站、服务器等。为提高安全性，它还提供了大量的网络管理软件、网络分析软件和网络安全软件等。

**==第四大特性：广泛的硬件支持==**

由于世界范围内有众多开发者在为Linux的扩充贡献力量，所以Linux有着异常丰富的驱动程序资源，支持各种主流硬件设各和最新的硬件技术，Linux能支持x86、ARM、MIPS、ALPHA和PowerPC等多种体系结构的微处理器。已成功地移植到数十种硬件平台，几乎能运行在所有流行的处理器上。

## 2、 系统安装

### 1.1、 软件环境准备

宿主机环境：Windows 1909版本

虚拟机软件：VMware workstation 16

Linux系统版本：CentOS7 2009

### 1.2、创建虚拟机

点击新建虚拟机

![image-20210615185654255](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615185654.png)

选择自定义可以根据自己的实际情况修改虚拟机的配置信息

![image-20210615185808619](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615185808.png)

选择稍后安装操作系统，如果选择“安装程序光盘映像文件”会自动安装操作系统，无法学习安装操作系统的过程。

![image-20210615185908222](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615185908.png)

系统类型选择 Linux 版本选择 CentOS7 64位 ，这样选择的好处就是虚拟机软件会帮我们对虚拟机进行优化。

![image-20210615190118076](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615190118.png)

虚拟机名称可以根据自己的爱好选择，但是位置不要随意选择，虚拟机文件会随着系统的使用越来越大，最好选择电脑硬盘空间比较大的分区。

![image-20210615190310642](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615190310.png)

根据电脑配置修改虚拟机的CPU信息，一般分配的CPU数量不能高于宿主机（物理机）的线程数，我电脑是12线程的CPU，所以我给虚拟机分配2核CPU；如果你的电脑是4线程，分1核CPU就可以了。

![image-20210615190442898](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615190442.png)

分配虚拟机的内存空间，由于我的电脑物理内存为32G，所以我这里分配4G内存给虚拟机使用；如果你的电脑内存为4G，那么建议分配2G一下的内存给虚拟机，预留2G内存给Windows宿主机使用。

![image-20210615190753065](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615190753.png)

选择虚拟机使用的网络，

>  桥接网络：虚拟机和物理使用同段的地址，网络中其他的机器可以访问虚拟机。
>
> NAT网络：虚拟机通过NAT转换为物理机IP地址上网，网络中其他机器不能访问虚拟机。
>
> 仅主机网络：只能虚拟机和物理机相互访问，不能访问处物理机以外的其他网络资源，网络中其他机器不能访问虚拟机。
>
> 不使用网络：不给虚拟机分配网卡。

![image-20210615191038343](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615191038.png)

使用默认配置

![image-20210615191538291](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615191538.png)

使用默认配置

![image-20210615191609733](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615191609.png)

创建新的虚拟磁盘

![image-20210615191647473](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615191647.png)

修改默认最大磁盘空间大小，立即分配所有磁盘空间：创建完虚拟机后立即为虚拟机分配指定的磁盘空间，单个文件：就是把虚拟磁盘文件保存为一个文件，多个文件：就是把虚拟磁盘文件保存为多个文件，这里把磁盘大小修改了，其他保存默认就可以了。

![image-20210615191738518](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615191738.png)

这里可以修改创建的虚拟磁盘名称，直接使用默认名称就可以了。

![image-20210615192351086](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615192351.png)

点击完成，就完成了虚拟机的创建

![image-20210615192435481](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615192435.png)

可以在左侧看到虚拟机的硬件配置信息

![image-20210615192615836](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615192616.png)

### 1.3、安装 CentOS7 系统

#### 1、挂载镜像

首先需要在虚拟机的CD/DVD光驱加载 CentOS 7 2009 系统的镜像文件，点击“编辑虚拟机设置”

![image-20210615192859710](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615192859.png)

依次打开“CD/DVD”--->”浏览“--->找到镜像文件位置选中，点击“打开”

![image-20210615193116990](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615193117.png)

然后点击确定，完成镜像的挂载，注意“启动时连接”要勾选上。然后点击确定，就可以开机安装系统了。

![image-20210615193306322](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615193306.png)

点击开启虚拟机

![image-20210615193431488](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615193431.png)

#### 2、 安装系统

开机会自动进入到如下界面，默认选中的是测试安装媒介并安装系统，需要在黑色屏幕部分点击下鼠标，然后按上下键切换，选中“Install CentOS7 ”按Enter，

> 注意：如果需要操作Windows系统，同时按下“Ctrl”和“Alt”可以将鼠标由虚拟机切换到Windows系统中

![image-20210615193602178](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615193602.png)

默认安装为英文版，我们使用默认，不做修改，点击`Conttinue`

![image-20210615193957788](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615193957.png)

选中网络配置，默认不启用网络配置，需要我们手动开启网络配置。

![image-20210615194152647](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615194152.png)

输入主机名称点击`Apply`是配置的主机名生效，点击`Congiguretion`配置网络信息

![image-20210615194342160](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615194342.png)

配置网卡连接时自动启用

![image-20210615194451398](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615194451.png)

系统默认为自动获取，一般服务器使用静态地址，需要我们修改，然后点击`Add`添加地址配置，在`Address`输入分配给虚拟机的IP地址，`Netmask`输入子网掩码`Gateway`输入该网段的网关地址`DNS Server`输入DNS信息，然后点击`Save`保存配置

![image-20210615194710260](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615194710.png)

检查配置和我们分配的地址信息是否一致，如果一致点击`Done`完成网络配置，如果不一致再次点击`Congiguretion`修改配置即可

![image-20210615195054912](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615195055.png)

选择使用的磁盘和磁盘分区

![image-20210615195248147](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615195248.png)

如果对硬盘分区没有特殊要求可以使用系统默认分区，也可以根据需要选择手动分区，这里使用系统的默认分区。

![image-20210615195343595](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615195343.png)

选择服务器安装的模式，最小化，带GUI的服务器，还是其他需要自定义的服务器；这里我使用默认配置最小化安装

![image-20210615195531475](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615195531.png)

在地图上选择需要设置的时区，一般使用的是亚洲上海时区，开启使用同步，时间同步在实际生产环境和集群环境下是非常重要的。

![image-20210615195958346](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615195958.png)

修改NTP服务器地址，如果服务器可以连接互联网络可以使用互联网上的NTP服务器同步时间；在内网环境，如果条件允许，建议使用专业的NTP服务器作为NTP服务器使用，如果没有也可以在内网搭建一台NTP服务器为网络内其他服务器同步时间；配置完成点击`OK`是配置生效。

![image-20210615200327278](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615200327.png)

配置完成后点击`Done`完成时区选择和时间配置。

![image-20210615200439361](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615200439.png)

点击`Begin Installation`开始系统安装

![image-20210615200526816](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615200526.png)

打开`ROOT PASSWORD`配置root用户的登录密码；也可根据需要创建sudo管理员用户。

![image-20210615200620799](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615200620.png)

如果输入的密码为简单密码或者系统认为密码为简单密码，需要点击两次`Done`完成`root`用户密码的设置。

![image-20210615200826240](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615200826.png)

系统安装完成后点击`Reboot`重启系统，完成系统安装，实际生产环境下取下系统安装介质比如U盘，光盘等

![image-20210615201333433](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615201333.png)

最小化安装系统启动的界面

![image-20210615201543120](https://danteitnote.oss-cn-chengdu.aliyuncs.com/picgo/20210615201543.png)
