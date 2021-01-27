## swagger2自动生成离线html和PDF文档
使用方式：
* 可以参考我的博客：https://blog.csdn.net/han_chuang/article/details/98748944
* 下载后导入到idea中，然后等待pom下载相关依赖
* 下载完依赖后，在pom.xml文件中修改swaggerInput为项目对应的swagger在线文档地址。(比如：http://localhost:8088/v2/api-docs)
* 然后使用maven工具栏点击clean和test就会在target/asciidoc/html和target/asciidoc/pdf生成对应的文档信息

## 数据库中的pdf依赖这个版本是在公共私服下载不到的，需要将jar转成pom,如下命令：
mvn deploy:deploy-file -DgroupId=org.asciidoctor -DartifactId=asciidoctorj-pdf -Dversion=1.5.0-alpha-zh.16 -Dfile=D:\idea_sample\swagger2-demo\asciidoctorj-pdf-1.5.0-alpha-zh.16.jar -DrepositoryId=maven-releases -Durl=http://ip:port/repository/maven-releases/

<dependency>
    <groupId>org.asciidoctor</groupId>                        
    <artifactId>asciidoctorj-pdf</artifactId>                        
    <version>1.5.0-alpha-zh.16</version>                      
</dependency>                   




