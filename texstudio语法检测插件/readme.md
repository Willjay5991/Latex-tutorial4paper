## 为texstudio配置语法检测插件的步骤

### 安装JDK

正常安装[JDK-17_windows-x64_bin.exe](https://www.oracle.com/java/technologies/downloads/#jdk18-windows)

配置JAVA环境：

 1. 在系统环境中， 新建 JAVA_HOME 项，并且把JDK的安装根目录作为值

 2. 在系统环境中，编辑path项，新建 %JAVA_HOME%\bin

 3. 确认所有设置

验证JAVA配置

 	1. cmd中输入 `java -version`
 	2. cmd中输入 `java`
 	3. cmd中输入 `javac`



### [配置languageTools](https://languagetool.org/windows)

1. 将languageTools 解压

2. 在其中`languagetools.jar` 路径下打开cmd，运行 `java -jar languagetool.jar`

   配置languagetool

    - Tex checking ---- 选项 ---- general : 勾选 `运行服务器端口 8081`， `对服务其使用以上设置`
    - 确定

### 添加词典

将’dict-en-20211001.oxt‘ 文件拷贝到texstudio 安装目录的dictionaries 目录下



### 配置 texstudio

 	1. options------configure texstudio-----language checking
      	1. server URL:   `http://localhost:8081`
      	2. java:    'D:\application\JDK\bin\javaw.exe'    # java 路径
      	3. LT path:  'D:\application\latex\LanguageTool-5.5\languagetool.jar'  # languagetool 路径
      	4. 其他默认

### 测输文本纠错能力

重启texstudio

输入 `you is right`

