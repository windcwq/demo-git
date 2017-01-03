### 目录结构

    / 根目录
    |__ build 编译工具以及webpack配置文件
    |   |__ config webpack配置
    |   |__ public 实例静态文件
    |   |__ router 实例的路由
    |   |__ views 实例的模板
    |   |__ app.js 实例入口
    |__ dist 发行目录
    |__ src 开发目录
    |   |__ app 应用私有目录
    |   |__ components 组件目录
    |   |__ img 公用图片
    |   |__ lib 基础库等
    |   |__ styles 公用样式
    |   |__ main.js UI入口
    |__ package.json 依赖管理
    
### 环境依赖

    - node 6以上版本

###　运行方式

###### 安装

    npm i //或 yarn

    //安装失败时、导致运行失败时尝试：
    npm cache clean //或 yarn cache clean
    npm config set registry http://registry.npm.taobao.org  //或 yarn config set registry https://registry.npm.taobao.org 

###### 开发

    npm run dev

###### 打包

    npm run build

### css命名规范

    - .l- js UI 样式前缀
    注意：只要是以.l-开头的，命名都是直接在UI里面定义，如果要增删改请修改js

    - .ui- 组件类前缀

### js规范

    - 组件components目录下，每个组件都必须有独立的index.js，方便独立打包。

    - 开发组件有需要可继承基础类，方便管理公用dom，如果弹窗、控制z-index等。 