
#  build 构建项目
    工程右侧目录 GoatGradle  --->  chapter0-0-8 ---> Tasks ---> build ---> build 开始执行项目构建
    构建后： 项目中的build目录下  libs 下生成了 chapter0-0-8-1.0-SNAPSHOT.jar
    
    原理：
    是根据当前模块根目录下的 build.gradle 文件 相当于 maven中的 pom.xml文件
    
# 执行jar
    打开IDEA Terminal 输入命令： java -jar chapter0-0-8/build/libs/chapter0-0-8-1.0-SNAPSHOT.jar
    报错：  chapter0-0-8/build/libs/chapter0-0-8-1.0-SNAPSHOT.jar中没有主清单属性
    再次输入命令： 
     报错：   java  -jar chapter0-0-8/build/libs/chapter0-0-8-1.0-SNAPSHOT.jar com.goat.chapter009.App
     正确：   java  -classpath chapter0-0-8/build/libs/chapter0-0-8-1.0-SNAPSHOT.jar com.goat.chapter009.App
   
