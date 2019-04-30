#### 1、subline text3安装
下载subline text3地址：https://github.com/GMerrr/subline-text3/
下好了安装。
#### 2、安装package control
下载地址：https://github.com/GMerrr/subline-text3

安装步骤：

```
下载 package_control-master.zip 解压，重命名为："Package Control"
打开subline text3 -> Preferences -> Browse Packages 
将Package Control文件夹拷贝进去。
重启subline。
```

#### 3、解决subline text3 不能install

打开subline text3 -> Preferences -> Package Settings -> Package Control -> Settings-User
加入内容

```
{
	"bootstrapped": true,
	"channels":
	[
		"https://raw.githubusercontent.com/HBLong/channel_v3_daily/master/channel_v3.json"

	],
	"in_process_packages":
	[
	
	],
	"installed_packages":
	[
		"Emmet",
		"Package Control"
	]
}
```

#### 4、sublime text3解决Gosublime无法自动补全代码

package install Gosublime;

安装好后设置Perferences –> Package Settings –> Gosublime –> Settings - User

```
{
    "env": {
        "GOPATH": "F:/01go",
        "GOROOT": "C:/Go"
    }
}
```

在windows上subline text3还是写go还是不能进行代码自动补全，解决方案：

```
打开Perferences–Browse Packages…，进入Gosublime：
1、在src目录下创建margo目录；
2、拷贝src/margo.sh/extension-example/extension-example.go文件到margo目录下；
3、拷贝margo文件夹（所有文件和目录）到src/margo.sh/vendor目录下；

转自：https://blog.csdn.net/CodyGuo/article/details/89199597
```

重新打开sublime text3，稍等几分钟就可以自动补全代码了。