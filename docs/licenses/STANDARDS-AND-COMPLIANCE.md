# ĐẶC TẢ TUÂN THỦ TIÊU CHUẨN KỸ THUẬT KHO VẬN & AN TOÀN
## (STANDARDS AND LOGISTICS COMPLIANCE)

> **Hệ thống Quản lý Kho Thông minh (Smart WMS)**  
> *Đặc tả các tiêu chuẩn kỹ thuật công nghiệp, chuẩn mã vạch quốc tế và an toàn kệ kho được tích hợp trong phần mềm.*

---

### 1. TIÊU CHUẨN ĐỊNH DANH TOÀN CẦU GS1 (GS1 GLOBAL STANDARDS)
Hệ thống Smart WMS tuân thủ cấu trúc dữ liệu và định danh theo chuẩn **GS1 General Specifications**:
- **GTIN (Global Trade Item Number)**: Hỗ trợ mã hóa và quét mã vạch sản phẩm EAN-13, EAN-8, UPC-A.
- **GLN (Global Location Number)**: Quy tắc định danh kho bãi, phân khu và vị trí ô kệ.
- **GS1-128 / Code 128**: Định dạng mã vạch công nghiệp tích hợp số lô sản xuất (Batch/Lot No), hạn sử dụng (Expiry Date) và số lượng kiện.
- **SSCC (Serial Shipping Container Code)**: Mã định danh công-ten-nơ và pallet vận chuyển trong các phiếu điều chuyển liên kho và xuất hàng.

---

### 2. TIÊU CHUẨN AN TOÀN KỆ CHỨA HÀNG CÔNG NGHIỆP
Thuật toán phân bổ vị trí `aiSlottingEngine.ts` được thiết kế dựa trên các chỉ số an toàn kết cấu kệ:
- **Tiêu chuẩn Châu Âu EN 15635:2008** (*Steel static storage systems - Application and maintenance of storage equipment*):
  - Phân bổ trọng tâm thấp: Kiện hàng nặng ($\ge 30\text{kg}$) được thuật toán chấm điểm ưu tiên tuyệt đối vào Tầng 1 và Tầng 2 để giảm thiểu mô-men uốn và chống hiện tượng sập đổ kệ liên hoàn.
  - Cảnh báo vượt tải: Hệ thống tự động chặn xếp hàng vào các ô kệ có tổng trọng lượng đạt $\ge 95\%$ tải trọng cho phép (`maxWeightCapacityKg`).
- **Tiêu chuẩn Mỹ ANSI/RMI MH16.1** (*Specification for the Design, Testing and Utilization of Industrial Steel Storage Racks*):
  - Đảm bảo khoảng hở công thái học và khoảng đệm an toàn tối thiểu 30% thể tích ô kệ ($\eta_{\text{packing}} = 70\%$) cho thao tác đưa hàng vào/lấy hàng ra của xe nâng.

---

### 3. TIÊU CHUẨN QUẢN TRỊ CHẤT LƯỢNG & AN TOÀN THÔNG TIN (ISO)
- **ISO 9001:2015 (Hệ thống Quản lý Chất lượng - Quality Management)**:
  - Chuẩn hóa toàn bộ chu trình kho: Tiếp nhận hàng $\rightarrow$ Lưu kho (Put-away) $\rightarrow$ Kiểm kê (Cycle count) $\rightarrow$ Điều chuyển (Transfer) $\rightarrow$ Xuất kho (Dispatch).
  - Tự động ghi nhận vết kiểm toán (Audit Trail) chi tiết người tạo, thời gian và sự thay đổi số dư tồn kho.
- **ISO/IEC 27001:2022 (Hệ thống Quản lý An toàn Thông tin - Information Security)**:
  - Cơ chế phân quyền chặt chẽ RBAC (Role-Based Access Control) cho Ban quản lý kho, Thủ kho và Nhân viên bốc xếp.
  - Cơ chế xác thực mã hóa token JWT và băm mật khẩu bảo mật `bcrypt`.
