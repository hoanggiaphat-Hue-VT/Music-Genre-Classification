# Music-Genre-Classification
Music genre classification using audio signal processing and MLP on the GTZAN dataset.
# Music Genre Classification Using MLP

Dự án phân loại 10 thể loại âm nhạc trên bộ dữ liệu **GTZAN**, sử dụng kỹ thuật xử lý tín hiệu âm thanh và mạng nơ-ron nhân tạo **Multilayer Perceptron (MLP)**.

## Kiến trúc mô hình

Mô hình sử dụng các đặc trưng âm thanh như MFCC, Chroma, RMS, Spectral Centroid, Spectral Bandwidth và Zero Crossing Rate làm đầu vào.

| Layer | Số nơ-ron | Activation |
|---|---:|---|
| Input Layer | Số đặc trưng đầu vào | — |
| Hidden Layer 1 | 512 | ReLU + Dropout (0.2) |
| Hidden Layer 2 | 256 | ReLU + Dropout (0.2) |
| Hidden Layer 3 | 128 | ReLU + Dropout (0.2) |
| Hidden Layer 4 | 64 | ReLU + Dropout (0.2) |
| Hidden Layer 5 | 32 | ReLU + Dropout (0.2) |
| Output Layer | 10 | Softmax (Inference) |

## Cấu hình huấn luyện

- **Optimizer:** Adam
- **Learning Rate:** 0.000146
- **Batch Size:** 256
- **Epochs:** 300
- **Loss Function:** Cross-Entropy

## Công nghệ sử dụng

Python, PyTorch, Librosa, NumPy, Pandas, Scikit-learn.

## Thành viên

- Hoàng Gia Phát
- Đỗ Thanh Sơn
