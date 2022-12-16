## VOC数据集
### 目标检测
文件结构：

```ini
taskname.zip/
├── images/                                         # 图像文件夹
│   ├── <image_name1>.jpg
│   ├── <image_name2>.jpg
│   └── <image_nameN>.jpg
└── annotations/                                    # 标注文件夹
│   ├── <image_name1>.xml
│   ├── <image_name2>.xml
│   └── <image_nameN>.xml

```

xml格式：
自定义字段:

- rotate_angle: 旋转角度，顺时针为正，单位为度

```XML
<annotation>
  <folder>VOC2012</folder>                          # 图像所在文件夹
  <filename>2007_000032.jpg</filename>              # 图像文件名
  <source>                                          # 图像源
    <database>The VOC2007 Database</database>
    <annotation>PASCAL VOC2007</annotation>
    <image>flickr</image>
  </source>
  <size>                                            # 图像尺寸信息
    <width>500</width>                              # 图像宽度
    <height>281</height>                            # 图像高度
    <depth>3</depth>                                # 图像深度，也就是通道数
  </size>
  <segmented>1</segmented>                          # 图像是否用于分割
  <object>                                          # 一个目标对象的信息
    <name>aeroplane</name>                          # 目标的类别名
    <pose>Frontal</pose>                            # 拍摄角度，Unspecified
    <truncated>0</truncated>                        # 是否被截断，0表示完整未截断
    <difficult>0</difficult>                        # 是否难以识别，0表示不难识别
    <bndbox>                                        # 边界框信息
      <xmin>104</xmin>                              # 左上角x
      <ymin>78</ymin>                               # 左上角y
      <xmax>375</xmax>                              # 右下角x
      <ymax>183</ymax>                              # 右下角y
      <rotate_angle>2.889813</rotate_angle>         # 旋转角度,默认为0，顺时针为正
    </bndbox>
  </object>
                                                    # 下面是其他目标的信息，这里略掉
  <object>
    ...
  </object>
</annotation>
```
### 语义分割
目录结构
```
demo_dir
 ├── annotations
 │   ├── labelmap.txt
 │   └── SegmentationClass
 │       ├── 1.png
 │       ├── 2.png
 │       └── 3.png
 └── images
     ├── 1.jpg
     ├── 2.jpg
     └── 3.jpg
```
labelmap.txt格式
```
# labelmap.txt
# label : color (RGB) : 'body' parts : actions
background:0,128,0::
aeroplane:10,10,128::
bicycle:10,128,0::
bird:0,108,128::
boat:108,0,100::
bottle:18,0,8::
bus:12,28,0::
```
