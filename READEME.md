# 第一节
## github关键字查询
`awesome` **去此类别中查询项目**<br>
python `tutorial` **查询资料、书籍、文档**<br>
socket `sample` **查询对应技术的代码样本**<br>

## Github三要素
### Repository仓库
仓库是github项目管理存储基本单位<br>
一个仓库中存储一个项目，一个用户可以有多个仓库，一般仓库分为public、private<br>
### Commit提交
程序员在整个开发周期，有大量的对代码资源的选代和修改，都可以通过commit的方式进行记录,便于程序员回溯代码, 即使这些代码被删除提交便于使用者观察整个工程的开发流程以及设计流程<br>
### Branch分支
在仓库中可以包含多个分支，分支才是代码文件的第一存储单位，默认的仓库主分支为`master/main`，**可以管理代码存储，便于多人协作开发**
[![1.jpg](https://i.postimg.cc/Nf4XZhT8/1.jpg)](https://postimg.cc/mtPhF5mh)

## 仓库内容
`Code：`资源存储、代码资源、二进制、项目管理脚本、许可证等等<br>
`issue：`使用时遇到的bug 或 进行提交，等待反馈<br>
`README:`使用maekdown语言编写，工程自述文件、开发进度、版本更新、使用介绍等等<br>
`LICENSE许可证:`**GPL2.0、3.0 ，Apahce2.0 ，Mit** 这些许可证，给使用者最大使用权限以及最少的限制<br>
## Git软件、分布式版本控制系统
仓库管理软件，使用git管理私人代码或企业代码<br>
[![20240607212115.jpg](https://i.postimg.cc/KcR0X0wL/20240607212115.jpg)](https://postimg.cc/MXJ7VmWK)
## 设备认证
1. 绑定网站账户及本地设备，方便后续代码管理
```cpp
	git init //创建本地仓库           
	git config --list //查看git的配置文件
	git config --global user.email "邮箱"
	git config --global user.name "用户名"
	ssh-keygan -t rsa -C "注册邮箱" //创建本地密文
	//去对应的目录查找密文文件
	rsa.pub 复制密文，粘贴 settingds-> SSh key and GPG -> new ssh key -> 粘贴
	ssh -T git@github.com //测试关联是否成功
```
2. 为仓库起别名，定位目标仓库，后续上传
```cpp
	git remote add origin "ssh地址" //为ssh仓库地址创建别名为origin
	git remote remove origin //删除origin别名
	git remote add origin "ssh地址" //再次起别名
```
## 本地设备与云端仓库的交互逻辑
[![20240607213615.jpg](https://i.postimg.cc/j5TBCxD9/20240607213615.jpg)](https://postimg.cc/xks64Syy)
```cpp
	git status //查看状态
```
## 代码更新的依赖关系被破坏
一般本地内容要比云端新，完成更新替换，若直接修改云端内容，会导致本地内容无法再次提交，就需要**先拉取git pull 云端内容与本地内容合并，然后再上传**<br>


# 一级标题
## 二级标题
### 三级标题
#### 四级标题

*测试文本：斜体* <br>
**测试文本：加粗** <br>
***测试文本：斜体加粗***

~~文本划线~~

## 设备认证
### 1,绑定用户设备和网站账户
*git init*  
创建本地仓库 <br>
*git config --list* 查看git的配置文件<br>

## 表格
名称|技能|排行
--|:--:|--:
蝙|钱|12
蜘蛛侠|新闻|123

## 代码片段
```cpp
	#inlcude <iostream>
	using namespace std;
	int main()
	{
		printf("rec");
		return 0;
	}
```
```python
	rcscrsc
	srcsefrsc
	eadeccer
```
这是一个`重点标记`的文本。
