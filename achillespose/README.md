# AchillesPose 

## 简介
基于人体骨骼关键点的跑步姿态评估项目。整个项目分为两个主要部分，人体骨骼关键点识别和跑步姿态标准评估。

## 安装
1. 安装相关依赖包  
``` pip install -r requirements.txt```
2. 下载与训练模型**duc_se.pth**([Google Drive](https://drive.google.com/file/d/1x_Oi2I0KceJDk4b0-a47CRY0DC0-_kjF/view?usp=sharing))和**yolov3-spp.weights**([Google Drive](https://drive.google.com/file/d/1hJfSOMtcMWhbLNyejGu4FNwBCyTWE9p2/view?usp=sharing))，拷贝到 ``` ./models.sppe``` 和 ``` ./models/yolo```

## 运行
1. 获取人体关键点识别结果  
```python single_thread.py --video video_path --device GPU  --detbatch 1 --outdir /directory/to/save/result  --vis --save_video```

## 跑步姿态标准
[现行标准](https://docs.google.com/spreadsheets/d/1qdN8ysYR7LHV1DloGBMoyXg8e3HwxfkZyoYzkeR3VU8/edit#gid=0)