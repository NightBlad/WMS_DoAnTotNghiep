# ĐIỀU KHOẢN DỊCH VỤ TRÍ TUỆ NHÂN TẠO & ĐÁM MÂY
## (AI PLATFORM & CLOUD SERVICE TERMS)

> **Hệ thống Quản lý Kho Thông minh (Smart WMS)**  
> *Quy định về việc sử dụng các dịch vụ AI bên thứ ba, an toàn dữ liệu và thỏa thuận mức dịch vụ điện toán đám mây.*

---

### 1. DỊCH VỤ GOOGLE CLOUD VERTEX AI & GEMINI API
- **Mô hình nền tảng**:
  - `gemini-2.5-flash`: Sử dụng cho nút phân loại câu hỏi (Question Classifier) và sinh câu lệnh SQL (SQL Generator).
  - `gemini-2.5-flash-lite`: Sử dụng cho nút giải thích SOP và gợi ý câu hỏi tiếp theo.
  - `gemini-embedding-2-preview`: Sử dụng cho mã hóa vector cơ sở tri thức kho vận phục vụ RAG.
- **Thỏa thuận pháp lý**:
  - Tuân thủ **Google Cloud Platform Terms of Service** và **Gemini API Additional Terms of Service**.
  - **Chính sách Zero Data Retention**: Dữ liệu truy vấn kho hàng của doanh nghiệp truyền qua API được bảo mật độc lập, **tuyệt đối không được Google lưu trữ hoặc sử dụng để huấn luyện (train/fine-tune)** các mô hình ngôn ngữ công cộng.

---

### 2. DỊCH VỤ CƠ SỞ DỮ LIỆU ĐÁM MÂY DOANH NGHIỆP (ENTERPRISE MANAGED CLOUD DATABASE)
- **Thỏa thuận mức dịch vụ (SLA)**: Cam kết tính khả dụng hạ tầng dịch vụ đạt **99.99%**.
- **Tiêu chuẩn an toàn**: Đạt các chứng chỉ độc lập tiêu chuẩn quốc tế **SOC 2 Type II**, **ISO 27001**, **PCI-DSS**.
- **Bảo mật kết nối**:
  - Toàn bộ kết nối từ AI Service Adapter và Backend API tới cơ sở dữ liệu đều được mã hóa bằng giao thức an toàn TLS 1.3 / SSL.
  - Sử dụng tài khoản phân quyền chỉ đọc độc lập (Dedicated Read-Only Service Account) cho các tác vụ phân tích và tra cứu ngôn ngữ tự nhiên, ngăn chặn tuyệt đối 100% mọi rủi ro chỉnh sửa, xóa bỏ hoặc biến dạng dữ liệu gốc.
