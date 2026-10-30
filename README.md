# Lab02 - VinaFood21 CNN Classification
 
## Cài đặt
pip install -r requirements.txt
 
## Dữ liệu
Đặt dữ liệu tại data/VinaFood21/{train,val,test}. Nếu thiếu val/, code tự tách 10% từ train.
 
## Huấn luyện
python train.py --config configs/lenet5.yaml
python train.py --config configs/googlenet.yaml
python train.py --config configs/resnet18.yaml
python train.py --config configs/resnet50.yaml
 
## Đánh giá lại
python evaluate.py --config configs/lenet5.yaml --exp lenet5_avgpool
 
Kết quả lưu trong outputs/<tên_thực_nghiệm>/.