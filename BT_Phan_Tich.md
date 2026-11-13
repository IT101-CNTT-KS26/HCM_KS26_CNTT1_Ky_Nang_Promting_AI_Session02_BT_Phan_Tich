# [Bài Tập Phân tích] So sánh Trade-off các giải pháp ra lệnh cho Cấu trúc Prompt Tiêu chuẩn & Định dạng
## 1. Đề xuất 2 prompt tương ứng với 2 phương án giải quyết.
### Viết rõ 2 prompt tương ứng với 2 phương án giải quyết.

- **Giải pháp 1:** Đơn giản, ngắn gọn

    >Hãy phân tích bình luận của khánh hàng dưới đây, xác định xảm xúc (Tích cực, Tiêu cực, hoặc Trung tính) cà trình bày kết quả thành dạng bảng.
    
    >Ví dụ: "Sản phẩm tốt lắm" -> Tiêu cực.

    >Dữ liệu cần phân tích: "Sản phẩm tệ lắm, nhân viên thái độ kém, sẽ không quay lại"

- **Giải pháp 2:** Chi tiết, có nhiều ràng buộc

    >**[Vai trò]:** Bạn là một chuyên gia phân tích dữ liệu khách hàng. 

    >**[NHiệm vụ]:** Phân tích nội dung bình luận được cung cấp , xác định rõ cảm xúc của khách hàng và lọc ra các từ khóa chính.

    >**[Ràng buộc]:** Kết quả trả về bắt buộc phải được trình bày theo đúng mẫu báo cáo dạng danh sách dưới đây, tuyệt đối không được viết thêm bất kỳ câu chữ giải thích nào ở ngoài.

    >**[Ví dụ mẫu]:** 

    >**Đầu vào:** "Áo rất đẹp nhưng giao hàng hơi chậm."

    >**Mẫu báo cáo kết quả:**

    - **Trạng thái cảm xúc:** Trung tính

    - **Các từ khóa chính:** áo đẹp, giao hàng chậm

    **[Đầu vào cần xử lý]:** "Dịch vụ quá tệ, nhân viên thái độ kém, sẽ không quay lại!"

## 2. Lập bảng so sánh Trade-off
### Lập bảng so sánh tiêu chí

| Tiêu chí | Giải pháp 1 (Đơn giản) | Giải pháp 2 (Chi tiết) |
| :--- | :--- | :--- |
| Độ dễ hiểu | **Cao:** Rất dễ viết, nhanh chóng, phù họp cho người mới bắt đầu học. | **Trung bình:** Cần làm quen với các quy tắc và mẫu trình bày rõ ràng. |
| Tốn token | **Ít:** Tiết kiệm từ ngữ và thời gian AI xử lý. | **Nhiều hơn:** Tốn thêm không gian cho ví dụ và quy tắc ràng buộc. |
| Chặn lỗi biên | **Trung bình:** AI dễ viết lan man ngoài lề hoặc vẽ bảng sai ý muốn. | **Cực tốt:** Kiểm soát chặt chẽ đầu ra, kết quả luôn đúng mẫu yêu cầu. |


## 3. Lựa chọn và chạy thử 
### Chọn phương án tối ưu nhất, giải thích lý do và chạy thử lấy kết quả.

- Lựa chọn giải pháp 2 là phương pháp tối ưu nhất.
- **Lý do:** Mặc dù câu lệnh hơi dài, nhưng nhờ có ví dụ mẫu minh họa và có các Quy tắc trình bày đầy đủ bối cảnh, nên AI sẽ không trả lơig chung chung, lan man hay thừa thãi, mà nó sẽ đưa ra kết quả gọn gàng chính xác đúng theo mẫu báo cáo mà mình mong muốn.

- **Kết quả chạy thử của Giải pháp 2:** 
    
    - **Trạng thái cảm xúc:** Tiêu cực 
    - **Các từ khóa chính:** dịch vụ tệ, nhân viên thái độ kém, không quay lại.