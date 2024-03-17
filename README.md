# Yolo_V9-Custom_Dataset
'''This Reposistory will helps to create &amp; Train you custom Dataset ,which is already annotated &amp; Well structured in Folders: train,Test,Val
## Environment setup:
git clone https://github.com/WongKinYiu/yolov9.git

cd yolov9

pip install -r requirements.txt

## Train model -
!python train_dual.py --workers 8 --batch 4 --img 640 --epochs 50 --data /mydrive/yolov9/yolov9/data.yaml --weights /mydrive/yolov9/yolov9-e.pt --device 0 --cfg /mydrive/yolov9/yolov9/models/detect/yolov9_custom.yaml --hyp /mydrive/yolov9/yolov9/data/hyps/hyp.scratch-high.yaml

## Detections using custom trained model:
!python detect.py --img 1280 --conf 0.1 --device 0 --weights /mydrive/yolov9/yolov9/runs/train/exp9/weights/best.pt --source /mydrive/yolov9/test.jpg
