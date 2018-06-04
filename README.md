## healer [![Build Status](https://travis-ci.org/yuanliccc/healer.svg?branch=master)](https://travis-ci.org/yuanliccc/healer) [![codecov.io](https://codecov.io/gh/yuanliccc/healer/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/gh/yuanliccc/healer?branch=master)  [![GitHub version](https://badge.fury.io/gh/YuanLiccc%2Fhealer.svg)](https://badge.fury.io/gh/YuanLiccc%2Fhealer)
治愈系妹子APP，你懂的！
### 关于如何发布到服务器

1）将项目打包： 

```java
mvn package
```
2）在项目下找到文件夹`target`下找到`healer.war`文件

3）将文件复制到服务器的`/usr/local/volumn/tomcat`下，此文件夹对应普通tomcat的webapps文件夹。

4）执行命令：

```shell
docker restart tomcat
```

5）等待tomcat启动完成，这个很慢，大概需要七八分钟，为什么需要这么久，在网上查阅原因与session有关，从日志可以看出这一步大概耗费了五分钟，该问题暂时未解决。

### 关于如何复制到服务器

1）下载一个工具：[Xftp](http://www.netsarang.com/download/software.html)，这是一个付费的软件，但是beta版是免费的，暂时还没发现怎么找到beta版

2）安装完毕后，连接服务器：120.77.171.82

3）若链接成功后，主屏会分为两个块。左边是本地文件夹管理界面，右面是服务器文件管理界面。

4）复制或拖拽到服务器的指定文件夹下即可。