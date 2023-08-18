# HandDetection
 ## Using YOLOV8
 ### Install Requirement
 ```
 pip install -r requirements.txt
 ```
### Install Ultralytics
```
pip install ultralytics
```
### Train model
```
python train.py
```
### Export model to onnx file
```
yolo export model=best.pt imgsz=640 format=onnx opset=12
```
### Use Model to detect hand in a picture
```
python main.py --model best.onnx --img image.jpg
```

