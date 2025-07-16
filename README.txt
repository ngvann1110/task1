==================================================
     DỰ ÁN PHÂN LOẠI ẢNH BẰNG VISION TRANSFORMER
==================================================

📌 Mô tả:
Dự án sử dụng mô hình học sâu Vision Transformer (ViT)
để phân loại ảnh. Mô hình được huấn luyện bằng thư viện
Transformers của Hugging Face, và có khả năng dự đoán
ảnh mới do người dùng cung cấp.

==================================================
📂 Cấu trúc thư mục `task1/`:

task1/
├── classify.ipynb         # Notebook chính: huấn luyện, đánh giá, dự đoán
├── confusion_matrix.png   # Hình confusion matrix (đã lưu từ notebook)
├── test1.jpg              # Ảnh đầu vào từ người dùng
├── test2.jpg
├── test3.jpg
├── results/               ├── .venv/                 # Thư mục môi trường ảo Python

==================================================
▶️ Cách chạy notebook:

1. Mở `classify.ipynb` bằng Jupyter Notebook hoặc VSCode.
2. Chạy từng bước:
   - Tiền xử lý dữ liệu
   - Khởi tạo và huấn luyện mô hình ViT
   - Đánh giá mô hình (accuracy, F1, loss)
   - Hiển thị confusion matrix
   - Dự đoán ảnh mới do người dùng cung cấp

3. Kết quả in ra màn hình và có thể lưu thành hình ảnh.

==================================================
🖼️ Dự đoán ảnh người dùng:

- Các ảnh `test1.jpg`, `test2.jpg`, `test3.jpg` là ví dụ ảnh ngoài dữ liệu.
- Trong notebook, cập nhật `image_path = "test1.jpg"` hoặc ảnh tương ứng.
- Mô hình sẽ in ra nhãn được dự đoán.

==================================================
📊 Kết quả đạt được:

- Accuracy: khoảng 97.2%
- F1-score: khoảng 97.1%
- Eval loss: khoảng 0.14
- Mô hình phân loại tốt ảnh chưa từng thấy trong quá trình huấn luyện.

==================================================
🚧 Hạn chế:

- Hiện chưa có giao diện kéo-thả ảnh (GUI)
- Việc vẽ confusion matrix với tập lớn còn chậm
- Chưa áp dụng kỹ thuật tăng cường dữ liệu (augmentation)

==================================================
📌 Yêu cầu môi trường:

- Python >= 3.8
- transformers
- datasets
- scikit-learn
- matplotlib
- Pillow (PIL)
- torch (PyTorch)

👉 Cài đặt nhanh (nếu dùng môi trường ảo):
    pip install -r requirements.txt

==================================================
📄 Tác giả: [Nguyễn Vân]

