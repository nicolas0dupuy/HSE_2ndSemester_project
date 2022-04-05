# COPY of the HeadPoseEstimation-WHENet-yolov4-onnx-openvino
ONNX, OpenVINO, TFLite, TensorRT, EdgeTPU, CoreML, TFJS, YOLOv4/YOLOv4-tiny-3L

## Original repository
https://github.com/PINTO0309/HeadPoseEstimation-WHENet-yolov4-onnx-openvino


**For academic purposes in partnership of the Higher School of Economics Nizhny Novgorod**
**Online Master of Computer Vision** 

## Starting the demo
```bash
$ git clone https://github.com/PINTO0309/HSE_2ndSemester_project
$ cd HSE_2ndSemester_project
$ wget https://github.com/PINTO0309/HeadPoseEstimation-WHENet-yolov4-onnx-openvino/releases/download/v1.0.2/saved_model_224x224.tar.gz
$ tar -zxvf saved_model_224x224.tar.gz && rm saved_model_224x224.tar.gz
$ pip install -r requirements.txt

$ python3 demo.py
```
```bash
usage: demo.py \
[-h] \
[--whenet_mode {onnx,openvino}] \
[--device DEVICE] \
[--height_width HEIGHT_WIDTH]

optional arguments:
  -h, --help
      show this help message and exit
  --whenet_mode {onnx,openvino}
      Choose whether to infer WHENet with ONNX or OpenVINO. Default: onnx
  --device DEVICE
      Path of the mp4 file or device number of the USB camera. Default: 0
  --height_width HEIGHT_WIDTH
      {H}x{W} Default: 480x640
```