# 伍佰搜服系统使用说明书
一、后台系统使用说明书

**1.运行环境**
- IIS7.0以上
- Microsoft .NET Framework 4.0，安装包地址：https://www.microsoft.com/zh-cn/download/details.aspx?id=17718
- MVC4.0以上， 安装包地址：http://www.jb51.net/softs/103800.html
- 数据库为sqlserver2008以上

**2.数据库部署**
- 下载数据库脚本文件，并以此执行
- 脚本文件下载地址为：

**3.数据库连接字符串配置**
- 打开目录Config，找到DaoConfig.xml文件，使用记事本打开
- Data Source后面的ip地址改为你数据库的ip地址，User ID后面的账户名改为你数据库的登录名，password改为你数据库的登录密码

**部分配置文件说明**
- 配置文件都在Config目录下

| 项目        | 内容          |备注 |
| ------------- |:-------------:|:-----:|
| AdminMenuConfig.xml      | 导航目录配置栏 |请不要删除里面的内容，可以修改里面的AdminMenu name来达到修改导航栏名称的目的  |
| CacheConfig.xml     | 全局缓存配置文件  | minitus为缓存时间（分钟），如非必要，不要修改；其他内容不得删改 |
| DaoConfig.xml     | 数据库连接字符串配置文件| 按照第3个步骤进行数据库连接字符串进行配置 |
| Log4net.xml     | 日志配置文件|请在专业人士指导下修改  |
| SettingConfig.xml    | 后台网址标题配置文件|修改WebSiteTitle之间的内容就可以实现后台标题自定义  |
| SystemConfig.xml     | 系统配置文件|请勿删改  |
| UploadConfig.xml    | 文件上传配置文件|请勿删改  |
