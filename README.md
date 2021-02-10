# linux常用命令



### linux文件操作核心命令

cd	切换目录

pwd	查看当前目录

ls,ll	显示目录内容

mkdir	创建目录

cp	复制文件与目录

mv	移动或者重命名文件

rm	删除文件或者目录

find	查找目录或者文件



### vim三种模式

普通模式：默认模式，文本只读，不可编辑

编辑模式：编辑文本模式，普通模式按i键进入，Esc键退出

命令模式：执行保存，搜索，退出等操作

### vim重要快捷键

delete或x	删除单个字符

dd	删除整行

/str	全文查找str字符串，n下一个，N前一个

:% s/old/new/g	替换文件内所有old字符串为new

u	撤销最近一次操作

:wq或者:wq!	退出并保存，只读文件要额外加！

:q!	强制退出放弃保存



### 常用文本工具

echo	屏幕打印与文本输出

cat	合并文件或查看文件内容

tail	显示文件内容尾部

grep	文本过滤工具



### tar打包与压缩

压缩命令：tar zcvf tomcat.tar.gz /usr/local/tomcat

解压缩命令：tar zxvf tomcat.tar.gz -C /usr/local/tomcat

### tar常用可选项

z	通过gzip压缩或解压

c	创建新的tar.gz文件

v	显示执行 过程

f	指定压缩文件名称

x	解压缩tar.gz文件

-C	指定解压缩目录



### yum常用命令

yum search	应用名 #在仓库中查询是否存在指定应用 

yum install -y	应用名 #全自动下载安装应用及其依赖

yum info 	应用名 #查看应用详细信息

yum list installed 应用名 #查看已安装的应用程序

rpm -ql 应用名 #查看安装后输出的文件清单

yum remove -y 应用名 #全自动卸载指定应用

### 编译方式安装应用程序

如果yum仓库未提供rpm，往往需要采用编译安装方式

编译安装是指从应用官网下载源码后，对源码进行编译后使用

编译命令：make #使用对应编译器对源码编译生成可执行文件

