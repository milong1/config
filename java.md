# java

## 下载

地址https://www.oracle.com/java/technologies/javase-downloads.html

下载完了直接装

## 配置

系统变量中，增加/设置：

- 变量名：JAVA_HOME
- 变量值：C:\Program Files (x86)\Java\jdk1.8.0_91     // 要根据自己的实际路径配置

- 变量名：CLASSPATH
- 变量值：.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar;     //记得前面有个"."

- 变量名：Path
- 变量值：%JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;   //分开来

其中没有jre的话：

管理员cmd，进入D:\conf\java，命令`bin\jlink.exe --module-path jmods --add-modules java.desktop --output jre`，ok

## 测试

java --version

