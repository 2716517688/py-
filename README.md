# py-
let input str list change to math list

​		固件pytest的python运行环境是3.7   3.7大版本上的小版本不限。

​        python Windows安装程序下载地址：https://www.python.org/downloads/windows/python-3.7.8-amd64

​        **写搭建文档时使用的是3.7.8版本的python**

​        windows环境下，下载安装包：https://www.python.org/ftp/python/3.7.8/python-3.7.8-amd64.exe

​         如果不好下载，可以使用ftp上的备份：ftp://192.168.10.20/incoming/wangdh/python-3.7.8-amd64

​         双击执行安装程序，之后界面上选择安装，选择**将python添加到环境变量**，然后一直下一步默认安装即可。
#### 2.pip3安装python库

    pip3 install pytest allure-pytest numpy lxml namedlist xlrd==1.2.0 harvesters 



#### 3.安装allure工具支持包 

​         下载地址：https://[github](https://so.csdn.net/so/search?q=github&spm=1001.2101.3001.7020).com/allure-framework/allure2/releases

​          或者ftp：

​          这里使用的是：https://github.com/allure-framework/allure2/releases/download/2.17.3/allure-2.17.3.zip 这个版本的包

​          下载zip包后，解压到想解压的位置，然后将对应路径下的/bin 添加到环境变量

​           在命令行测试一下： 

    	 allure --help

​           没有报错就通过了。
#### 4.可选功能列表测试程序将python解释器程序修改为GalaxyView

​    例如我自己的python程序路径为：

```shell
C:\Users\wangdh\AppData\Local\Programs\Python\Python37
```

目录中存在一个python.exe的可执行文件，需要将这个文件复制一份然后修改名字为GalaxyView.exe

![python](\pic\python.PNG)

在执行可选功能列表测试工具时，使用换名后的GalaxyView作为解释器 (否则枚举不到相机)

```shell
     GalaxyView ./main.py
```
![run](\pic\run.PNG)





#### *附录：

​          使用allure生成的报告文件直接使用html无法打开，需要使用allure命令打开：

      allure open [报告存放目录]



​    
真的吗