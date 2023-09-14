# JSource-Obfuscator

> Why I write this?
>
> - 学习混淆加密的相关姿势
> - 市面上大多都是混淆class文件，配置繁琐，并且极易跑不起来
> - 混淆java文件，即可以重修打包，打包能过，项目十有八九也可以运行，并且混淆java文件，自由度更高，可以适配修改甚至二次混淆等等
> - java文件层的混淆，即使反编译后也难以阅读，确实可以极大增加审计难度
> - 以后出题ex选手🐶

### 混淆功能

- 类名、方法名、字段命名混淆
- 字符串混淆

### Quick Start

--path 指定java文件目录，会直接替换掉原来的java文件，请**注意备份⚠️！！！**

```
java -jar JSource-Obfuscator-1.0-SNAPSHOT.jar --path /Users/1ue/Downloads/obf-test/src/main/java
```

使用JSource-Obfuscator加密如下示例代码

![截屏2023-09-14 14.37.03](images/%E6%88%AA%E5%B1%8F2023-09-14%2014.37.03.png)

```
(base) 1ue@zhdeMacBook-Pro target % java -jar JSource-Obfuscator-1.0-SNAPSHOT.jar --path /Users/zhchen/Downloads/obf-test/src/main/java
 ╦╔═╗┌─┐┬ ┬┬─┐┌─┐┌─┐  ╔═╗┌┐ ┌─┐
 ║╚═╗│ ││ │├┬┘│  ├┤───║ ║├┴┐├┤ 
╚╝╚═╝└─┘└─┘┴└─└─┘└─┘  ╚═╝└─┘└  

usage: --path 指定混淆的java目录

begin obfucate strings...
finished!!!
```

混淆后的代码大致如下

![截屏2023-09-14 14.40.54](images/%E6%88%AA%E5%B1%8F2023-09-14%2014.40.54.png)

并且正常运行

![截屏2023-09-14 14.41.46](images/%E6%88%AA%E5%B1%8F2023-09-14%2014.41.46.png)

### TODO-List

