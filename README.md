# Equations-solver
## 1. Tải weight và darknet
- Tải weight file tại https://drive.google.com/drive/folders/1S1Erf46mekv9FFRBgLlLJC_Sqwe3sjx9?usp=sharing
- Tải darknet tại https://github.com/AlexeyAB/darknet.git
## 2. Config
- Sau khi tải Darknet, vào thư mục darknet/config tạo bản sao của yolov4-custom.cfg và đặt tên là yolov4_training.cfg
- Trong file yolov4_training.cfg :
  - Sửa classes = 80 thành classes = 1 tại dòng số : 970 1058 1146
  - Sửa filters = 255 thành filters = 18 tại dòng số : 1139 1051 963
- Trong file Makefile trong thư mục darknet :
  - Sửa GPU = 0 thành GPU = 1
  - Sửa OPENCV =0 thành OPENCV = 1
## 3. Chạy chương trình trên Google Colab và Flask
- Clone repository : !git clone https://github.com/khangdx1998/Equations-solver.git
- Upload folder weights và darknet lên google drive
- Chạy file demo.ipynb 

![Result 1] (result/1.png)


