# Phát hiện Viêm phổi từ Ảnh X-quang Ngực

Dự án học sâu (deep learning) dùng để phân loại **Pneumonia vs Normal** từ ảnh X-quang ngực bằng mạng nơ-ron tích chập (CNN). Repository bao gồm xử lý dữ liệu, huấn luyện mô hình, đánh giá và dự đoán.

---

## 🚀 Tính năng
- Pipeline tiền xử lý dữ liệu X-quang
- Kiến trúc CNN (tự xây hoặc dùng transfer learning)
- Script huấn luyện & kiểm định
- Đánh giá mô hình (accuracy, confusion matrix, các biểu đồ…)
- Script suy luận để dự đoán viêm phổi từ ảnh mới

---

## 📦 Cài đặt
### 1. Clone repo
```bash
git clone https://github.com/ankkun13/bao-cao-cuoi-ki-introAI.git
bao-cao-cuoi-ki-introAI
```

### 2. Tạo môi trường ảo
```bash
python -m venv venv
source venv/bin/activate   # Linux/MacOS
venv/Scripts/activate      # Windows
```

### 3. Cài đặt thư viện
```bash
pip install -r requirements.txt
```

---

## 📊 Dataset
Dataset có thể tải từ Kaggle:

[Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

Giải nén và đặt vào thư mục `data/`:
```
/data
    /train
    /val
    /test
```
Mỗi thư mục gồm 2 lớp:
```
NORMAL/
PNEUMONIA/
```

---

## 🧠 Huấn luyện mô hình

Mở [Notebook](pneumonia_detection.ipynb)

Chạy tuần tự tất cả Cell code
---

## 📈 Đánh giá mô hình

Kết quả bao gồm:
- Accuracy & loss
- Confusion matrix
- Classification report
- ROC curve

---


## ⚙️ Kiến trúc mô hình
Dự án hỗ trợ:
- DenseNet-121
- Transfer learning (MobileNetV2, ResNet50…)


---

## 📌 TODO
- Thêm Grad-CAM
- Thêm augmentation tùy chỉnh
- UI cho inference
- Công bố pretrained model

---

## 🤝 Đóng góp
Giáo viên: Hoàng Anh Đức - MIM-HUS
Cử nhân: Phạm Ngọc Hải - K66A5

---

## ❤️ Ghi nhận
- Dataset: Kaggle Chest X-Ray Pneumonia
- Pytorch
- Cảm hứng từ các nghiên cứu về medical imaging

