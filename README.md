# edabk-ic-design-dataset

Dataset benchmark cho thiết kế mạch số (Digital IC Design)

## 1. Tổng quan về Benchmark

Benchmark được chia thành 4 cấp độ từ cơ bản đến nâng cao:

### Level 1: Lý thuyết cơ bản
- Định nghĩa và khái niệm cơ bản
  + Hệ thống số (nhị phân, thập phân, thập lục phân)
  + Đại số Boole và các phép toán logic
  + Cổng logic cơ bản (AND, OR, NOT, NAND, NOR, XOR)
  + Bảng chân trị và biểu thức logic
  + Minterm và Maxterm
  + Bản đồ Karnaugh (K-map)
  + Mạch tổ hợp và mạch tuần tự
  + Flip-flop và các loại bộ nhớ
  + Mã hóa và giải mã
  + Multiplexer và Demultiplexer
  + Bộ cộng và bộ trừ
  + Bộ so sánh
  + Bộ đếm và bộ chia tần
  + Các phương pháp tối ưu hóa mạch
  + Các tiêu chuẩn thiết kế và verify mạch
  + Các công nghệ chế tạo IC (CMOS, TTL, ECL)
  + Các thông số kỹ thuật quan trọng (tốc độ, công suất, nhiễu)
  + Các phương pháp test và debug mạch
  + Các công cụ thiết kế và mô phỏng
- Các bước thiết kế mạch số
- Quy trình tối ưu mạch
- Phương pháp verify mạch

### Level 2: Tính toán cơ bản
- Chuyển đổi số nhị phân sang thập phân
- Phép toán với số nhị phân
- Các phép tính logic cơ bản

### Level 3: Tối thiểu hóa và chứng minh
- Tối thiểu hóa hàm logic
- Chứng minh công thức
- Áp dụng lý thuyết vào bài toán thực tế

### Level 4: Triển khai mạch
- Chuyển đổi công thức thành mạch
- Thiết kế mạch từ đặc tả
- Tối ưu hóa cấu trúc mạch


## 2. Quy mô Dataset

### Số lượng và phân loại dữ liệu

Dataset được chia thành 3 nhóm chính tương ứng với 3 level đầu tiên:

| Level | Tên | Số lượng | Mô tả |
|-------|-----|----------|-------|
| 1 | Lý thuyết cơ bản | 436 | Các câu hỏi lý thuyết tổng hợp, bao phủ toàn bộ các chủ đề trọng tâm của điện tử số |
| 2 | Tính toán cơ bản | 4090 | Chủ yếu là các bài toán chuyển đổi hệ số, phép toán nhị phân, số bù, số dấu, ... |
| 3 | Tối thiểu hóa hàm/Karnaugh Map | 7200 | Các bài toán tối thiểu hóa hàm logic với K-map 3, 4, 5, 6 biến |

#### Thống kê chi tiết:
- **Level 1:** 436 câu hỏi lý thuyết (được crawl và kiểm tra thủ công)
- **Level 2:** 4090 bài toán, trong đó:
  - 3072 bài chuyển đổi hệ số (75%)
  - 100 bài toán nhị phân (2%)
  - 312 bài số dấu (8%)
  - 297 bài số bù 1 (7%)
  - 309 bài số bù 2 (8%)
- **Level 3:** 7200 bài toán K-map, gồm:
  - 3500 K-map 3 biến (49%)
  - 3500 K-map 4 biến (49%)
  - 100 K-map 5 biến (1%)
  - 100 K-map 6 biến (1%)

#### Phương pháp xây dựng dữ liệu
- Level 1: Crawl dữ liệu + kiểm tra thủ công
- Level 2: Tool + bài tập thực tế
- Level 3: Tool sinh tự động

#### Thống kê token
- Level 1: 21,695
- Level 2: 1,204,064
- Level 3: 3,192,868

### Hình ảnh minh họa dataset

![*Biểu đồ tổng số lượng dữ liệu từng nhóm*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/total.jpg)


![*Phân bố các dạng bài toán ở Level 2*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/level2-data.jpg)


![*Phân bố các dạng bài toán ở Level 3*](https://github.com/duonggiang156/banchmark-edabk/blob/master/images/level3-data.jpg)



## 3. Hướng dẫn sử dụng

### Môi trường cài đặt
- Python >= 3.x
- Các thư viện cần thiết: `pandas`, `numpy`, `...`

### Quy trình sử dụng benchmark

```
Bước 1: Clone repository
    |
Bước 2: Cài đặt dependencies
    |
Bước 3: Chạy benchmark với dataset tương ứng
    |
Bước 4: Đánh giá kết quả theo metrics
```

### Các bước chi tiết

1. **Clone repository**
   ```bash
   git clone <link-repo>
   cd <tên-thư-mục-repo>
   ```

2. **Cài đặt dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Chạy benchmark**
   - Thực hiện theo hướng dẫn trong thư mục `src/` hoặc theo từng notebook/script cụ thể.

4. **Đánh giá kết quả**
   - Sử dụng các metrics:
     - Độ chính xác (Accuracy)
     - Thời gian xử lý
     - Độ phức tạp của giải pháp


