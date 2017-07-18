# 需求概述

### 相关组件
------
* System （Default、Annotation）
* Startup（Load Config、Bind address）
* Config （Filter、init、web)
* Spring （Context、MVC）
* Netty  （HTTP、TCP）
* XTools （XML、JSON、YAML、Properties）

### System模块
------
+ 系统常量定义，相关注解，枚举，协议等lib使用所需的数据类型定义
+ 支持初始化系统Context，程序共享一份Context参数

### Startup模块
------
+ 程序启动加载配置
+ 初始化Spring上下文
+ 初始化MVC上下文
+ 绑定发布的地址和端口
+ 启动服务监听

### Config模块
------
+ 支持的配置文件类型：ymal，json，xml，properties
+ 提供多种配置文件加载方式：String，File，Stream
+ ConfigFactory 统一对外提供Value获取接口（K,V）
+ 提供配置文件修改接口：修改值或替换全部，并重新加载
+ 支持任意自定义配置，可方便用户进行扩展
+ 配置加载时，需要对配置项进行校验：必选配置，可选配置

### Spring模块
------
+ 支持Spring集成平台
+ 支持自定义MVC
+ 支持配置指定相关文件或参数
+ 支持应用级过滤器
+ 支持参数类型和值智能注入

### Netty模块
------
+ 支持HTTP原生处理
+ 支持TCP自定义协议
+ 支持自定义协议扩展
+ 支持多协议并行处理
+ 支持扩展协议可配置

### XTools模块
------
+ 提供lib使用中所需的常用工具，如：xml，json，properties，ymal等工具
