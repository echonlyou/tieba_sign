# 百度贴吧云签到
#可以快速部署到OpenShift平台，集成常见插件。#
在服务器上配置好就无需进行任何操作便可以实现贴吧的全自动签到。     
配合插件使用还可实现云灌水、点赞、封禁、删帖、审查等功能。     
获取插件，教程，扩展，资料等请前往Wiki [Git@OSC](https://git.oschina.net/kenvix/Tieba-Cloud-Sign/wikis/home) [GitHub](https://github.com/MoeNetwork/Tieba-Cloud-Sign/wiki)              

## 常见问题解决方案
往往大部分人安装出错第一反应都是：“没错啊，哪里错了，一定是程序错了”
##### 1.如何安装程序
上传此程序到您的网站，然后访问您的网站
##### 2.如何开启 MySQL 连接方式强制功能
如果数据库配置正确，但连接数据库失败（错误代码 20XX），可使用此方法     
打开   mysql_autoload.php     
找到   define('SQLMODE', 'mysqli');     
替换为 define('SQLMODE', 'mysql');
##### 3.如何开启数据库长连接
打开   mysql_autoload.php     
找到   define('LONGSQL', false);     
替换为 define('LONGSQL', true); 
##### 4.如何手动修改数据库配置
打开 config.php 并按照里面的注释修改     
切勿使用记事本编辑，否则程序将不能工作
##### 5.如何手动导入数据库
打开 /setup/install.template.sql 并按照里面的注释修改
##### 6.如何安装新版本
（1）自动更新：前往 检查更新 更新程序即可     
（2）手动更新：直接下载 Zip，删除压缩包内的 config.php ，然后上传到您的网站即可     
另外，每一个大版本都会有一个升级脚本，别忘了运行它     
（文件名一般为 update旧版本to新版本.php ，例如 update1.0to2.0.php）

