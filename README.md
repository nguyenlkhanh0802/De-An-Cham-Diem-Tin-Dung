# Đề án 01: Chấm điểm Tín dụng có Giải thích (Credit Scoring)

## 📌 1. Giới thiệu Dự án
Dự án nhằm xây dựng mô hình học máy chấm điểm tín dụng và dự báo rủi ro vỡ nợ của khách hàng dựa trên bộ dữ liệu **UCI Default of Credit Card Clients** (30,000 quan sát).

---

## 📊 2. Data Dictionary (Từ điển dữ liệu)

| Tên biến | Kiểu dữ liệu | Ý nghĩa / Mô tả |
| :--- | :--- | :--- |
| `LIMIT_BAL` | Numeric | Hạn mức tín dụng được cấp (Đơn vị: NT dollar) |
| `SEX` | Categorical | Giới tính (1 = Nam, 2 = Nữ) |
| `EDUCATION` | Categorical | Trình độ học vấn (1 = Cao học, 2 = Đại học, 3 = Trung học, 4 = Khác) |
| `MARRIAGE` | Categorical | Tình trạng hôn nhân (1 = Đã kết hôn, 2 = Độc thân, 3 = Khác) |
| `AGE` | Numeric | Tuổi của khách hàng (Năm) |
| `PAY_0` | Numeric | Trạng thái thanh toán tháng 9 (-1=Trả đúng hạn, 1=Chậm 1 tháng, 2=Chậm 2 tháng,...) |
| `PAY_2` | Numeric | Trạng thái thanh toán tháng 8 |
| `PAY_3` | Numeric | Trạng thái thanh toán tháng 7 |
| `PAY_4` | Numeric | Trạng thái thanh toán tháng 6 |
| `PAY_5` | Numeric | Trạng thái thanh toán tháng 5 |
| `PAY_6` | Numeric | Trạng thái thanh toán tháng 4 |
| `BILL_AMT1` | Numeric | Số tiền trên hóa đơn tháng 9 (NT dollar) |
| `BILL_AMT2` | Numeric | Số tiền trên hóa đơn tháng 8 |
| `BILL_AMT3` | Numeric | Số tiền trên hóa đơn tháng 7 |
| `BILL_AMT4` | Numeric | Số tiền trên hóa đơn tháng 6 |
| `BILL_AMT5` | Numeric | Số tiền trên hóa đơn tháng 5 |
| `BILL_AMT6` | Numeric | Số tiền trên hóa đơn tháng 4 |
| `PAY_AMT1` | Numeric | Số tiền đã thanh toán trong tháng 9 (NT dollar) |
| `PAY_AMT2` | Numeric | Số tiền đã thanh toán trong tháng 8 |
| `PAY_AMT3` | Numeric | Số tiền đã thanh toán trong tháng 7 |
| `PAY_AMT4` | Numeric | Số tiền đã thanh toán trong tháng 6 |
| `PAY_AMT5` | Numeric | Số tiền đã thanh toán trong tháng 5 |
| `PAY_AMT6` | Numeric | Số tiền đã thanh toán trong tháng 4 |
| `default` | Binary | **Biến mục tiêu**: Vỡ nợ vào tháng tiếp theo (1 = Có, 0 = Không) |

---

## 🛠️ 3. Hướng dẫn Tái lập Môi trường (Reproduce Environment)

1. **Cloning Repository:**
   ```bash
   git clone [https://github.com/nguyenlkhanh0802/De-An-Cham-Diem-Tin-Dung.git](https://github.com/nguyenlkhanh0802/De-An-Cham-Diem-Tin-Dung.git)
   cd De-An-Cham-Diem-Tin-Dung