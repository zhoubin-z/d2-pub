---
pageClass: page--custom-pre
---

# D2Admin

[D2Admin](https://github.com/d2-projects/d2-admin) 是一个完全 **开源免费** 的企业中后台产品前端集成方案，使用最新的前端技术栈，小于 60kb 的本地首屏 js 加载，已经做好大部分项目前期准备工作，并且带有大量示例代码，助力管理系统快速开发。

### 完整版

* 仓库：
[Github](https://github.com/d2-projects/d2-admin) / 
[码云](https://gitee.com/fairyever/d2-admin) / 
[coding](https://d2-projects.coding.net/p/d2-projects/d/d2-admin/git)
* 预览：
[https://d2.pub/d2-admin/preview](https://d2.pub/d2-admin/preview)

### 简化版

* 仓库：
[Github](https://github.com/d2-projects/d2-admin-start-kit) / 
[码云](https://gitee.com/fairyever/d2-admin-start-kit) / 
[coding](https://d2-projects.coding.net/p/d2-projects/d/d2-admin-start-kit/git)
* 预览：
[https://d2.pub/d2-admin-start-kit/preview](https://d2.pub/d2-admin-start-kit/preview)

## 功能

* 使用 vue-cli3 构建
* 首屏加载等待动画
* 五款主题
* 内置 UEditor 富文本编辑器
* 详细的文档
* 登录和注销
* 分离的路由和菜单设置
* 可折叠侧边栏
* 多国语
* 富文本编辑器
* Markdown 编辑器
* 全屏
* Fontawesome 图标库
* 图标选择器
* 自动注册 SVG 图标
* 模拟数据
* 剪贴板封装
* 图表库
* 时间日期计算工具
* 导入 Excel （ xlsx + csv ）
* 数据导出 Excel （ xlsx + csv ）
* 数据导出文本
* 数字动画
* 可拖拽调整大小的区块布局
* 可拖拽调整大小和位置的网格布局
* 开箱即用的页面布局组件
* 加载并解析 markdown 文件
* GitHub 样式的 markdown 显示组件
* markdown 内代码高亮
* 为 markdown 扩展了百度云链接解析和优化显示
* 右键菜单组件
* 自定义滚动条和滚动控制
* 公用样式抽离，方便的主题定制
* 支持临时菜单配置
* 系统功能展示模块 `1.1.4 +`
* 多标签页模式 `1.1.4 +`
* 美化滚动条 `1.1.4 +`
* json view `1.1.4 +`
* cookie 封装 `1.1.5 +`
* 多标签页全局控制 API `1.1.5 +`
* 菜单全局控制 API `1.1.5 +`
* 多标签页关闭控制支持右键菜单 `1.1.10 +`
* 模块化全局状态管理 `1.2.0 +`
* 多种数据持久化方式：区分用户，区分路由，页面数据快照功能 `1.2.0 +`
* 支持跳出外部链接的菜单系统 `1.2.0 +`
* 支持菜单 svg 图标 `1.3.0 +`
* 日志记录和错误捕捉 `1.3.0 +`
* 全局菜单搜索 `1.3.0 +`
* 自定义登录重定向 `1.3.0 +`
* 切换全局基础组件尺寸 `1.4.0 +`
* 页面载入进度条 `1.4.1 +`
* 自适应的顶部菜单栏 `1.4.7 +`
* 数据导出 xslx 时支持合并单元格 `1.5.4 +`
* 多标签页支持拖拽排序 `1.8.0 +`
* 优化生产环境构建，首页只加载小于 60kb 的本地 js 代码 `1.8.0 +`
* 内置了构建文件体积检查工具 `1.8.0 +`

## 项目结构

::: tip 树形图生成工具
[Folder Explorer](https://github.com/d2-projects/folder-explorer)
:::

```
├─.DS_Store 
├─.browserslistrc ------------------- // 目标浏览器配置
├─.env ------------------------------ // 基础环境变量配置
├─.env.development ------------------ // 开发模式下的环境变量配置
├─.env.netlify ---------------------- // Netlify 构建时的环境变量
├─.env.nomock ----------------------- // 无 mock 数据构建模式下的环境变量
├─.env.travis ----------------------- // Travis 构建时的环境变量
├─.eslintignore --------------------- // ESLint 的忽略目录配置
├─.eslintrc.js ---------------------- // ESLint 的配置文件
├─.github --------------------------- // Github 配置
│ └─ISSUE_TEMPLATE ------------------ // GitHub issue 模板
├─.gitignore ------------------------ // git 的忽略配置
├─.postcssrc.js --------------------- // postcss 插件设置
├─.travis.yml ----------------------- // Travis 配置文件
├─LICENSE --------------------------- // 开源协议
├─README.md ------------------------- // 介绍
├─README.zh.md ---------------------- // 中文介绍 在码云仓库下自动加载这个文件
├─babel.config.js ------------------- // babel 设置
├─cdnrefresh-dirs.txt --------------- // 自动构建后在七牛 CDN 上刷新的目录
├─d2-admin.babel -------------------- // 多国语设置软件 BabelEdit 的项目文件
├─doc ------------------------------- // 文档素材
│ └─image 
├─jest.config.js -------------------- // 单元测试配置
├─jsconfig.json --------------------- // 指定根文件和 JavaScript 语言服务提供的功能选项
├─package-lock.json ----------------- // 锁定依赖版本
├─package.json ---------------------- // 项目信息和依赖
├─public ---------------------------- // 静态资源文件夹，不经过 webpack 处理
│ ├─html ---------------------------- // 用于演示加载静态页面的资源
│ ├─icon.ico ------------------------ // 网站图标
│ ├─image 
│ │ ├─baidu-pan-logo.png 
│ │ ├─loading ----------------------- // index.html 使用的加载图标
│ │ └─theme ------------------------- // 主题图片资源
│ │   ├─d2 
│ │   ├─line 
│ │   ├─star 
│ │   ├─tomorrow-night-blue 
│ │   └─violet 
│ ├─index.html ---------------------- // 网站的基础页面模板
│ ├─lib ----------------------------- // 静态依赖
│ │ └─UEditor ----------------------- // 编辑器
│ └─markdown ------------------------ // 用于展示 Markdown 远程加载资源的文件
├─qiniu-config ---------------------- // 用于构建展示网站的七牛设置
├─qshell ---------------------------- // 七牛 SDK
├─src ------------------------------- // 主要的代码目录
│ ├─App.vue ------------------------- // 项目根组件
│ ├─api ----------------------------- // 请求接口
│ ├─assets -------------------------- // 资源文件夹
│ │ ├─style ------------------------- // 样式资源
│ │ │ ├─animate --------------------- // 页面过渡动画
│ │ │ ├─fixed ----------------------- // 覆盖一些组件库的默认样式
│ │ │ ├─public-class.scss ----------- // 导出可以直接使用的 class
│ │ │ ├─public.scss ----------------- // 导出所有公用的 scss 资源
│ │ │ ├─theme ----------------------- // 主题样式相关
│ │ │ │ ├─d2 
│ │ │ │ ├─line 
│ │ │ │ ├─register.scss ------------- // 注册所有主题样式
│ │ │ │ ├─star 
│ │ │ │ ├─theme-base.scss ----------- // 每个主题共用的样式
│ │ │ │ ├─theme.scss ---------------- // 每个主题特有的设置
│ │ │ │ ├─tomorrow-night-blue 
│ │ │ │ └─violet 
│ │ │ └─unit ------------------------ // scss 的基础变量
│ │ └─svg-icons --------------------- // svg 图标
│ │   ├─icons ----------------------- // 用来存放图标的文件夹
│ │   └─index.js -------------------- // 自动导入所有符合条件的图标
│ ├─components ---------------------- // 组件
│ │ ├─d2-container 
│ │ ├─d2-container-frame 
│ │ ├─d2-count-up 
│ │ ├─d2-highlight 
│ │ ├─d2-icon 
│ │ ├─d2-icon-select 
│ │ ├─d2-icon-svg 
│ │ ├─d2-icon-svg-select 
│ │ ├─d2-link-btn 
│ │ ├─d2-markdown 
│ │ ├─d2-mde 
│ │ ├─d2-module-index-banner 
│ │ ├─d2-module-index-menu 
│ │ ├─d2-quill 
│ │ ├─d2-ueditor 
│ │ ├─highlight-styles -------------- // 代码高亮样式
│ │ └─index.js ---------------------- // 组件注册
│ ├─i18n.js ------------------------- // 国际化配置
│ ├─layout -------------------------- // 布局
│ │ └─header-aside ------------------ // 具有顶栏加侧边栏的布局
│ ├─libs ---------------------------- // 一些通用的方法
│ │ ├─util.cookies.js 
│ │ ├─util.db.js 
│ │ ├─util.import.development.js ---- // 开发环境下使用的页面导入方法
│ │ ├─util.import.production.js ----- // 开发环境下使用的页面导入方法
│ │ ├─util.js 
│ │ └─util.log.js 
│ ├─locales ------------------------- // 国际化语言配置
│ │ ├─en.json 
│ │ ├─ja.json 
│ │ ├─zh-chs.json 
│ │ └─zh-cht.json 
│ ├─main.js ------------------------- // 程序主入口
│ ├─menu ---------------------------- // 静态的菜单数据
│ │ ├─index.js 
│ │ └─modules 
│ │   ├─demo-business.js 
│ │   ├─demo-charts.js 
│ │   ├─demo-components.js 
│ │   ├─demo-d2-crud.js 
│ │   ├─demo-element.js 
│ │   ├─demo-frame.js 
│ │   ├─demo-playground.js 
│ │   └─demo-plugins.js 
│ ├─mock 
│ │ ├─api --------------------------- // 需要注册的接口
│ │ ├─d2-mock ----------------------- // 简化接口注册的工具
│ │ └─index.js ---------------------- // mock 数据自动注册
│ ├─plugin -------------------------- // 插件
│ │ ├─axios ------------------------- // 网络请求
│ │ ├─d2admin ----------------------- // 统一注册系统必须的资源
│ │ ├─error ------------------------- // 错误拦截
│ │ ├─log --------------------------- // 日志
│ │ └─open -------------------------- // 新窗口打开
│ ├─router -------------------------- // 路由
│ │ ├─index.js ---------------------- // 注册路由以及设置拦截规则
│ │ ├─modules ----------------------- // 预先设置好的静态路由
│ │ │ ├─business.js 
│ │ │ ├─charts.js 
│ │ │ ├─components.js 
│ │ │ ├─d2-crud.js 
│ │ │ ├─element.js 
│ │ │ ├─frame.js 
│ │ │ ├─playground.js 
│ │ │ └─plugins.js 
│ │ └─routes.js --------------------- // 导入所有路由
│ ├─setting.js ---------------------- // 全局设置
│ ├─store --------------------------- // vuex
│ │ ├─index.js ---------------------- // vuex 注册主入口
│ │ └─modules ----------------------- // 模块目录
│ │   └─d2admin --------------------- // 系统自带模块，业务模块建议在同级新建
│ │     ├─index.js ------------------ // 模块主入口
│ │     └─modules ------------------- // 子模块
│ │       ├─account.js -------------- // 用户身份
│ │       ├─color.js ---------------- // 主题颜色
│ │       ├─db.js ------------------- // 本地数据库
│ │       ├─fullscreen.js ----------- // 全屏
│ │       ├─gray.js ----------------- // 灰度模式
│ │       ├─log.js ------------------ // 日志
│ │       ├─menu.js ----------------- // 菜单
│ │       ├─page.js ----------------- // 多页面控制
│ │       ├─releases.js ------------- // 版本
│ │       ├─search.js --------------- // 全局搜索
│ │       ├─size.js ----------------- // 全局尺寸
│ │       ├─theme.js ---------------- // 主题
│ │       ├─transition.js ----------- // 过渡效果
│ │       ├─ua.js ------------------- // 浏览器信息
│ │       └─user.js ----------------- // 用户信息
│ └─views --------------------------- // 页面视图
│   ├─demo -------------------------- // 演示页面
│   │ ├─business -------------------- // 业务页面演示
│   │ │ ├─index 
│   │ │ ├─issues 
│   │ │ └─table 
│   │ ├─charts ---------------------- // 图表
│   │ │ ├─index 
│   │ │ └─list 
│   │ │   ├─_data 
│   │ │   ├─_mixin 
│   │ │   ├─bar 
│   │ │   ├─candle 
│   │ │   ├─funnel 
│   │ │   ├─gauge 
│   │ │   ├─heatmap 
│   │ │   ├─histogram 
│   │ │   ├─line 
│   │ │   ├─map 
│   │ │   ├─pie 
│   │ │   ├─radar 
│   │ │   ├─ring 
│   │ │   ├─sankey 
│   │ │   ├─scatter 
│   │ │   ├─tree 
│   │ │   └─waterfall 
│   │ ├─components ------------------ // 内置组件演示
│   │ │ ├─container 
│   │ │ ├─contextmenu 
│   │ │ ├─countup 
│   │ │ ├─editor-quill 
│   │ │ ├─editor-simpleMDE 
│   │ │ ├─editor-ueditor 
│   │ │ ├─highlight 
│   │ │ ├─icon 
│   │ │ ├─index 
│   │ │ ├─json-tree 
│   │ │ ├─layout 
│   │ │ └─markdown 
│   │ ├─d2-crud --------------------- // D2CRUD 表格封装演示
│   │ ├─element --------------------- // Element UI 组件
│   │ ├─frame ----------------------- // 嵌套第三方页面演示
│   │ ├─playground ------------------ // 试验台
│   │ │ ├─add-routes ---------------- // 动态添加路由
│   │ │ ├─db ------------------------ // 数据持久化
│   │ │ ├─env ----------------------- // 环境变量
│   │ │ ├─index 
│   │ │ ├─locales ------------------- // 多国语
│   │ │ ├─log ----------------------- // 日志
│   │ │ ├─page-argu ----------------- // 页面参数
│   │ │ ├─page-cache ---------------- // 页面缓存
│   │ │ └─store --------------------- // 全局状态控制
│   │ │   ├─fullscreen 
│   │ │   ├─gray 
│   │ │   ├─menu 
│   │ │   ├─page 
│   │ │   ├─size 
│   │ │   ├─theme 
│   │ │   ├─transition 
│   │ │   └─ua 
│   │ └─plugins --------------------- // 插件演示
│   │   ├─better-scroll 
│   │   ├─clipboard-polyfill 
│   │   ├─day 
│   │   ├─export 
│   │   ├─import 
│   │   ├─index 
│   │   ├─js-cookie 
│   │   └─mock 
│   └─system ------------------------ // 系统页面
│     ├─error 
│     ├─function 
│     │ ├─redirect ------------------ // 重定向
│     │ └─refresh ------------------- // 刷新
│     ├─index 
│     ├─log 
│     └─login 
├─tests ----------------------------- // 单元测试
├─tools 
│ └─vue-filename-injector ----------- // 用于对每个组件注入源代码位置的插件
└─vue.config.js --------------------- // vue-cli3 的项目配置文件
```