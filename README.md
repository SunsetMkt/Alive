<div style="display: flex; width: 100%; gap: 16px;">
<img style="width: 156px; height: 156px; border-radius: 12px;" src="./public/app-icon.png" alt="App Icon"/></a>

<div align="center" style="height: 156px; display: flex; flex-direction: column; align-items: center;">

<i>Alive：支持 Live2d 和 MMD 模型的开源桌宠软件。</i>

<a href="https://github.com/TopSea/Alive/stargazers"><img src="https://img.shields.io/github/stars/TopSea/Alive" alt="Stars Badge"/></a>
<a href="https://github.com/TopSea/Alive/pulls"><img src="https://img.shields.io/github/issues-pr/TopSea/Alive" alt="Pull Requests Badge"/></a>
<a href="https://github.com/TopSea/Alive/issues"><img src="https://img.shields.io/github/issues/TopSea/Alive" alt="Issues Badge"/></a>
<a href="https://github.com/TopSea/Alive/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/TopSea/Alive?color=2b9348"></a>
<br>
<a href="https://github.com/TopSea/Alive/blob/master/LICENSE"><img src="https://img.shields.io/github/license/TopSea/Alive?color=2b9348" alt="License Badge"/></a>
<a href="https://github.com/TopSea/Alive/releases"><img src="https://img.shields.io/github/downloads/TopSea/Alive/total" alt="Download Badge"/></a>

</div>
</div>

## 开发进度
0.0.1-alpha 已发布！
beta 版还在全力开发中，预计可以在年前发布。   
关注我（[GoAHi](https://space.bilibili.com/307219768)），更快获得发布信息。

## 功能实现计划
### 已实现的功能
- [x] Live2d 和 MMD 模式切换
- [x] Live2d 和 MMD 模型的展示和交互操作
- [x] Live2d 和 MMD 更换展示的模型
- [x] 鼠标点击穿透
- [x] 保存窗口的位置和大小
- [x] 开机启动

### 0.0.1-beta 计划实现的功能
- [ ] 多语言切换
- [ ] 深色模式
- [ ] 自动下载更新

## 适配计划
Windows：Windows 11/10 。windows 10 之前的版本不会进行测试和适配，不保证能否运行。  
Linux：~~Ubuntu 最新发布版（22.04）。其他的 Linux 发行版没有适配打算，Ubuntu 22.04 之前的版本不会进行测试和适配，不保证能否运行。~~ 最近要准备面试找班上了，暂时先鸽了。  
MacOS：没有适配打算。我没有可用于开发和测试的 Mac 电脑，除非你送我一台。

## Build
如果你想自己 build 的话。  
必须条件：Rust 环境、Nodejs 和 yarn
```
git clone https://github.com/TopSea/Alive
cd Alive
yarn

yarn tauri dev
```
Linux 和 MacOS 可能还需要一些依赖，可参考：[Tauri 官方文档](https://tauri.app/zh-cn/v1/guides/getting-started/prerequisites)

## 主要依赖
Live2d：pixijs 和 pixi-live2d-display。   
MMD：babylonjs 和 babylon-mmd。

## 关于模型和动作
**MMD**：  
* 芙卡洛斯模型 ==> 作者：[给你柠檬椰果养乐多你会跟我玩吗](https://space.bilibili.com/32704665)，下载地址：[水神 芙卡洛斯](https://www.aplaybox.com/details/model/ZftsfJMVgQsx)
* 丘丘摇动作 ==> 作者：[Ponx_迫奈熏](https://space.bilibili.com/345268724)，下载地址：[胡桃待机动作-丘丘摇](https://www.aplaybox.com/details/motion/HDLRono2SdAG)   

**模型和动作文件不为本项目所有。本项目对模型和动作的使用已征得作者同意，如果你要将模型和动作用在他处请遵守作者的使用要求。**    
**关于 alive_mmd.json 的编写规范：[关于 .alive_mmd.json](./docs/alive_mmd.md) 。**

## 关于项目
一切的开始是因为碧蓝航线之前更新了一个拉菲的兔女郎服装（对兔女郎毫无抵抗力.jpg）。  

然后就搜怎么提取怎么展示。搜到了 PPet，但是用着不太符合我的想法而且 PPet 项目也好久没更新了。所以就打算自己改改来用，但是 electron 这个包死活下不下来，换镜像用代理都不行。淦！刚好当时学 Tauri 和 React 有一段时间了，干脆再造个轮子。  

最开始是用 Tauri 和 React 写的（[Live2d-Tauri](https://github.com/TopSea/Live2d-Tauri)），但是写的不是很好。就打算用 vue 再再造个轮子顺便也让我在原神中的老婆们能展示展示，所以 Alive 就诞生了。




[app-icon]: ./public/app-icon.png