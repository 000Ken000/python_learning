## 直接先安装anaconda
### 安装python3 
1. 官网下载python3.7安装包，mac终端输出``$ python3``,检查是否安装成功。
2. 安装pip.
3. 安装第三方库
```
$ pip3 install numpy
$ pip3 install pandas
$ pip3 install matplotlib
$ pip3 install scipy
$ pip3 install --upgrade pip
$ pip3 install tushare
$pip3 install tushare -upgrade 
```
##install pip
安装pip
安装Python2.7以上版本，会自动带pip。
系统自带的python没有pip，只有easy_install
Python3高版本自带pip3
// 给系统的python安装pip
easy_install pip
检验pip
// 系统自带的
pip -v
//brew安装的
pip3 -v
6 安装ipython
// 系统自带的
pip install ipython
//brew安装的
pip3 install ipython

```

## 疑问
直接在终端默认界面输出pip3命令行，不要先输入python3命令行进入python3环境，否则会出错。

问题描述：
背景环境：mac mojave v10.14.1, 在已经安装python3.7的背景下，并通过pip3在终端通过命令行安装三方库存，python3.7及相关三方库在储存路径为/Library/Frameworks/Python.framework/Versions/3.7/bin/python3
之后，再安装anaconda3-5.0.1，启动jupyternotebook，编写代码调用tushare运行后失败！

    输入：
    `import tushare as ts
    ts._version_`
    
    输出
    `---------------------------------------------------------------------------
    ModuleNotFoundError                       Traceback (most recent call last)
    <ipython-input-2-28704fedd8c3> in <module>()
    ----> 1 import tushare as ts
          2 ts._version_
    
    ModuleNotFoundError: No module named 'tushare'
    `

最佳解决方案：
1、环境变量问题：https://zhuanlan.zhihu.com/p/61717000
2、在终端通过pip install tushare 安装和pip install tushare --upgrade升级
3、在终端输出python进行python模式，输入import tushare
print(tushare.__version__)，回车查看tushare版本
4、在jupyter notebook输入import tushare
print(tushare.__version__)，运行查看tushare版本，成功！
