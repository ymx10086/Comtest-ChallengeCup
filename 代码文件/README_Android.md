

# Android工程结构

```bash
app
├── build								# 编译生成的文件目录
├── build.gradle						# 项目配置文件
└──	src									# 源代码目录
    ├── test 								# 测试代码目录
    ├── androidTest							# android功能测试代码目录
    └──	main								# 项目代码目录
        ├── AndroidManifest.xml					# 程序运行时的组件、权限配置 
        ├── assets
        │   └── domain.crt							# HTTPS证书
        ├── res	
        │   ├── drawable							# 图片资源目录
        │   ├── layout								# 布局文件目录
        │   ├── menu								# 菜单选项目录
        │   └── values								# 常量目录
        └── java
        	└── com.graduate.design
        		├── MainActivity.java					# 程序入口
        		├── activity							# 管理activity组件目录
        		├── fragment							# 管理fragment组件目录
        		├── adapter								# 管理列表项目录
                ├── entity								# 管理实体类目录
                │   ├── BiIndex.java						# 双向索引结构
                │   └── GotNodeList.java					# 保存已经请求过的文件列表
                ├── proto								# protobuf生成的接口类目录
                ├── sharetokenProtocol	
                │	└── ShareTokenGen.java					# 分享令牌生成类
                ├── utils								# 工具类
                ├── view								# 自定义UI标签
                │	├── ClearEditText.java					# 可以清空的输入框
                │	└── NestedListView.java					# 可以滑动的展示列表
                └── service
                	├── UserService.java					# 接口模块，负责调用服务器端接口完成用户请求
                	├── NetWorkService.java					# 网络模块，负责与服务器进行通信
                	├── EncryptionService.java				# 加密算法模块
               		└──	impl								# 对应实现类目录
```

# layout

```bash
layout
├── activity_main.xml					# 启动界面
├── activity_login.xml					# 登录界面
├── activity_register.xml				# 注册界面
├── activity_home.xml					# 主界面，包含底部导航栏
├── activity_bt_client.xml				# 蓝牙发起方界面
├── activity_bt_server.xml				# 蓝牙接收方界面
├── activity_share.xml					# 蓝牙传输界面
├── activity_receive.xml				# 蓝牙接收界面
├── fragment_disk.xml					# 文件界面
├── fragment_file_content.xml			# 文件内容界面
├── fragment_search.xml					# 文件搜索界面
├── fragment_mine.xml					# 用户界面
├── fragment_change_password.xml		# 修改密码界面
├── fragment_settings.xml				# 设置界面
├── fragment_about.xml					# 关于界面
├── dialog.xml							# 创建文件夹的弹框布局设计
├── item_file.xml						# 文件信息列表项布局设计
├── item_file_share.xml					# 分享文件列表项布局设计
└── item_device.xml						# 设备列表项布局设计
```

# activity

```bash
activity
├── LoginActivity.java 					# 登录组件，展示登录界面
├── RegisterActivity.java				# 注册组件，展示注册界面
├── HomeActivity.java					# 主界面组件，可以通过底部导航栏切换文件和用户界面
├── BtClientActivity.java 				# 蓝牙组件，连接发起方
├── BtServerActivity.java 				# 蓝牙组件，连接接收方
├── ShareActivity.java 					# 蓝牙组件，传输文件
└── ReceiveActivity.java 				# 蓝牙组件，接收文件
```

# fragment

```bash
fragment
├── DiskFragment.java 					# 展示文件界面
├── FileContentFragment.java 			# 展示文件内容界面
├── SearchFragment.java 				# 展示搜索界面
├── MineFragment.java 					# 展示用户界面
├── ChangePasswordFragment.java 		# 展示修改密码界面
├── SettingsFragment.java 				# 展示设置界面
└── AboutFragment.java  				# 展示产品信息界面
```

# adapter

```bash
adapter
├── DeviceItemAdapter.java				# 蓝牙连接发起方扫描到的设备列表
└── fileItem
    ├── BaseFileItemAdapter.java		# 是下面列表项的父类
    ├── GetNodeFileItemAdapter.java		# 文件界面或搜索界面获取到的文件信息列表
    ├── ShareFileItemAdapter.java		# 选择传输文件列表
    ├── ReceiveFileItemAdapter.java		# 接收文件列表
    └── ChooseDirFileItemAdapter.java	# 选择保存接收文件的位置列表
```

