### 项目结构
```
|-- Vue
    |-- babel.config.js
    |-- ca.crt            # ca证书信息
    |-- ca.key            # ca证书信息
    |-- LICENSE
    |-- package-lock.json # 配置信息
    |-- package.json      # 配置信息 
    |-- vue.config.js     # Vue配置文件
    |-- yarn.lock         # 配置文件
    |-- coverage          # 前端配置信息
    |   |-- clover.xml
    |   |-- coverage-final.json
    |   |-- lcov.info
    |   |-- lcov-report
    |       |-- base.css
    |       |-- block-navigation.js
    |       |-- favicon.png
    |       |-- index.html
    |       |-- prettify.css
    |       |-- prettify.js
    |       |-- sort-arrow-sprite.png
    |       |-- sorter.js
    |-- public
    |   |-- index.html
    |-- src             # 主要源代码
    |   |-- App.vue     # 主组件
    |   |-- element.js  # 导入的element-ui
    |   |-- main.js     # 入口文件
    |   |-- assets      # 静态资源
    |   |   |-- images
    |   |   |   |-- common
    |   |   |   |   |-- logo.png
    |   |   |   |-- error
    |   |   |   |   |-- 401.png
    |   |   |   |   |-- 404.png
    |   |   |   |   |-- 500.png
    |   |   |   |-- file
    |   |   |   |   |-- dir.png
    |   |   |   |   |-- file_avi.png
    |   |   |   |   |-- file_chm.png
    |   |   |   |   |-- file_code.png
    |   |   |   |   |-- file_css.png
    |   |   |   |   |-- ……
    |   |   |   |-- footer
    |   |   |   |   |-- wechatImg.png
    |   |   |   |-- login
    |   |   |   |   |-- qqIcon.png
    |   |   |   |-- settings
    |   |   |       |-- use.jpg
    |   |   |       |-- userImg.png
    |   |   |-- styles
    |   |       |-- mixins.styl
    |   |       |-- varibles.styl
    |   |       |-- css
    |   |           |-- base.css
    |   |           |-- border.css
    |   |           |-- element-cover.css
    |   |           |-- mediaScreen.styl
    |   |-- components     # 组件
    |   |   |-- DragVerify.vue
    |   |   |-- Header.vue
    |   |-- global         # 全局常量声明
    |   |   |-- globalConst.js
    |   |-- pb_gen         # 与服务器通讯的接口文件
    |   |   |-- change_password_pb.js
    |   |   |-- common_pb.js
    |   |   |-- create_dir_pb.js
    |   |   |-- delete_file_pb.js
    |   |   |-- delete_share_token_pb.js
    |   |   |-- get_dir_pb.js
    |   |   |-- get_node_id_pb.js
    |   |   |-- get_node_pb.js
    |   |   |-- ……
    |   |-- request        # 封装通讯函数
    |   |   |-- file.js
    |   |   |-- http.js
    |   |   |-- user.js
    |   |-- router         # Vue-router的配置文件
    |   |   |-- before.js  # 拦截器配置
    |   |   |-- router.js  # 路由配置
    |   |-- ssl            # cert证书
    |   |   |-- cert.crt   
    |   |   |-- cert.key
    |   |-- store          # Vuex
    |   |   |-- index.js   # Vuex的配置文件
    |   |   |-- module     # Vuex的子模块
    |   |       |-- user.js
    |   |-- utils          # 工具函数封装
    |   |   |-- ByteUtils.js     # 字节数组处理函数
    |   |   |-- EncryptUtils.js  # 加密函数
    |   |   |-- FileUtils.js     # 文件处理函数
    |   |   |-- JSON.js          # JSON处理函数
    |   |   |-- StringUtils.js   # 字符串处理函数
    |   |-- views                # 视图组件
    |       |-- file
    |       |   |-- File.vue     # 文件组件
    |       |-- user             
    |           |-- Login.vue    # 登录页面组件
    |           |-- Register.vue # 注册逐渐组件
    |-- tests
        |-- test.js
```