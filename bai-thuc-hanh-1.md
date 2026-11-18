# [Bài thực hành 1] Lập kế hoạch tài chính cá nhân bằng Chain-of-Thought
## *Prompt hoàn chỉnh*
```
Bạn là 1 chuyên gia tài chính cá nhân. Hãy lập kế hoạch tài chính hàng tháng từ dữ liệu đầu vào gồm: Thu nhập, Chi phí cố định, Các khoản nợ, Mục tiêu tiết kiệm.

Hãy suy nghĩ từng bước một và tính toán chi tiết trước khi đưa ra quyết định bằng kỹ thuật Chain-of-Thought (CoT):

Vạch ra quy trình lập luận gồm các bước:
-   Bước 1: Tính toán tổng thu nhập khả dụng sau khi trừ thuế và chi phí cố định bắt buộc.
-   Bước 2: Phân bổ khoản tiền trả nợ tối thiểu.
-   Bước 3: Trích lập quỹ tiết kiệm theo tỷ lệ cam kết.
-   Bước 4: Chia phần còn lại cho chi tiêu linh hoạt theo quy tắc 50/30/20 cải tiến.

Trình bày kết quả lập luận thành hai phần rõ rệt:
-   Phần 1: Nhật ký suy luận logic (Reasoning Steps) chỉ ra công thức tính toán và số liệu trung gian.
-   Phần 2: Bảng phân bổ ngân sách cuối cùng bằng Markdown Table với các cột: Hạng mục, Số tiền, Tỷ lệ %, Ghi chú.

Bắt buộc hiển thị đầy đủ phép tính cộng trừ nhân chia trung gian, không nhảy cóc ra kết quả.
Đảm bảo tổng tỷ lệ phần trăm phân bổ ngân sách phải bằng chính xác 100%.
```
## *Kết quả của AI*

# Kế Hoạch Tài Chính Cá Nhân Hàng Tháng

### Bộ dữ liệu đầu vào giả định
* **Tổng thu nhập (Gross):** $15.000.000\text{ VNĐ/tháng}$ (Giả định thuế TNCN & bảo hiểm bắt buộc khấu trừ $10\% = 1.500.000\text{ VNĐ}$).
* **Chi phí cố định bắt buộc:** $4.500.000\text{ VNĐ}$ (Tiền thuê trọ: $3.200.000\text{ VNĐ}$, Điện/nước/Internet: $800.000\text{ VNĐ}$, Xăng xe/gửi xe cơ bản: $500.000\text{ VNĐ}$).
* **Các khoản nợ (Trả góp/nợ cá nhân):** $1.500.000\text{ VNĐ/tháng}$.
* **Mục tiêu tiết kiệm cam kết:** $20\%$ trên tổng thu nhập khả dụng sau thuế.

---

### Phần 1: Nhật ký suy luận logic (Reasoning Steps)

* **Bước 1: Tính toán tổng thu nhập khả dụng sau khi trừ thuế và chi phí cố định bắt buộc**
  * Tính thu nhập ròng (Net Income) sau thuế và bảo hiểm:
    $$\text{Thu nhập ròng} = 15.000.000 - (15.000.000 \times 10\%) = 15.000.000 - 1.500.000 = 13.500.000\text{ VNĐ}$$
  * Tính thu nhập khả dụng sau chi phí cố định bắt buộc:
    $$\text{Thu nhập khả dụng (B1)} = 13.500.000 - 4.500.000 = 9.000.000\text{ VNĐ}$$

* **Bước 2: Phân bổ khoản tiền trả nợ tối thiểu**
  * Trừ khoản nghĩa vụ trả nợ hàng tháng từ phần thu nhập khả dụng còn lại ở Bước 1:
    $$\text{Số tiền còn lại sau nợ (B2)} = 9.000.000 - 1.500.000 = 7.500.000\text{ VNĐ}$$

* **Bước 3: Trích lập quỹ tiết kiệm theo tỷ lệ cam kết**
  * Áp dụng nguyên tắc "Trả cho mình trước" (Pay yourself first) với tỷ lệ cam kết $20\%$ trên Thu nhập ròng ($13.500.000\text{ VNĐ}$):
    $$\text{Quỹ tiết kiệm} = 13.500.000 \times 20\% = 13.500.000 \times 0,2 = 2.700.000\text{ VNĐ}$$
  * Tính ngân sách còn lại cho chi tiêu biến đổi (linh hoạt):
    $$\text{Ngân sách chi tiêu linh hoạt (B3)} = 7.500.000 - 2.700.000 = 4.800.000\text{ VNĐ}$$

* **Bước 4: Chia phần còn lại cho chi tiêu linh hoạt theo quy tắc 50/30/20 cải tiến**
  * Vì các khoản cố định (Needs cơ bản), nợ và tiết kiệm (Savings) đã được tách riêng ở trên, phần $4.800.000\text{ VNĐ}$ còn lại sẽ được chia theo tỷ lệ cải tiến $60\%$ Nhu cầu thiết yếu biến đổi : $30\%$ Mong muốn cá nhân : $10\%$ Quỹ dự phòng/Phát triển bản thân:
    * Ăn uống & Nhu yếu phẩm hàng ngày ($60\%$):
      $$4.800.000 \times 60\% = 4.800.000 \times 0,6 = 2.880.000\text{ VNĐ}$$
    * Giải trí & Mong muốn cá nhân ($30\%$):
      $$4.800.000 \times 30\% = 4.800.000 \times 0,3 = 1.440.000\text{ VNĐ}$$
    * Phát triển bản thân & Dự phòng phát sinh ($10\%$):
      $$4.800.000 \times 10\% = 4.800.000 \times 0,1 = 480.000\text{ VNĐ}$$
  * Kiểm tra lại tổng số tiền phân bổ trên Thu nhập ròng ($13.500.000\text{ VNĐ}$):
    $$4.500.000 + 1.500.000 + 2.700.000 + 2.880.000 + 1.440.000 + 480.000 = 13.500.000\text{ VNĐ}\text{ (Khớp 100\%)}$$

---

### Phần 2: Bảng phân bổ ngân sách cuối cùng
*(Tỷ lệ % được tính trên tổng Thu nhập ròng thực nhận là $13.500.000\text{ VNĐ}$)*

| Hạng mục | Số tiền (VNĐ) | Tỷ lệ % | Ghi chú |
| :--- | :---: | :---: | :--- |
| **1. Chi phí cố định bắt buộc** | 4.500.000 | 33,33% | Thuê nhà, điện nước, internet, đi lại cơ bản ($4.500.000 / 13.500.000$) |
| **2. Trả nợ tối thiểu** | 1.500.000 | 11,11% | Thanh toán nợ trả góp đúng hạn ($1.500.000 / 13.500.000$) |
| **3. Quỹ tiết kiệm cam kết** | 2.700.000 | 20,00% | Trích lập tự động ngay khi nhận lương ($2.700.000 / 13.500.000$) |
| **4. Ăn uống & Nhu yếu phẩm** | 2.880.000 | 21,33% | Chi tiêu thiết yếu linh hoạt (~96.000 VNĐ/ngày) ($2.880.000 / 13.500.000$) |
| **5. Giải trí & Cá nhân** | 1.440.000 | 10,67% | Cà phê, giao lưu bạn bè, mua sắm cá nhân ($1.440.000 / 13.500.000$) |
| **6. Phát triển & Dự phòng** | 480.000 | 3,56% | Sách, khóa học, chi phí y tế nhỏ phát sinh ($480.000 / 13.500.000$) |
| **TỔNG CỘNG** | **13.500.000** | **100,00%** | **Cân đối chính xác tuyệt đối** |