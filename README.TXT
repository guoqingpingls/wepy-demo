
01. cd project-name
02. npm i
03. wepy build --watch
项目目录
    |—— dist                //微信开发者指定的目录（该目录由wepy的build指令自动编译生成）
    |—— node_modules        //依赖包
    |—— src                 // 代码编写的目录
    |   |—— components      // 组件目录
    |   |   |__
    |   |—— mixins          // 工具函数
    |   |—— pages           // 页面目录
    |   |   |—— inex.wpy    // index页面（经build后，会在dist目录下的pages目录生成index.js, index.json, index.wxml,index.wxss文件）
    |   |   |__ other.wpy   // other页面（经build后，会在dist目录下的pages目录生成other.js、other.json、other.wxml和other.wxss文件）
    |   |—— store
    |   |   |—— action
    |   |   |—— reducer
    |   |   |—— types
    |   |   |__ index.js
    |   |__app.wpy          // 小程序配置项（全局数据、样式、声明钩子等；经build后，会在dist目录下生成app.js、app.json和app.wxss文件）
    |__ package.json        // 项目的package配置