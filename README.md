
# UnitreeG1 Part Detection

This is a simple UnitreeG1 Part Detection programm it uses Yolov8 and DetectNet is puts bounding boxes around the arms head legs and body/chest of the unitreeG1 


## Installation

Install yolov8

```bash
  pip install ultralytics
```
Train AI model

```bash
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=300 imgsz=640
```
Validate The model

```bash
yolo task=detect mode=val model=/home/nvidia09/project/data/runs/detect/train6/weights/best.pt data=data.yaml
```

Now Predict the model

```bash
yolo task=detect mode=predict model=runs/detect/train3/weights/best.pt source=/home/nvidia09/project/data/UnitreeG1.jpeg
```

```
When You are ready click the UnitreeG1DemoPicture.jpeg to view one of the many images i have for this project
```
