macOS 提示“应用已损坏，无法打开”？
由于 macOS 的安全机制，非 App Store 下载的应用可能会触发此提示。您可以按照以下步骤快速修复：

命令行修复 (推荐): 打开终端，执行以下命令：
sudo xattr -rd com.apple.quarantine "/Applications/Antigravity Tools.app"
Homebrew 安装技巧: 如果您使用 brew 安装，可以添加 --no-quarantine 参数来规避此问题：
brew install --cask --no-quarantine antigravity-tools

基于Vue和Vue-router搭建的电影移动WebApp应用
======

简介:
----
- 项目使用`Vue.js`组件化开发完成；
- 使用`Vue-router`完成组件间路由跳转；
- 使用`Vue-resource`获取数据；
- 使用`sessionStorage`完成对首页和列表页面数据的存储，在不结束回话的前提下减少不必要的请求并提高访问速度；
- 使用`frozen UI`移动UI库中的小图标及完成项目整体样式；
- 使用`Jade`和`Sass`完成HTML和样式编写；
- 使用了`ES6`语法并通过`babel`完成编译；
- 使用`ESlint`对项目代码进行风格统一及校验；
- 使用`Webpack`完成模块打包加载，并通过`Webpack-dev-server`运行，支持代码`热替换`

效果展示
----
<a href="http://loogeek.github.io/MovieApp-Vue" target="\_blank">使用Chrome游览器开发者工具手机模式查看效果</a>

项目整体效果
-------
<div>
  <img src="https://raw.githubusercontent.com/Loogeek/Project_Imgs/master/MovieApp-Vue/1.png" width="240px"/>
  <img src="https://raw.githubusercontent.com/Loogeek/Project_Imgs/master/MovieApp-Vue/3.png" width="240px"/>
  <img src="https://raw.githubusercontent.com/Loogeek/Project_Imgs/master/MovieApp-Vue/4.png" width="240px"/>
</div>
<div>
  <img src="https://raw.githubusercontent.com/Loogeek/Project_Imgs/master/MovieApp-Vue/5.png" width="240px"/>
  <img src="https://raw.githubusercontent.com/Loogeek/Project_Imgs/master/MovieApp-Vue/6.png" width="240px"/>
  <img src="https://raw.githubusercontent.com/Loogeek/Project_Imgs/master/MovieApp-Vue/2.png" width="240px"/>
</div>

运行
-------
npm install安装包后通过npm run dev命令启动服务器，`0.0.0.0:3000` 端口下查看项目，
若想改成其他启动端口可在package.json文件中修改scripts下的dev--host域名及--port端口

``` bash
npm install    
npm run dev   # run the counter example
```

后期完善
-------
完善代码功能
