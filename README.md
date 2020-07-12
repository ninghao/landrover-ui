# Land Rover 页面实战

这是宁皓网在[页面设计实战课程](https://ninghao.net/package/website)里做的一个项目，课程的目的是熟悉网页设计，项目里用了一些社区提供的资源，比如 Semantic UI 样式框架，Material Design 小图标，Slick Carousel 幻灯片 ... 项目主要的样式是我们自己一步一步写好的，写样式的时候用了 Sass ，这个实战课程里包含了大量的页面设计技巧，完整的展示了页面设计流程。

之前的开发流程比较复杂，很多同学反应配置开发环境的时候出了很多问题。我们重新修改了开发流程，让整个项目只有一个依赖（Sass），极大简化了开发流程，大家可以专注于页面设计本身。

**演示地址**：[_https://demo.ninghao.net/landrover-ui_](https://demo.ninghao.net/landrover-ui)
**课程地址**：_https://ninghao.net/package/website_

## 准备工具

推荐使用 VSCode 代码编辑器，给编辑器安装一个 [Live Serve 插件](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)。另外我们还会用到命令行工具，macOS 用户可以使用系统自带的终端，Windows 用户可以额外下载安装一个[完整版的 Cmder](https://ninghao.net/video/8068)。

## 准备项目

**1：进入到想要保存项目的地方**

```
cd ~/desktop
```

**2：把项目克隆到本地**

```
git clone https://github.com/ninghao/landrover-ui
```

**3：进入到项目所在目录**

```
cd landrover-ui
```

**4：用编辑器打开项目目录**

你可以使用自己的编辑器打开刚刚克隆到本地的这个项目，观察一下项目里的东西。

```
├── README.md
├── assets
│   ├── enquire.js
│   ├── jquery
│   ├── material-design-icons
│   ├── semantic
│   └── slick-carousel
├── images
│   ├── ...-304360_1600x900.jpg
│   ├── ...
├── index.html
├── product.html
├── scripts
│   └── main.js
└── styles
    ├── main.css
    ├── main.scss
```

- **assets**：社区提供的资源，比如 Semantic UI，Slick Carousel 等等
- **images**：项目需要的一些图像资源
- **index.html**：项目的首页
- **product.html**：项目的产品页面
- **scripts**：自定义脚本
- **styles**：自定义样式，包含 .scss 文件与编译好的 .css 文件

## 预览项目

你可以直接在文件系统双击打开项目里的 index.html 或者 product.html 这两个网页文件，系统默认会用浏览器打开网页文件。或者你可以使用给 VSCode 编辑器安装的 Live Server 插件打开这两个页面，方法是在编辑器里打开网页文件，然后打开编辑器的命令面板，搜索 Open with live server，执行一下这个命令，会创建一个服务器，然后自动在浏览器上打开网页文件。

## 开发项目

课程里有几节会介绍准备开发流程，你可以跳过这些视频，因为我们在这里准备了一个简化的开发流程。另外在课程里我们会安装一些 Package，这些你都不需要额外安装了，因为我已经把所有你需要的东西都准备好了，放在了 assets 这个目录下面了，你可以直接引用这个项目里的东西，就不需要再额外安装它们了。

**1：安装依赖**

项目只有一个依赖就是 Sass，因为我们写样式的时候用到了 Sass / Scss 这种格式，所以需要把它们编译成普通的 CSS，这就需要安装一个 Sass 工具。在项目所在目录的下面，执行下面这个命令安装项目依赖的 Sass：

```
npm install
```

**2：监视 .scss**

在项目的 styles 目录的下面会有一些 .scss 格式的文件，你可以修改这些文件，然后再把它们编译成 .css 文件。执行下面这个命令会监视项目里的这些 .scss 文件的变化，然后自动编译它们：

```
npm run watch:scss
```

**3：实时预览**

如果你使用的是 VSCode 编辑器，并且给编辑器安装了 Live Server 插件，你可以打开项目里的一个网页文件，然后打开编辑器的命令面板，搜索并执行 Open with live server 命令，这样会创建一个 Web 服务器，然后自动打开网页。这样每次项目里的文件有变化的时候，浏览器会自动刷新。

## 从头开始

准备开始学习之前，你可能希望准备一个空白的项目，然后跟着视频一步一步操作。你可以基于 _starting-point_ 这个分支创建一个本地的开发分支，然后跟着课程视频一步一步练习。

**1：创建本地开发分支**

```
git checkout -b develop remotes/origin/starting-point
```

**2：安装依赖**

```
npm install
```

**3：监视 .scss**

```
npm run watch:scss
```
