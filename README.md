# yolov5

train:
在/codes目录里运行
python yolov5/train.py --img 512 --batch 32 --epochs 500 --data data.yaml --cfg models/yolov5s.yaml  --name TEST
img: image size
batch: batch_size
epochs: epochs
data: parameters of dataset
cfg: parameters of model
name: named for this training

test:
在/codes/yolov5目录里运行
python detect.py --weights ./codes/runs/train/IHC/weights/best.pt --img 512 --conf 0.15 --source ./data/images/test
weights: best saving model path
img: image size
conf: confidence
source: testing dataset path

data.yaml:
training dataset path
validation datset path
number of classes
class name
