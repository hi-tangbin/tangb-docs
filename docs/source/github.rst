

==============================
GitHub
==============================

+--------+------------+----------------------+-----------------------------------------------+
| 版本   | 更新日期   | 编辑                 | 说明                                          |
+========+============+======================+===============================================+
| v1.0.0 | 2022.10.27 | 唐斌: 7120094@qq.com | 整理并归档                                    |
+--------+------------+----------------------+-----------------------------------------------+

1. GitHub 访问加速
==============================

**可以通过以下三种方式加速 GitHub 的访问**


1.1 使用镜像网站
------------------------------

使用github的镜像网站 https://hub.fastgit.org/ 进行搜索


1.2 使用代理网站下载
------------------------------

对于github release中下载的大文件

使用 https://toolwa.com/github/ 来下载，速度起飞,无需注册，亲测有效。


1.3 CDN加速
------------------------------

通过修改系统hosts文件的办法，绕过国内dns解析，直接访问GitHub的CDN节点，从而达到github访问加速的目的。不需要海外的服务器辅助。

GitHub在国内访问速度慢的问题原因有很多,但最直接和最主要的原因是GitHub的分发加速网络的域名遭到dns污染,下载网站上任何东西的时候会下半天,有时还会失败需要从头再来,多失败了几次又因访问次数过多被做了ip限制,让人恼火

做到以上需要三步

1. 获取GitHub官方CDN地址
2. 修改系统Hosts文件
3. 刷新系统DNS缓存

1.3.1 获取GitHub官方CDN地址
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

* https://www.ipaddress.com/search/

* http://tool.chinaz.com/dns/

**查询以下三个链接的DNS解析地址**

* github.com

* assets-cdn.github.com

* github.global.ssl.fastly.net

1.3.2 修改系统Hosts文件
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

接着,打开系统hosts文件(需管理员权限)。
路径：C:\Windows\System32\drivers\etc

1.3.3 刷新系统DNS缓存
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

最后,Windows+X 打开系统命令行（管理员身份）或powershell

运行 ipconfig /flushdns 手动刷新系统DNS缓存。
