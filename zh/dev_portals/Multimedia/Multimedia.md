**关注译者公众号**：
<br/>
<img src='../../../pic/tinylab-wechat.jpg' width='110px'/>
<br/>


> 原文：[eLinux.org](http://eLinux.org/Multimedia "http://eLinux.org/Multimedia")<br/>
> 翻译：[@lzufalcon](https://github.com/lzufalcon)

# 多媒体

## 目录

-   [1 简介](#introduction)
-   [2 CELF 2.0 AVG（Audio, Video, Graphic） 规范](#celf-2-0-specification-for-avg)
-   [3 音、视频工作组](#audio-video-working-group)
-   [4 DirectFB 研究](#directfb-study)
    -   [4.1 什么是 DirectFB，DirectFB 如何工作](#what-is-directfb-how-does-directfb-work)
    -   [4.2 嵌入式 Linux 平台上的 DirectFB 示例实现](#sample-implementation-of-directfb-on-an-embedded-linux-platform)
    -   [4.3 嵌入式 Linux 平台上的一些 DirectFB 基准测试结果](#some-directfb-benchmark-on-embedded-linux-platform)
-   [5 相关项目](#related-projects)
    -   [5.1 图形/视频输出](#graphics-video-out)
        -   [5.1.1 Framebuffer](#framebuffer)
        -   [5.1.2 DirectFB](#directfb)
        -   [5.1.3 V4L2](#v4l2)
        -   [5.1.4 X11](#x11)
        -   [5.1.5 NanoX](#nanox)
        -   [5.1.6 OpenGL (OpenML)](#opengl-openml)
        -   [5.1.7 SDL](#sdl)
        -   [5.1.8 Cairo](#cairo)
        -   [5.1.9 Clutter](#clutter)
        -   [5.1.10 Enlightenment Foundation Libraries (EFL)](#enlightenment-foundation-libraries-efl-http-elinux-org-efl-efl)
        -   [5.1.11 Qt](#qt)
        -   [5.1.12 演示图板套件(演示图板设计师/引擎，来自 Crank Software)](#storyboard-suite-storyboard-designer-engine-from-crank-software)
        -   [5.1.13 GStreamer](#gstreamer)
        -   [5.1.14 Xine](#xine)
        -   [5.1.15 MPlayer](#mplayer)
        -   [5.1.16 文档](#documentation)
    -   [5.2 视频输入](#video-in)
        -   [5.2.1 V4L[2]](#v4l-2)
        -   [5.2.2 OpenML](#openml)
        -   [5.2.3 LinuxTV (DVB API)](#linuxtv-dvb-api)
    -   [5.3 音频输入/输出](#audio-in-out)
        -   [5.3.1 OSS](#oss)
        -   [5.3.2 ALSA](#alsa)
        -   [5.3.3 OpenAL](#openal)
        -   [5.3.4 PulseAudio](#pulseaudio)
    -   [5.4 AVG 标准的使用者](#users-of-avg)
        -   [5.4.1 Video Lan](#video-lan)
        -   [5.4.2 Freevo](#freevo)
        -   [5.4.3 LinuxTV](#linuxtv)
        -   [5.4.4 MythTV](#mythtv)
        -   [5.4.5 DVR](#dvr)
        -   [5.4.6 OpenPVR](#openpvr)
        -   [5.4.7 Morphine.TV](#morphine-tv)
    -   [5.5 其他](#other)
        -   [5.5.1 ARIB 架构](#arib-architecture)
        -   [5.5.2 启动动画](#boot-splash)
        -   [5.5.3 数字家庭工作组](#digital-home-working-group)
        -   [5.5.4 Disko 框架](#disko-framework)
        -   [5.5.5 Free Type](#free-type)
        -   [5.5.6 UPnP](#upnp)
        -   [5.5.7 TV Anytime](#tv-anytime)
        -   [5.5.8 TV Linux 联盟](#tv-linux-alliance)


<span id="introduction"></span>

## 简介

本文有 Linux 下的音频、视频、图形系统相关的各类资源。

关于图形系统部分，也可以通过阅读[用户接口](../.././dev_portals/Multimedia/User_Interfaces/User_Interfaces.md "User Interfaces")一节了解更多信息。

<span id="celf-2-0-specification-for-avg"></span>

## CELF 2.0 AVG 规范

（更像是一套建议，而不是一个规范）

-   [AVG 规范 V2](http://eLinux.org/images/4/43/CelfAudioVideoGraphicsSpec2_accepted_20060606.pdf "CelfAudioVideoGraphicsSpec2 accepted 20060606.pdf")

<span id="audio-video-working-group"></span>

## 音、视频工作组

请从 CELF 维基：[AVG 工作组](http://www.celinuxforum.org/CelfPubWiki/AudioVideoGraphicsWorkingGroup) 获取更多信息。

也有一些 AVWG 相关的[但是过期了的文章](../.././dev_portals/Multimedia/Outdated_pages/Outdated_pages.md "Outdated pages")。

<span id="directfb-study"></span>

## DirectFB 研究

<span id="what-is-directfb-how-does-directfb-work"></span>

### 什么是 DirectFB，DirectFB 如何工作

- [DirectFB](../.././dev_portals/Multimedia/DirectFB/DirectFB.md "DirectFB")

<span id="sample-implementation-of-directfb-on-an-embedded-linux-platform"></span>

### 嵌入式 Linux 平台上 DirectFB 示例实现

- [移植 DirectFB](../.././dev_portals/Multimedia/Porting_DirectFB/Porting_DirectFB.md "Porting DirectFB")

<span id="some-directfb-benchmark-on-embedded-linux-platform"></span>

### 嵌入式 Linux 平台上一些 DirectFB 基准测试结果

- [DirectFB 基准测试](../.././dev_portals/Multimedia/Benchmark_DirectFB/Benchmark_DirectFB.md "Benchmark DirectFB")

<span id="related-projects"></span>

## 相关项目

<span id="graphics-video-out"></span>

### 图形/视频输出

<span id="framebuffer"></span>

#### Framebuffer/帧缓冲

-   [Documentation/fb](http://www.kernel.org/doc/Documentation/fb)
-   [http://linuxconsole.sourceforge.net/fbdev/HOWTO/](http://linuxconsole.sourceforge.net/fbdev/HOWTO/)
-   [http://www.tldp.org/HOWTO/Framebuffer-HOWTO.html](http://www.tldp.org/HOWTO/Framebuffer-HOWTO.html)

    帧缓冲用于把帧信息存到视频中……

<span id="directfb"></span>

#### DirectFB

-   [http://www.directfb.org/](http://www.directfb.org/)
-   [http://www.directfb.org/documentation/DirectFB\_overview\_V0.2.pdf](http://www.directfb.org/documentation/DirectFB_overview_V0.2.pdf)
-   [DirectFB](../.././dev_portals/Multimedia/DirectFB/DirectFB.md "DirectFB")

<span id="v4l2"></span>

#### V4L2

-   [http://www.linuxtv.org/](http://www.linuxtv.org/)
-   [http://www.linuxtv.org/downloads/video4linux/API/V4L2\_API/spec-single/v4l2.html](http://www.linuxtv.org/downloads/video4linux/API/V4L2_API/spec-single/v4l2.html)

<span id="x11"></span>

#### X11

-   [http://www.x.org/](http://www.x.org/)
-   [X11](../.././dev_portals/Multimedia/X11/X11.md "X11")

<span id="nanox"></span>

#### NanoX

-   [http://www.microwindows.org/](http://www.microwindows.org/)

<span id="opengl-openml"></span>

#### OpenGL (OpenML)

-   [http://www.opengl.org/](http://www.opengl.org/)
-   [http://www.khronos.org/opengles/](http://www.khronos.org/opengles/)

<span id="sdl"></span>

#### SDL

-   [http://www.libsdl.org/](http://www.libsdl.org/) - 是一个即时图形渲染库，采用了诸如矩形填充和转换这样的非常精简的原语。因为它只暴露了帧缓冲区和少量原语，所以非常容易移植到其他平台，实际上，它产生之初，即是作为一种方式，用于移植 Windows 游戏到 Linux 平台。

<span id="cairo"></span>

#### Cairo

-   [http://www.cairographics.org/](http://www.cairographics.org/) 是另外一个即时图形渲染库，可用于处理复杂的向量图形，包括矩形转换。它运行于 DirectFB、X11、内存缓冲区以及其他设施之上。它是诸多 GTK 工具套件和 Firefox 这样的应用程序的基础。

<span id="clutter"></span>

#### Clutter

-   [http://clutter-project.org/](http://clutter-project.org/) 是构建在 OpenGL（或者 OpenGL-ES）与场景管理之上的一个面向对象的 3D 画板，它基于 GLib/GObject 并很好地匹配 GNOME 平台。很多强大的 Linux 手机在不久的将来，将转向采用基于 Clutter 的接口，像英特尔的 Moblin 平台，Ubuntu Touch 移动平台和 Maemo（译着注：实际上这三个平台两个已经死了，只有 Touch 半死不活，一个系统要真能在实际产品中占有一席之地，还真得是综合实力的考量！）。

<span id="enlightenment-foundation-libraries-efl-http-elinux-org-efl-efl"></span>

#### Enlightenment Foundation Libraries ([EFL](../.././dev_portals/Multimedia/EFL/EFL.md "EFL"))

[The Enlightenment Foundation Libraries](http://www.enlightenment.org/) 包含 Evas，一个构建在 OpenGL/X11, XRender/X11, X11, FB, DirectFB, DirectDraw 等之上的面向对象的 2D 画板。它包括场景管理并且集成了 Ecore，能很好地与 EFL 组件，比如 Edje 匹配。它已经被用于一些媒体中心和 OpenMoko 手机上。

可查看在 2008 年欧洲嵌入式 Linux 会议上的 Gustavo Barbieri 会议：

- [演讲稿](http://tree.celinuxforum.org/CelfPubWiki/ELCEurope2008Presentations?action=AttachFile&do=get&target=Rich_GUI_without_pain.pdf)
- [演讲视频](http://free-electrons.com/pub/video/2008/elce/elce2008-barbieri-rich-gui-without-pain.ogv)，Gustavo 的公司：[ProFUSION](http://profusion.mobi/)，提供围绕 EFL 的服务。

<span id="qt"></span>

#### Qt

-   Qt 是一个跨平台的图形工具套件，支持帧缓冲和 X，拥有先进的动画功能，采用[图形视图](http://doc.trolltech.com/4.5/graphicsview.html)框架。

<span id="storyboard-suite-storyboard-designer-engine-from-crank-software"></span>

#### 演示图板套件 (演示图板设计师/引擎，来自 Crank Software)

-   [http://www.cranksoftware.com/storyboard](http://www.cranksoftware.com/storyboard)

    来自 Crank Software 的演示图板（Storyboard）套件，提供一套完整的环境，可用于设计、开发和部署嵌入式用户接口，支持多种渲染技术（DirectFB，FBDev，SDL，OpenGL，OpenVG，……），支持多种操作系统（Linux，QNX，VxWorks，WinCE/Win32……），跨越多种处理器架构（x86，ARM，PPC，SH……）。该演示图板方法非常独特，它开发时就考虑到如何从图形设计师那里直接加入内容并部署数据集，它也为各类 OS/CPU/渲染技术进行了专门的优化。

<span id="gstreamer"></span>

#### GStreamer

-   [http://www.gstreamer.net/](http://www.gstreamer.net/)

    是一个多媒体框架，允许通过在一个图形（管道）上汇编处理节点（元素）来创建多媒体应用，大量插件可用于轻松地创建播放应用、 录音机、 音频/视频编辑、 流媒体服务器、视讯会议系统。插件类型包括解码器、编码器、混音器、多路分配器、各种协议的网络资源、硬件加速功能 (解码、 显示、 捕获，...)、视频筛选器。底层的灵活性也带来了使用上的麻烦，但是在多种便利的插件（playbin, decodebin, camerabin）的帮助下，使得使用简单的使用案例很易用。它构建在 Glib/GObject 之上，因此很容易被移植到任意新平台上，得益于有很多可用的高质量并且支持多种格式的插件，不仅支持 lip-sync，支持网络流媒体，支持标准 Linux API 并且容易封装诸如 DSP 加速的编码器这样的硬件设备，所以，在嵌入式中，它可能会被广泛使用。

<span id="xine"></span>

#### Xine

-   [http://xinehq.de/](http://xinehq.de/) 是一个媒体播放引擎，能够为我们处理大部分的复杂问题。它基于多线程，所以时钟和同步被自动处理，需要注意的是，该库采用 GPL 许可，所以你的应用程序必须兼容 GPL 才能使用它。

<span id="mplayer"></span>

#### MPlayer

-   [http://mplayerhq.hu/](http://mplayerhq.hu/) - 它不是一个库而是一个应用程序，但是可以被其他应用程序控制并且在一些系统上当作媒体框架使用。同 Xine 一样，它采用 GPL 许可，但是因为可以从外部控制，所以我们的应用程序不采用 GPL 许可也可使用它。

<span id="documentation"></span>

#### 文档

-   [如何选择嵌入式图形库](http://tree.celinuxforum.org/CelfPubWiki/ELCEurope2008Presentations?action=AttachFile&do=get&target=choosing-embedded-graphical-libraries.pdf) - 由 Thomas Petazzoni 在 ELCE 2008 做的报告

<span id="video-in"></span>

### Video in

<span id="v4l-2"></span>

#### V4L[2]

-   [Documentation/video4linux](http://www.kernel.org/doc/Documentation/video4linux)
-   [http://www.linuxtv.org](http://www.linuxtv.org)
-   [http://www.linuxtv.org/downloads/video4linux/API/V4L2\_API/spec-single/v4l2.html](http://www.linuxtv.org/downloads/video4linux/API/V4L2_API/spec-single/v4l2.html)

<span id="openml"></span>

#### OpenML

-   [http://www.khronos.org/openml/](http://www.khronos.org/openml/)

<span id="linuxtv-dvb-api"></span>

#### LinuxTV (DVB API)

-   [http://www.linuxtv.org](http://www.linuxtv.org)

<span id="audio-in-out"></span>

### 音频输入/输出

<span id="oss"></span>

#### OSS

-   [Documentation/sound/oss](http://www.kernel.org/doc/Documentation/sound/oss)
-   [http://www.4front-tech.com/oss.html](http://www.4front-tech.com/oss.html)

<span id="alsa"></span>

#### ALSA

-   [Documentation/sound/alsa](http://www.kernel.org/doc/Documentation/sound/alsa)
-   [http://www.alsa-project.org](http://www.alsa-project.org)

<span id="openal"></span>

#### OpenAL

-   [http://www.openal.org/](http://www.openal.org/)

<span id="pulseaudio"></span>

#### PulseAudio

-   [http://pulseaudio.org](http://pulseaudio.org) PulseAudio 是一个跨平台的声音服务，为 Linux 声音子系统带来了很多很酷的特性。在嵌入式系统中使用它的理由描述在[这里](http://0pointer.de/blog/projects/pulse-glitch-free.html)。

<span id="users-of-avg"></span>

### AVG 标准的使用者

<span id="video-lan"></span>

#### Video Lan

-   [http://www.videolan.org](http://www.videolan.org)

<span id="freevo"></span>

#### Freevo

-   [http://freevo.sourceforge.net](http://freevo.sourceforge.net)

<span id="linuxtv"></span>

#### LinuxTV

-   [http://www.linuxtv.org/](http://www.linuxtv.org/)

<span id="mythtv"></span>

#### MythTV

-   [http://www.mythtv.org/](http://www.mythtv.org/)

<span id="dvr"></span>

#### DVR

-   [http://dvr.sourceforge.net/html/main.html](http://dvr.sourceforge.net/html/main.html)

<span id="openpvr"></span>

#### OpenPVR

-   [http://www.funktronics.ca/openpvr/](http://www.funktronics.ca/openpvr/)
-   [http://sourceforge.net/projects/openpvr/](http://sourceforge.net/projects/openpvr/)

<span id="morphine-tv"></span>

#### Morphine.TV

-   [http://wiki.morphine.tv](http://wiki.morphine.tv)
-   [http://sourceforge.net/projects/mms4l/](http://sourceforge.net/projects/mms4l/)

<span id="other"></span>

### 其他

<span id="arib-architecture"></span>

#### ARIB 架构（一个数字广播系统标准）

-   [http://www.arib.or.jp/english/html/overview/ov/std\_b24.html](http://www.arib.or.jp/english/html/overview/ov/std_b24.html)

<span id="boot-splash"></span>

#### 启动画面

-   [www.bootsplash.org](http://www.BootSplash.org/)

<span id="digital-home-working-group"></span>

#### 数字家庭工作组

-   [http://www.dhwg.org/](http://www.dhwg.org/)

<span id="disko-framework"></span>

#### Disko 框架

-   [http://www.diskohq.org](http://www.diskohq.org)
-   [http://www.directfb.org](http://www.directfb.org)

<span id="free-type"></span>

#### Free Type（软件字体引擎）

-   [http://freetype.sourceforge.net/freetype2/](http://freetype.sourceforge.net/freetype2/)

<span id="upnp"></span>

#### UPnP

-   [UPnP](../.././dev_portals/Multimedia/UPnP/UPnP.md "UPnP")

<span id="tv-anytime"></span>

#### TV Anytime 论坛

-   [http://www.tv-anytime.org/](http://www.tv-anytime.org/)

<span id="tv-linux-alliance"></span>

#### TV Linux 联盟

-   [http://www.tvlinuxalliance.com/](http://www.tvlinuxalliance.com/)

[分类](http://eLinux.org/Special:Categories "Special:Categories"):

-   [多媒体](http://eLinux.org/Category:Multimedia "Category:Multimedia")
-   [CE Linux 工作组](http://eLinux.org/Category:CE_Linux_Working_Groups "Category:CE Linux Working Groups")
