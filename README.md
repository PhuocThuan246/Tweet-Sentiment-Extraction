# Tweet-Sentiment-Extraction
Dự án triển khai mô hình **trích xuất cảm xúc trong tweet** (Tweet Sentiment Extraction – Kaggle).  
Khác với phân loại cảm xúc, bài toán này yêu cầu mô hình **xác định chính xác đoạn văn bản con** thể hiện cảm xúc.

Bài toán được mô hình hoá theo dạng **Question Answering (QA)**:  
- **Câu hỏi:** sentiment (positive / negative / neutral)  
- **Ngữ cảnh:** nội dung tweet  
- **Câu trả lời:** selected_text  

Pipeline gồm:  
✔ Preprocessing nhẹ  
✔ Char-to-token span mapping  
✔ Huấn luyện RoBERTa  
✔ Ensemble logits  
✔ Reranking spans  
✔ Post-processing  

Kết quả cuối đạt **Public Score: 0.71830**, tương đương **Top ~80** và sát **Top 50** leaderboard.

---


