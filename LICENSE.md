# 📜 Smart WMS – Giấy Phép Bản Quyền & Tuân Thủ Chuẩn Quốc Tế
### (Licensing & International Compliance Directory)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Workflow: Apache 2.0](https://img.shields.io/badge/Workflow_Engine-Apache_2.0-orange.svg?style=for-the-badge)](docs/licenses/LICENSE-APACHE-2.0.md)
[![AI Privacy: Zero Retention](https://img.shields.io/badge/AI_Privacy-Zero_Data_Retention-brightgreen.svg?style=for-the-badge)](docs/licenses/LICENSE-AI-SERVICES.md)
[![Standards: GS1 & EN 15635](https://img.shields.io/badge/Standards-GS1_|_EN_15635-purple.svg?style=for-the-badge)](docs/licenses/STANDARDS-AND-COMPLIANCE.md)

---

Dự án **Smart WMS (Hệ thống Quản lý Kho Thông minh)** áp dụng mô hình phân tách giấy phép minh bạch (**Multi-license Architecture**), đảm bảo mã nguồn mở hoàn toàn tự do cho cộng đồng phát triển, đồng thời đáp ứng các tiêu chuẩn khắt khe nhất về an toàn dữ liệu doanh nghiệp và kỹ thuật kho bãi quốc tế.

## ⚖️ Bảng Ma Trận Quyền Hạn & Giới Hạn Giấy Phép (MIT License)

| Quyền hạn được phép (Permissions) | Điều kiện áp dụng (Conditions) | Giới hạn trách nhiệm (Limitations) |
| :--- | :--- | :--- |
| ✅ **Sử dụng thương mại** (Commercial use) | ℹ️ **Bảo lưu thông báo bản quyền** (License & copyright notice) | ❌ **Không chịu trách nhiệm pháp lý** (Liability) |
| ✅ **Tùy biến & Sửa đổi** (Modification) | | ❌ **Không bảo hành mặc định** (Warranty) |
| ✅ **Phân phối lại** (Distribution) | | |
| ✅ **Sử dụng nội bộ/cá nhân** (Private use) | | |
| ✅ **Cấp phép thứ cấp** (Sublicense) | | |

---

## 📑 Danh Mục Giấy Phép & Tài Liệu Kỹ Thuật Đính Kèm

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                              SMART WMS COMPLIANCE STACK                                │
├────────────────────────────────────────────────────────────────────────────────────────┤
│  [MÃ NGUỒN CỐT LÕI]    ──► docs/licenses/LICENSE-MIT.md (Frontend, Backend & AI Engine)│
│  [AGENTIC WORKFLOW]    ──► docs/licenses/LICENSE-APACHE-2.0.md (Dify WMS.yml & Plugins)│
│  [DỊCH VỤ ĐÁM MÂY AI]  ──► docs/licenses/LICENSE-AI-SERVICES.md (Gemini Zero Retention) │
│  [TIÊU CHUẨN KHO VẬN]  ──► docs/licenses/STANDARDS-AND-COMPLIANCE.md (GS1, EN 15635)  │
│  [BẢN GỐC GITHUB]      ──► LICENSE (Canonical MIT License File)                        │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

### 1. 🌐 [Giấy phép MIT License](docs/licenses/LICENSE-MIT.md) (`docs/licenses/LICENSE-MIT.md`)
- **Phạm vi áp dụng**:
  - Giao diện người dùng Web: React 18, Vite, TypeScript, Tailwind CSS, Lucide React icons.
  - Hệ thống API Backend: NestJS 10, Node.js, TypeORM, class-validator.
  - Thuật toán cốt lõi: **AI Slotting Engine** (`apps/frontend/src/features/warehouses/utils/aiSlottingEngine.ts`) với 3D Bin Packing và ma trận chấm điểm 6 tiêu chí.
- **Tệp giấy phép chuẩn**: Xem bản đầy đủ tại [LICENSE](LICENSE).

### 2. ⚙️ [Giấy phép Apache License 2.0](docs/licenses/LICENSE-APACHE-2.0.md) (`docs/licenses/LICENSE-APACHE-2.0.md`)
- **Phạm vi áp dụng**:
  - Cấu hình đồ thị Agentic Workflow đa tác tử Dify tại [`WMS.yml`](WMS.yml).
  - Plugin chuyển đổi ngôn ngữ tự nhiên thành truy vấn cơ sở dữ liệu (`rookie_text2data:1.0.3`).
  - Giao diện nhúng Dify Web Chatbot (`apps/frontend/src/shared/components/DifyChatbot.tsx`).

### 3. 🛡️ [Điều khoản Dịch vụ Trí tuệ Nhân tạo & Bảo mật Đám mây](docs/licenses/LICENSE-AI-SERVICES.md) (`docs/licenses/LICENSE-AI-SERVICES.md`)
- **Phạm vi áp dụng**:
  - Mô hình Google Gemini 2.5 Flash, Gemini 2.5 Flash-Lite và Gemini Embedding 2.
  - **Cam kết Zero Data Retention**: Dữ liệu vận hành kho hàng không bao giờ bị Google lưu trữ hoặc dùng để huấn luyện mô hình công cộng.
  - Thỏa thuận dịch vụ SLA 99.99% và kết nối CSDL phân quyền chỉ đọc an toàn (Read-Only Least Privilege).

### 4. 📦 [Đặc tả Tuân thủ Tiêu chuẩn Kho vận & Kỹ thuật Quốc tế](docs/licenses/STANDARDS-AND-COMPLIANCE.md) (`docs/licenses/STANDARDS-AND-COMPLIANCE.md`)
- **Phạm vi áp dụng**:
  - **GS1 Global Identification**: GTIN-13/14, GLN vị trí ô kệ, GS1-128 và SSCC kiện pallet.
  - **An toàn Kệ Kho**: Tiêu chuẩn Châu Âu EN 15635:2008 & Hoa Kỳ ANSI/RMI MH16.1.
  - **Quản lý & Bảo mật**: Vết kiểm toán ISO 9001:2015 và an toàn thông tin ISO/IEC 27001:2022.

---

*Mọi thắc mắc về cấp phép doanh nghiệp, tích hợp OEM hoặc quyền sở hữu trí tuệ, vui lòng mở Issue trên GitHub hoặc liên hệ Ban Phát triển Dự án Smart WMS.*
