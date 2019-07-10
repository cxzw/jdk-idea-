jdk以及IDEA的下载和安装
=======================

# jdk下载以及配置安装
## 下载
先在Oracle官网下载最新的java开发环境包,也就是jdk,需要注册一个甲骨文的账号
https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
但其实速度很慢,我选择了国内某平台下载了不是最新版的jdk,但都是1.8
解压然后打开下载好的文件
![此处输入图片的描述][1]


 一路默认下一步然后等他自动安装就好了
 安装过程中会提示让安装jre，可以根据自己的需要新建安装的文件夹名,建议全部默认
 ![此处输入图片的描述][2]


## 配置环境变量
桌面“我的电脑”右击，选择“属性”打开“系统控制面板”选择“高级系统设置”
![此处输入图片的描述][3]


1. 配置JAVA_HOME，选择“用户变量”新建，输入jdk安装路径；eg：一般选择用户变量就好，这样不会影响系统其它用户；
![此处输入图片的描述][4]


2.配置PATH，变量值填写JDK的安装目录下的bin目录，因“JAVA_HOME”已配置好，所以可通过JAVA_HOME变量来设置，这样比较灵活，下次要变更JDK的话，只需修改JAVA_HOME即可；
 ![此处输入图片的描述][5]


3.配置CLASSPATH，变量值填写JDK相关的jar包，也是通过JAVA_HOME变量来设置，可直接写%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar，然后连续【确定】。
![此处输入图片的描述][6]


## 验证是否配置成功
点击【开始】菜单，收入cmd进入命令模式，输入“java -version”可以查看安装版本
![此处输入图片的描述][7]



输入javac 查看jdk信息
![此处输入图片的描述][8]


 
# IDEA的下载及配置安装

## 下载及安装

IntelliJ IDEA 官网：https://www.jetbrains.com/idea/

安装时只需要选择一下自己是64位还是32位的就好,其他可以全部默认
可以根据博主的文章一步步安装即可https://blog.csdn.net/mashuai720/article/details/79389314

## 破解
http://idea.lanyus.com/
下拉至最下点击注册按钮即可生成一段激活码,在安装后会有激活选项,选择activity code,把上面自动生成的代码复制粘贴进去即可,然后在hosts文件中将IDEA官网的网址和IP地址添加进去防止它自动联网检测即可

## 编码以及properties 文件读取
![此处输入图片的描述][9]
Editor->File Encodings -> Defaule encoding for properties files 属性设置成utf-8
三个选项全都改为utf-8
选中Transparent native-to-ascii conversion

## 序列化接口实现版本号
1.使用Ctrl+Alt+S快捷键打开settings,设置如下图所示
![此处输入图片的描述][10]


  上图中的Disable new inspections by default可以选中，否则每次重启Idea后，都需要重新设置。
  
## 缩进
![此处输入图片的描述][11]


## 换行符

![此处输入图片的描述][12]



  [1]: https://img-blog.csdnimg.cn/20190317171534770.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [2]: https://img-blog.csdnimg.cn/20190317172734708.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [3]: https://img-blog.csdnimg.cn/20190317173837454.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [4]: https://img-blog.csdnimg.cn/20190317174707354.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [5]: https://img-blog.csdnimg.cn/20190317180701117.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [6]: https://img-blog.csdnimg.cn/20190317175755930.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [7]: https://img-blog.csdnimg.cn/20190317180819753.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [8]: https://img-blog.csdnimg.cn/20190317181146278.?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl8zNzYwMTU0Ng==,size_16,color_FFFFFF,t_70
  [9]: https://img-blog.csdn.net/20171129155059833?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2dsMTI1MTY3MDE2/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast
  [10]: https://img-blog.csdn.net/20170707175618090?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvcXFfMzE0OTY4OTc=/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast
  [11]: https://imgsa.baidu.com/exp/pic/item/6391e903918fa0ec86ed29b82d9759ee3d6ddb1a.jpg
  [12]: https://img-blog.csdn.net/20150909130939973
  在设置中设置为unix及mac os即可