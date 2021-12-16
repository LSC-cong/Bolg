# 一、MySQL安装与配置（v5.7）

1. 到官网，https://dev.mysql.com/downloads/mysql/，找到Windows (x86, 64-bit), ZIP Archive免安装版本，下载5.7版本比较稳定。
2. 在`D:\mysql-5.7.35-winx64`目录下新建my.ini文件

```java
[mysql]
# 设置mysql客户端默认字符集
default-character-set=utf8
 
[mysqld]
# 设置端口号
port=3306

# 设置mysql的安装目录，即解压目录
basedir="D:\mysql-5.7.35-winx64\"

# 设置数据库的数据存放目录
datadir="D:\mysql-5.7.35-winx64\data"

# 设置允许最大连接数
max_connections=200

# 设置允许连接失败次数
max_connect_errors=10

# 设置服务端的默认字符集
character-set-server=utf8

# 创建表使用的默认存储引擎
default-storage-engine=INNODB
 
[WinMySQLadmin]  
Server = "D:\mysql-5.7.35-winx64\bin\mysqld.exe"
```

3. 配置Mysql的环境变量，修改系统变量中的Path，添加`D:\mysql-5.7.35-winx64\bin`

![image-20211215222012682](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202112152220741.png)

4. 以**管理员**的身份打开**命令行运行窗口**，输入`mysqld --initialize`。执行这条命令需要花一定的时间(大概几秒，根据电脑情况)，不会有返回结果，但是可以在MySQL的安装目录下看到，原本为空的data文件夹里面有了许多文件和文件夹

5. 接着输入`mysqld -install`。当看到Service successfully installed时，表示Mysql服务添加成功

6. 输入命令`net start mysql`，启动Mysql服务

7. 登录mysql后，修改密码（默认密码为空）

    （1）以管理员身份打开“命令行窗口”，输入mysql -u root -p并按下回车键

    （2）在弹出Enter password: 时，继续按下回车键，即可登录mysql

    （3）输入命令use mysql;

    （4）输入命令ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '新密码'; （注意末尾要有分号）

    （5）输入命令flush privileges; 

    （6）输入命令exit;

# 二、Navicat安装与配置（v15）

Navicat安装配置与使用说明。（百度云：西汉丐帮）

链接：https://pan.baidu.com/s/1yP60p07h4FuGUPeglIvjhw 
提取码：6vzh