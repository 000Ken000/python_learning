# 常用命令行
命令模式：
python --version #查看python版本
python3 --version #查看python3 版本(返回提示当前安装的是python3 .7.1)
which python3 #s查看python3的安装路径(返回:/Library/Frameworks/Python.framework/Versions/3.7/bin/python3）
python3 #进入python3环境(返回:>>>）
exit() #退出python3环境，返回命令行模式

## 专有名词
pip #Pip installs Packages

## 常用操作命令
环境操作：
sudo vi ~/.bash_profile #检查环境变量
export PATH="/Users/anaconda3/bin:$PATH"（这里要填写自己的路径哦）#手动添加conda环境变量
source ~/.bash_profile #刷新环境变量
conda env -h #查看环境管理的全部命令帮助
conda info -e #查看当前系统下的环境
source activate env_name #激活（进入）某个环境
deactivate env_name #退出某个环境
conda create new_env_name old_env_name #复制某个环境：
conda remove env_name #删除某个环境：

包管理：
conda list #查看已安装的包：
conda list -n xxx #查看指定环境下的包
conda search xxx #查找包
conda update xxx #更新包
conda install xxx、pip install xxx #安装包
conda install -n env_name xxx #指定的安装环境
conda install anaconda #安装anaconda发行版中所有的包
conda remove xxx #卸载包
conda create --name python27 python=2.7 #重新配置环境变量，把2.7版本的python命名为python27，安装在anaconda3下envs文件夹下，命名就是python27
conda activate python27 #从python3切换到python2
conda deactivate #换回python3

pip list #查看已安装的包

### pipg、conda，anaconda的区别
pip可以允许你在任何环境中安装python包，而conda允许你在conda环境中安装任何语言包（包括c语言或者python）

管理conda:
conda --version #检查conda版本
conda update conda #升级当前版本的conda

问题:在mac上成功安装anaconda，在终端命令行输入conda，返回提示不是有效命令
解决:在命令行输入export PATH=~/anaconda3/bin:$PATH #此方法无法永久解决，最有效方法是把python,anaconda和.bash _profile下所有路径都删除
输入conda --version#查看版本，返回conda4.3.30


#os 模块提供了非常丰富的方法用来处理文件和目录。

numpy读取/写入数组数据、文本数据时在mac环境指定的目录路径出错







