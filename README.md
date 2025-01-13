# Dự án Visual Question Answering
## 1. Giới thiệu

Visual Question Answering (VQA) là một bài toán kết hợp giữa Thị giác máy tính (Computer Vision) và Xử lý ngôn ngữ tự nhiên (Natural Language Processing). Mục tiêu là phân tích hình ảnh và trả lời các câu hỏi liên quan dựa trên thông tin từ hình ảnh.  

### Input và Output:
- **Input**: Một cặp hình ảnh và câu hỏi ngôn ngữ tự nhiên.
- **Output**: Câu trả lời cho câu hỏi dựa trên hình ảnh.

Mô hình VQA sẽ xử lý qua các bước:
1. **Trích xuất đặc trưng (Feature Extraction)**: Từ dữ liệu ảnh và văn bản.
2. **Kết hợp đặc trưng (Feature Fusion)**: Tổng hợp thông tin.
3. **Sinh câu trả lời (Answer Generator)**: Dự đoán câu trả lời từ dữ liệu đầu vào.

## 2. Cài đặt chương trình

### Các mô hình được sử dụng:
1. **CNN + LSTM**: Kết hợp mạng CNN để xử lý ảnh và LSTM để xử lý câu hỏi.
2. **Transformers**: Sử dụng VisionTransformer (ViT) và RoBERTa.
3. **Vision-Language Models (VLMs)**: Áp dụng LLaVA – một mô hình ngôn ngữ thị giác lớn.

### Hướng dẫn chi tiết:
- Tải dataset và các file code gợi ý từ phần Phụ lục.
- Import các thư viện cần thiết (PyTorch, HuggingFace).
- Thực hiện huấn luyện mô hình trên tập dữ liệu VQA.
- Đánh giá độ chính xác mô hình trên tập dữ liệu kiểm tra.

## 3. Kết quả
- **Mô hình CNN + LSTM**: Kết quả đạt ~50% độ chính xác.
- **Mô hình Transformers (ViT + RoBERTa)**: Cải thiện kết quả đạt ~66% độ chính xác.
- **Mô hình VLM (LLaVA)**: Hiệu quả cao với khả năng dự đoán tốt mà không cần huấn luyện thêm.

## 4. Phụ lục
- **Dataset**: Tải từ [Dataset VQA](https://drive.google.com/drive/folders/1vXGWfqf4CSyOLRpq3IFM0rRIxNQTpRvE?usp=sharing).

---