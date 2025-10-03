# 🏨 Hotel Booking System – Lab 2 (NMCNPM)

**Sinh viên:** Lâm Thụy Khương — **MSSV:** N23DCCN169  
**Trường:** Học viện Công nghệ Bưu chính Viễn thông (PTIT)

## 📖 Giới thiệu
Mini‑project mô phỏng quy trình đặt phòng khách sạn: tìm phòng → đặt phòng online → thanh toán → check‑in/check‑out → quản lý phòng & buồng phòng.  
Artefact được lưu bằng **GitHub**; nộp **ảnh PNG** của các sơ đồ.

## ⚙️ Chức năng theo vai trò
- **Guest:** tìm & xem chi tiết phòng, đặt phòng online, thanh toán online.  
- **Receptionist:** quản lý đặt phòng, **check‑in/check‑out**.  
- **Manager:** quản lý phòng & giá, **báo cáo doanh thu**.  
- **Housekeeping:** nhận **công việc dọn phòng** sau check‑out.  
- **Payment Gateway:** xử lý giao dịch thanh toán.

## 🖼️ Artefact nộp (chỉ PNG) – thư mục `docs/`
- **Use Case Diagram:** `docs/usecase_diagram.png`
- **Sequence – Đặt phòng (Booking) _<<include>> Thanh toán online_:** `docs/sequence_booking_includes_payment.png`
- **Sequence – Check‑in / Check‑out:** `docs/sequence_checkin_checkout_uc.png`
- **(Tuỳ chọn) Sequence – Thanh toán online:** `docs/sequence_online_payment.png`
- **ERD (6 bảng):** `docs/ERD_booking_system.png`

## 🗃️ Tóm tắt mô hình dữ liệu (ERD)
Bảng chính: **Guest, Staff, RoomType, Room, Reservation, Payment**  
Quan hệ: `Guest 1–n Reservation`, `RoomType 1–n Room`, `Room 1–n Reservation`, `Reservation 0–n Payment`, `Staff 0–n Reservation`.  
Trường nổi bật: `ReservationCode` (mã đặt phòng), `Status` (trạng thái), `TxnId` (mã giao dịch).

## 🛠️ Công cụ
PlantUML/Draw.io (UML) • Dbdiagram (ERD) • GitHub (lưu artefact).
