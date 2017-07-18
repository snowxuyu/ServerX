# 需求概述

### 相关组件
* System Define（Default、Annotation）
* Startup（Load Config、Bind address）
* Configuration (Filter、init、web)
* Spring       （Factory、MVC）
* Netty        （HTTP、TCP）
* XTools       （XML、JSON）

### config模块

+ 支持的配置文件类型：ymal，json，xml，properties
+ 提供多种配置文件加载方式：String，File，Stream
+ ConfigFactory 统一对外提供Value获取接口（K,V）
+ 提供配置文件修改接口：修改值或替换全部，并重新加载
+ 支持任意自定义配置，可方便用户进行扩展
+ 配置加载时，需要对配置项进行校验：必选配置，可选配置

### xtools模块

+ 提供lib使用中所需的常用工具，如：xml，json，properties，ymal等工具

### system模块

+ 系统常量定义，相关注解，枚举，协议等lib使用所需的数据类型定义
