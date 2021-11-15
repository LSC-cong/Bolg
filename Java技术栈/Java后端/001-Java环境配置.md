[TOC]

# 一、安装JDK

JRE，即Java Runtime Enviroment。提供了Java的运行环境

JDK，即Java Development Kit。提供了Java的开发环境和运行环境

1. 下载链接（java8、11、17）：https://www.oracle.com/java/technologies/downloads/#java8-windows
2. 安装的时候会两次选择安装路径，第一次是JDK安装路径，第二次是JRE安装路径。
2. 配置环境变量
   - 我的电脑 - 属性 - 高级系统设置 - 环境变量 - 系统变量
   - 修改3个地方：
     - 新建：JAVA_HOME       D:\JDK
     - 新建：CLASSPATH        .;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar
     - 修改：Path                     %JAVA_HOME%\bin      （在Path中新建一条，并将其移到第一行）

![image-20211115110157860](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151101916.png)



# 二、安装IDEA

1.官网下载：https://www.jetbrains.com/zh-cn/idea/download/#section=windows

![image-20211114225514251](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111142255552.png)

2.安装

![](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151000239.png)

3.可以登录教育账号，免费使用，有效期一年，一年后重新认证即可

4.安装配置好了jdk后，在IDEA中，通过选择jdk的路径，3选择jdk版本，

![image-20211115111212294](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151112326.png)

5.搞定了！

6.IDEA的个性化设置

- 设置IDE界面主题及字体（推荐13号，默认字体；Darcula主题）

![image-20211115150625449](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151506550.png)

- 设置代码字体（推荐18号，Fira Code字体）

![image-20211115150738076](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151507164.png)

