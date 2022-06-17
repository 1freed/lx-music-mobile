<p align="center"><a href="https://github.com/lyswhut/lx-music-mobile"><img width="200" src="https://github.com/lyswhut/lx-music-mobile/blob/master/doc/images/icon.png" alt="lx-music logo"></a></p>

<p align="center">
  <a href="https://github.com/lyswhut/lx-music-mobile/releases"><img src="https://img.shields.io/github/release/lyswhut/lx-music-mobile" alt="Release version"></a>
  <a href="https://github.com/lyswhut/lx-music-mobile/actions/workflows/release.yml"><img src="https://github.com/lyswhut/lx-music-mobile/workflows/Build/badge.svg" alt="Build status"></a>
  <a href="https://github.com/lyswhut/lx-music-mobile/actions/workflows/beta-pack.yml"><img src="https://github.com/lyswhut/lx-music-mobile/workflows/Build%20Beta/badge.svg" alt="Build status"></a>
  <a href="https://github.com/facebook/react-native"><img src="https://img.shields.io/github/package-json/dependency-version/lyswhut/lx-music-mobile/react-native/master" alt="React native version"></a>
  <!-- <a href="https://github.com/lyswhut/lx-music-mobile/releases"><img src="https://img.shields.io/github/downloads/lyswhut/lx-music-mobile/latest/total" alt="Downloads"></a> -->
  <a href="https://github.com/lyswhut/lx-music-mobile/tree/dev"><img src="https://img.shields.io/github/package-json/v/lyswhut/lx-music-mobile/dev" alt="Dev branch version"></a>
  <!-- <a href="https://github.com/lyswhut/lx-music-mobile/blob/master/LICENSE"><img src="https://img.shields.io/github/license/lyswhut/lx-music-mobile" alt="License"></a> -->
</p>


<h2 align="center">洛雪音乐助手移动版</h2>

### 说明

一个基于 React native 开发的音乐软件。

所用技术栈：

- React native
- Redux

支持的平台：

- Android

注：不计划支持IOS

软件变化请查看：[更新日志](https://github.com/lyswhut/lx-music-mobile/blob/master/CHANGELOG.md)<br>
软件下载请转到：[发布页面](https://github.com/lyswhut/lx-music-mobile/releases)<br>
或者到网盘下载（网盘内有MAC、windows版）：`https://www.lanzoui.com/b0bf2cfa/` 密码：`glqw`（若链接无法打开请百度：蓝奏云链接打不开）<br>
使用常见问题请转至：[常见问题](https://lyswhut.github.io/lx-music-doc/mobile/faq)<br>
桌面版项目地址：<https://github.com/lyswhut/lx-music-desktop>

### 源代码使用方式

#### 项目环境准备

1. **安装Node.js环境（如已安装请跳过）:** 下载[Node.js](https://nodejs.org/en/)安装结束后，打开命令行输入`node -v`将会输出Node.js的版本号即表示已安装完成
2. **拉取代码:** 克隆本仓库代码
3. **安装依赖:** 在项目根目录打开命令行，执行命令：`npm install`，若此命令执行的过程中报错可以尝试百度报错内容找解决方法，或在此处贴出报错日志一起讨论解决
4. 使用Android Studio打开项目根目录下的`android`文件夹，加载一遍`gradle`

#### 项目启动步骤

1. 启动模拟器或连接真实设备
2. **启动开发服务器:** 在项目根目录打开命令行，执行命令：`npm run ar`，若开发服务器意外停止了，可以执行`npm start`重新启动
3. **开发:** 修改项目下的JS即可实时看到修改后的效果

#### Native开发

使用Android Studio打开项目根目录下的`android`文件夹，即可在Android Studio内进行安卓代码的开发与调试

#### 构建安装包

首先生成安卓签名文件，然后将你的签名文件放在`android/app/`，然后在`android/`新建`keystore.properties`文件，填入你的签名信息：

```properties
storeFile=
storePassword=
keyAlias=
keyPassword=
```

最后在`android/`执行命令`./gradlew assembleRelease`，构建的安装包在`android/app/build/outputs/apk/release/`

<!--
### UI界面

<p><a href="https://github.com/lyswhut/lx-music-mobile"><img width="100%" src="https://github.com/lyswhut/lx-music-mobile/blob/master/doc/images/app.png" alt="lx-music UI"></a></p> -->

### 项目协议

本项目基于 [Apache License 2.0](https://github.com/lyswhut/lx-music-mobile/blob/master/LICENSE) 许可证发行，以下协议是对于 Apache License 2.0 的补充，如有冲突，以以下协议为准。

词语约定：本协议中的“本项目”指洛雪音乐移动版项目；“使用者”指签署本协议的使用者；“官方音乐平台”指对本项目内置的包括酷我、酷狗、咪咕等音乐源的官方平台统称；“版权数据”指包括但不限于图像、音频、名字等在内的他人拥有所属版权的数据。

1. 本项目的数据来源原理是从各官方音乐平台的公开服务器中拉取数据，经过对数据简单地筛选与合并后进行展示，因此本项目不对数据的准确性负责。
2. 使用本项目的过程中可能会产生版权数据，对于这些版权数据，本项目不拥有它们的所有权，为了避免造成侵权，使用者务必在**24小时**内清除使用本项目的过程中所产生的版权数据。
3. 本项目内的官方音乐平台别名为本项目内对官方音乐平台的一个称呼，不包含恶意，如果官方音乐平台觉得不妥，可联系本项目更改或移除。
4. 本项目内使用的部分包括但不限于字体、图片等资源来源于互联网，如果出现侵权可联系本项目移除。
5. 由于使用本项目产生的包括由于本协议或由于使用或无法使用本项目而引起的任何性质的任何直接、间接、特殊、偶然或结果性损害（包括但不限于因商誉损失、停工、计算机故障或故障引起的损害赔偿，或任何及所有其他商业损害或损失）由使用者负责。
6. 本项目完全免费，且开源发布于 GitHub 面向全世界人用作对技术的学习交流，本项目不对项目内的技术可能存在违反当地法律法规的行为作保证，**禁止在违反当地法律法规的情况下使用本项目**，对于使用者在明知或不知当地法律法规不允许的情况下使用本项目所造成的任何违法违规行为由使用者承担，本项目不承担由此造成的任何直接、间接、特殊、偶然或结果性责任。

若你使用了本项目，将代表你接受以上协议。

音乐平台不易，请尊重版权，支持正版。<br>
若对此有疑问请 mail to: lyswhut+qq.com (请将`+`替换成`@`)
