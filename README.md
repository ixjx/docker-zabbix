# docker-zabbix

基于官方的 docker-compose zabbix 3.4

使用 Ubuntu14.04 mysql nginx

修改了时区 PHP_TZ=Asia/ShangHai

增加黑体字体解决中文乱码

### 存储

Compose文件已经配置为支持主机的本地存储。当你使用compose文件运行Zabbix组件时，将在compose文件所在的文件夹中创建一个zbx_env目录。这个目录将包含Volumes的相同结构，以用于数据库存储。

/etc/localtime 和 /etc/timezone 卷下的文件为只读模式。

### 环境变量文件

环境变量文件的命名类似于.env_<组件类型>

### begin

`# docker-compose up -d`

默认nginx端口为8081，通过 http://localhost:8081 访问web界面