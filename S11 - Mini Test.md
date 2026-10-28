**BÀI KIỂM TRA** 

# **BỐI CẢNH CHUNG**

Công ty ABC có 300 nhân viên văn phòng. Mỗi sáng, nhân viên phải xuống sảnh ghi tên vào sổ đặt cơm trưa trước 9h30 và chọn 1 trong 4 suất ăn do nhà bếp nấu. Bộ phận hành chính đếm sổ, gọi điện báo số lượng cho nhà bếp, cuối tháng cộng tiền và trừ vào lương.

Những vấn đề đang gặp:

* Nhân viên đi công tác hoặc làm từ xa không đặt được suất ăn.

* Sổ giấy hay bị ghi nhầm tên và nhầm món.

* Hành chính mất khoảng 45 phút mỗi sáng chỉ để tổng hợp số liệu.

* Nhà bếp không biết trước tỷ lệ chọn từng món nên thường xuyên nấu thừa hoặc thiếu.

* Nhân viên không tự tra được trong tháng mình đã đặt bao nhiêu bữa và hết bao nhiêu tiền.

Công ty quyết định xây dựng ứng dụng SmartCanteen để giải quyết các vấn đề trên. Bạn là thành viên của Scrum Team nhận dự án này.

# **BÀI 1 – PHÂN RÃ YÊU CẦU**

**Cho Epic: "Đặt và quản lý suất ăn của nhân viên".**

**a)**Viết 2 Feature thuộc Epic trên.

| Feature 1: Đặt suất ăn hàng ngày Cho phép nhân viên (kể cả khi đang đi công tác hoặc làm từ xa) xem thực đơn, chọn 1 trong 4 suất ăn của nhà bếp trước 9h30 sáng, và hệ thống tự động lưu lại lịch sử đặt món cá nhân để tra cứu chi phí. Feature 2: Quản lý và tổng hợp suất ăn tự động  Tự động tổng hợp số liệu đặt cơm vào lúc 9h30 sáng để gửi báo cáo chính xác cho nhà bếp (tránh nấu thừa/thiếu) và tự động tính toán, trừ tiền vào lương nhân viên vào cuối tháng, thay thế hoàn toàn sổ giấy thủ công. |
| :---- |

**b)**Viết 2 User Story theo đúng cấu trúc "Là… tôi muốn… để…", mỗi story thuộc một Feature khác nhau ở câu a.

| Là nhân viên làm việc từ xa hoặc đi công tác, tôi muốn truy cập vào ứng dụng di động/web để chọn suất ăn trước 9h30 sáng để tôi vẫn có thể đặt được bữa trưa mà không cần phải xuống sảnh ký tên vào sổ giấy, theo dõi được số bữa đã đặt và tổng chi phí trong tháng. Là nhân viên bộ phận hành chính, tôi muốn hệ thống tự động tổng hợp và thống kê toàn bộ số lượng các món ăn đã được nhân viên đặt trước 9h30, để tôi không phải mất 45 phút mỗi sáng để tổng hợp sổ thủ công, hạn chế tối đa việc nhầm tên/nhầm món và gửi thông tin chính xác ngay lập tức cho nhà bếp. |
| :---- |

**c)**Nêu 1 hạng mục công việc thuộc Epic này nhưng là Task kỹ thuật chứ không phải User Story, và giải thích ngắn gọn vì sao.

| Thiết kế cơ sở dữ liệu lưu thông tin nhân viên, thực đơn và lịch sử đặt suất ăn. Giải thích: Đây là công việc kỹ thuật phục vụ phát triển hệ thống, không mô tả nhu cầu và giá trị trực tiếp của người dùng |
| :---- |

# **BÀI 2 – CHẨN ĐOÁN VÀ VIẾT LẠI USER STORY** 

Hai User Story dưới đây do một thành viên mới viết. Với mỗi story: chỉ ra tiêu chí INVEST bị vi phạm rõ nhất, giải thích trong 1 câu, rồi viết lại cho đạt chuẩn.

**Story A:**

*"Là người dùng, tôi muốn ứng dụng chạy nhanh và dễ dùng để tôi cảm thấy hài lòng."*

| Vi phạm: Testable Lý do: mục đích chưa rõ ràng, không có tiêu chí đo lường cụ thể Viết lại: Là người dùng, tôi muốn trang thực đơn tải trong vòng 2 giây để nhanh chóng chọn suất ăn  |
| :---- |

**Story B:**

*"Là nhân viên, tôi muốn có đầy đủ tính năng quản lý bữa trưa gồm đặt suất, hủy suất, đổi món, xem lịch sử, xem công nợ tháng, xuất báo cáo và đánh giá món ăn, để tôi chủ động với bữa trưa của mình."*

