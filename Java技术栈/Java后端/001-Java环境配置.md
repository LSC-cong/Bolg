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

- Git代码版本控制

  - 下载Git，官网下载：https://gitforwindows.org/
  - 安装Git，勾选如下：

  ![image-20211115160021434](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151600464.png)

  - 下一步

  ![image-20211115160253127](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151602154.png)

  - 这个界面是调整您的PATH环境。第二种配置是“从命令行以及第三方软件进行Git”。该选项被认为是安全的，因为它仅向PATH添加了一些最小的Git包装器，以避免使用可选的Unix工具造成环境混乱。 您将能够从Git Bash，命令提示符和Windows PowerShell以及在PATH中寻找Git的任何第三方软件中使用Git。这也是推荐的选项。

![image-20211115160602062](https://raw.githubusercontent.com/LSC-cong/Bolg/main/cloudimages/202111151606088.png)
