# 快速启动
本部分让用户能够快速开始使用本项目,了解本项目的大概功能. 请注意在输入命令的时候使用英文标点符号. 

虽然您可以使用浏览器自带的翻译功能,但是为了统一名称, 关键按钮等还是使用英文描述.

1. 安装 Label Studio：
```
pip install label-studio
```

2. 启动 Label Studio
```
label-studio start
```
如果您不明白以上两步怎么操作,请查看[安装说明](..\Install\install.md)

3. 在浏览器中输入 http://localhost:8080

4. 使用您创建的电子邮件地址和密码进行注册,不需要邮箱认证

5. 单击“Create”以创建项目并开始标记数据.
   
6. 点击"Project Name"来输入项目的名称

7. 单击“DataImport”并上传要使用的数据文件。这一步骤只能上传少量图片,如果上传多张图片会卡死. 如果想要上传大量图片,请参看 # TODO,并且暂时跳过此步骤。

8. 点击"Labeling Setup", 并选择一个数据标记的模板. 

如果要标记PCB板上的元件的方框,使用Computer Vision> Object Detection with Bounding Boxes;

如果要标记PCB板上元件的精细轮廓, 使用Computer Vision> Semantic Segmentation with Masks来涂抹出元件的形状, 或者使用Semantic Segmentation with Polygons画出元件的轮廓

9. 单击“保存”以保存您的项目。

您已准备好开始标记和注释您的数据！