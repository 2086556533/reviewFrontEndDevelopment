# 笔记
## 脚手架文件结构
    |-- .gitignore:git版本管制忽略的配置
    |-- babel.config.js：babel的配置文件
    |-- package-lock.json：包版本控制文件
    |-- package.json：应用包配置文件
    |-- README.md：应用描述文件
    |-- node_modules
    |-- public
    |   |-- favicon.ico：页签图标
    |   |-- index.html：主页面
    |-- src
        |-- App.vue：汇总所有组件
        |-- main.js：入口文件
        |-- assets：存放静态资源
        |   |-- logo.png
        |-- components：存放组件
            |-- Boss.vue
            |-- Bro.vue
            |-- HelloWorld.vue
## 关于不同版本的Vue：
- vue.js与vue.runtime.xxx.js的区别
    1. vue.js是完整版的Vue，包含：核心功能 + 模板解析器
    2. vue.runtime.xxx.js是运行版的Vue，只包含核心功能
- 因为vue.runtime.xxx.js没有模板解析器，所以不能使用template配置项，需要使用render函数接收到的createElement函数去制定具体内容
## vue.config.js配置文件
> 使用vue inspect > output.js 可以查看到vue脚手架的默认配置
> 使用vue.config.js可以对脚手架进行个性化定制，详情见：https://cli.vuejs.org/zh