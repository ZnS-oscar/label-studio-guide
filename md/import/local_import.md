# 本地数据批量导入
如 '快速开始' 部分所说, 本软件的大量导入需要使用外部存储. 本文说明从本地导入数据的方法. 本部分参考了[官方-本地数据导入说明](https://labelstud.io/guide/storage.html#Local-storage)

本软件还支持来自亚马逊云, 谷歌云, Redis等作为数据存储, 详见官方文档https://labelstud.io/guide/storage.html

# 1. 设置环境变量
请按照[这篇教程](https://blog.csdn.net/yanyc0411/article/details/135007051)设置如下2个系统环境变量:
```
LABEL_STUDIO_LOCAL_FILES_SERVING_ENABLED=true
LABEL_STUDIO_LOCAL_FILES_DOCUMENT_ROOT=D:\\pcbobb
# windows的地址尽量使用双反斜杠
```
![alt text](image.png)

其中LABEL_STUDIO_LOCAL_FILES_DOCUMENT_ROOT设置了你的数据的根路径. Label Studio会到这个根文件下寻找数据. 用户将需要标注的数据放在这个根文件夹或者根文件夹之下的文件夹.在上面的例子当中, 我的图片则必须存放在D:\\pcbobb之下, 不过我可以放在子文件夹D:\\pcbobb\\image当中,不必直接放在根路径下. 

# 2. 将本地数据加入到Label Studio当中
1. 在网络浏览器中打开 Label Studio。
2. 点击一个项目,点击右上角Setting
3. 单击添加源存储。