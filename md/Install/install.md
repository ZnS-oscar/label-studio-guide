# 安装说明
作为一款开源工具，其优点是免费、有很大的社区快速地维护更新；缺点是安装比较麻烦。以下是label_studio的windows电脑安装教程。本教程没有编程基础的用户也能看懂。

Label Studio还支持Docker安装,Ubuntu安装等, 请参看[官方英文文档](https://labelstud.io/guide/get_started)

简短的说明: 在python 3.6以上版本的环境下使用命令`pip install label-studio`安装,然后输入`label-studio start`启动, 就可以在http://localhost:8080/查看了

# 1.	安装python
Python是一门编程语言，Label_studio需要python 3.6以上的版本。可以通过以下方式检查您的电脑是否符合要求:

1.1. 按住win键后再按R键，在出现的窗口输入cmd，回车，出现黑色命令行窗口。
![运行窗口](md\Install\image.png)


1.2. 在黑色命令行窗口输入 python -V，显示版本号。如果结果为Python 3.X.Y, 而且X大于等于6即满足要求，可以跳过以下步骤，看2.步安装pip。

![alt txt](md\Install\iii.png)

1.3. 开始安装python。进入python官网https://www.python.org/downloads/windows/

![python 官网](md\Install\image-2.png)

1.4. 如果电脑是64位，则点击Windows installer(64-bit)，否则是32位，点击Windows installer(32-bit)。你会下载好一个安装包
查看自己电脑是64位还是32位请[点击此教程](https://baijiahao.baidu.com/s?id=1808041429607662313&wfr=spider&for=pc). 一般而言,2018年以后的电脑大部分是64位的, 2020年以后的电脑绝大部分都是64位的

1.5. 下载好之后双击安装包，出现如下画面。勾选其中的“Add python.exe to PATH”,点击Install Now，稍作等待即可。完成后您便安装好了python 3.12.5版本
![python下载界面](md\Install\image-3.png)

1.6. 您可以通过1.1和1.2步检查python是否安装成功，如果显示Python 3.12.5则安装成功

# 2.	安装pip
Pip是与python配套的包安装工具，我们需要使用这个工具安装label_studio.您可以通过以下方式查看您的电脑是否已经安装好了pip。

2.1	按住win键后再按R键，在出现的窗口输入cmd，回车，出现黑色命令行窗口。

2.2	在黑色的命令行窗口输入 `pip -V`。能够显示pip XX.X.X ….即可跳过以下步骤看3. 安装label_studio
![alt text](md\Install\image-4.png)

2.3	在2.1的cmd窗口当中输入命令`python -m ensurepip --default-pip`出现如下图所示，代表安装成功：
![alt text](md\Install\image-5.png)

2.4	安装完成之后，您可以执行2.1和2.2查看是否安装成功。

# 3.	安装label_studio
安装好了python 3.6以上版本和pip之后，就可以安装label_studio了。

3.1	方法1：按住win键后再按R键，在出现的窗口输入cmd，回车，出现黑色命令行窗口。输入pip install label-studio即可

3.2	方法2：如果方法1不成功，则使用以下3.2-3.3的步骤。首先下载我提供的压缩包label_studio-1.13.1.tar.gz，把它放在任意文件夹下。

3.3. 按住win键后再按R键，在出现的窗口输入cmd，回车，出现黑色命令行窗口。输入`pip install label_studio-1.13.1.tar.gz的位置`。例如我把label_studio-1.13.1.tar.gz放在了D盘下，那么我的指令就是`pip install D:\label_studio-1.13.1.tar.gz`

3.4. 输入label-studio start, 然后在浏览器输入http://localhost:8080/出现以下画面则安装成功
![alt text](md\Install\image-6.png)