| Vi phạm: Small Lý do: gộp quá nhiều chức năng, khó hoàn thành trong 1 Sprint Viết lại: Là nhân viên, tôi muốn xem lịch sử đặt suất ăn và tổng chi phí trong tháng để chủ động theo dõi tiền ăn của mình  |
| :---- |

# **BÀI 3 – VIẾT ACCEPTANCE CRITERIA** 

Cho User Story sau:

*"Là nhân viên, tôi muốn hủy suất cơm đã đặt trước 9h30 của ngày ăn, để tôi không bị tính tiền bữa mình không ăn."*

Viết 3 Acceptance Criteria theo cấu trúc Given – When – Then vào bảng dưới. Yêu cầu: AC-01 cho luồng thành công, AC-02 cho trường hợp quá giờ hủy, AC-03 do bạn tự chọn (một trường hợp ngoại lệ khác). Mỗi tiêu chí đúng được 1,0 điểm.

| Mã | Nội dung tiêu chí |
| :---: | ----- |
| **AC-01** | **Given:** Nhân viên đặt suất ăn và chưa đên 9h30 **When:** Nhân viên chọn huỷ suất ăn **Then:** Hệ thống huỷ suất ăn và không tính tiền bữa đó  |
| **AC-02** | **Given** Nhân viên đặt suất ăn và đã quá 9h30 **When** Nhân viên yêu cầu huỷ **Then** Hệ thống từ chối huỷ và giữ nguyên đơn đặt  |
| **AC-03** | **Given** Nhân viên chưa đặt suất ăn ngày đó **When** Nhân viên chọn huỷ suất ăn **Then** Hệ thống báo không có suất ăn để huỷ  |

# **BÀI 4 – ƯU TIÊN VÀ LẬP KẾ HOẠCH SPRINT**

Product Backlog của dự án SmartCanteen đã được ước lượng như sau. Velocity của nhóm trong 3 Sprint gần nhất lần lượt là 18, 22 và 20 Story Point. Sprint kế tiếp kéo dài 2 tuần, nhân sự không thay đổi.

**a) Điền mức ưu tiên MoSCoW cho từng hạng mục, sau đó giải trình lựa chọn cho 2 hạng mục bất kỳ.**

| Mã | Hạng mục | Story Point | MoSCoW |
| :---: | ----- | :---: | :---: |
| SC-01 | Nhân viên đặt suất ăn cho ngày hôm sau | 5 | Must |
| SC-02 | Nhân viên hủy suất ăn trước giờ chốt | 3 | Must |
| SC-03 | Hành chính xem báo cáo tổng hợp số suất theo món mỗi ngày | 8 | Must |
| SC-04 | Nhân viên xem lịch sử đặt và số tiền phải trả trong tháng | 5 | Should |
| SC-05 | Nhân viên đánh giá món ăn sau bữa trưa | 3 | Could |
| SC-06 | Đăng nhập bằng tài khoản nội bộ của công ty | 8 | Must |
| SC-07 | Chia sẻ thực đơn tuần lên fanpage công ty | 2 | Won’t |

Giải trình:

| SC-01 – Must: Là chức năng chính giúp nhân viên đặt cơm trực tuyến, thay thế sổ giấy SC-03 – Must: Giúp hành chính tổng hợp số lượng chính xác, hỗ trợ nhà bếp chuẩn bị món ăn phù hợp |
| :---- |

**b)Chọn các hạng mục đưa vào Sprint kế tiếp, ghi rõ tổng Story Point và căn cứ lựa chọn.**

|   |
| :---- |

**c)Viết Sprint Goal cho Sprint đó.**

| Xây dựng chức năng đăng nhập và đặt suất ăn trực tuyến, cho phép nhân viên hủy suất đúng hạn và theo dõi lịch sử, chi phí ăn hàng tháng  |
| :---- |

**d)Đến hết ngày làm việc thứ 5 của Sprint, số Story Point còn lại được ghi nhận như sau:**

| Ngày làm việc | 0 | 1 | 2 | 3 | 4 | 5 |
| ----- | :---: | :---: | :---: | :---: | :---: | :---: |
| Đường lý tưởng | 20 | 18 | 16 | 14 | 12 | 10 |
| Đường thực tế | 20 | 20 | 19 | 18 | 16 | 15 |

Nhận xét tình hình Sprint và đề xuất 1 hành động cụ thể cho nhóm:

| Nhận xét: Nhóm đang chậm tiến độ 5 SP so với kế hoạch, tốc độ hoàn thành thấp hơn dự kiến Đề xuất: Ưu tiên xử lý công việc đang tắc nghẽn, đưa công việc về đúng tiến độ của kế hoạch |
| :---- |

