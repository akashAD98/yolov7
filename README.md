# yolov7

Implementation of "YOLOv7: Trainable bag-of-freebies sets new state-of-the-art for real-time object detectors"

This implimentation is based on [yolov5](https://github.com/ultralytics/yolov5).

## Object detection

[code](./det)

## Instance segmentation

[code](./seg)

To convert yolov7-seg.pt into onnx & .trt format 

```
python3 export.py --weights yolov7-seg.pt --include torchscript onnx openvino engine coreml tflite
```
inference 

```
!python3 segment/predict.py --weights yolov7-seg.onnx --source "spiderman2.mp4" --project segmentop
```

## Image classification

[code](./det)
