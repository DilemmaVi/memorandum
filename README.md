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

**4.部分配置文件说明**
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

**5.后台系统功能说明**

a.系统管理
- 1.用户管理：可以增删查改用户以及赋予用户权限，其中拥有此权限的用户只能重置密码，不能修改密码，默认密码为：111111
- 2.角色管理：增删查改角色，使用轻量级的角色权限管理

b.SEO管理
- 1.文章管理：可以增删查改文章，使用轻量级文本编辑器实现，不支持上传图片，如需使用图片功能，请使用网络在线图片
- 2.文章频道管理：增删查改文章频道，增加一个频道就会在前台增加一个文章展示栏，频道激活数请保证为双数，否则前台展示会错乱
- 2.SEO优化：可以修改前台网站标题，关键词等各种SEO设置，请保证只有一套SEO方案生效，否则会产生未知错误

c.广告及报表
- 1.广告管理：主要功能是发广告，可以使用新增发单条广告和使用批量发广告功能，可撤销的广告在前面会有可勾选的小方框，可改时间的会在操作栏有改时间的按钮
- 2.充值管理：可以对广告管理员进行充值和冲正
- 3.费率管理：可以对各种广告类型的点数进行修改，不支持新增广告类型以及修改广告类型的名字
- 4.报表管理：统计各类型广告数据，首页默认展示近三十天数据，可以自定义时间查询展示，同时提供广告数据表，广告发布记录以及充值数据查询导出

d.日志管理
- 1.充值消费日志：查询广告管理员充值消费的日志
- 2.批量广告日志：查询批量发广告的日志，失败的广告可以点击失败详情查询
- 3.系统日志：系统运行日志，请在专业人士指导下使用


