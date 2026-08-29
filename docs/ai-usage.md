# Quy tắc dùng AI — nhóm đã dùng vào việc gì, và cố ý không dùng vào việc gì

**Nhóm JCungDuoc** · **MedTriage AI** · Day 27 · 29/08/2026

Mục 9 của đề bài chia rất rõ ranh giới. Đây là bản đối chiếu trung thực của nhóm.

---

## Được dùng — và nhóm đã dùng thật

| Việc đề bài cho phép | Nhóm dùng thế nào | Kết quả |
|---|---|---|
| **Gợi ý danh sách stakeholder còn thiếu** | Sau khi ba người tự liệt kê xong ở bước cá nhân (8 + 7 + 7 = 22 mục thô), nhóm hỏi AI: *"với một sản phẩm triage AI bán cho khoa cấp cứu bệnh viện Việt Nam, nhóm vai trò nào thường bị bỏ sót?"* | AI nhắc tới **hội đồng đạo đức / quản lý chất lượng** và **nhà cung cấp HIS đương nhiệm**. Cả hai đã có sẵn trong danh sách của Linh và Hưng, nên đây là **xác nhận chứ không phải bổ sung**. Không stakeholder nào vào bản đồ chỉ vì AI nghĩ ra. |
| **Gợi ý cách viết Pitch ngắn hơn, rõ hơn** | Đưa bản nháp chung nhờ cắt phần thừa | Bản nháp đầu dài gần một trang. Đã cắt xuống **nửa trang**, bỏ một đoạn kể về kiến trúc hệ thống mà trưởng khoa không cần nghe. **Nội dung do nhóm quyết, AI chỉ cắt độ dài.** |
| **Kiểm tra RACI có thiếu A/R/C/I** | Nhờ soát 6 hàng × 6 cột | Bắt được **1 lỗi thật**: hàng T5 ở bản nháp có **hai A** (Việt và Hưng). Nhóm tự chọn giữ A cho Hưng — người sở hữu hạ tầng, chịu trách nhiệm nếu kiosk chết giữa ca — và hạ Việt xuống R. |
| **Gợi ý role / capability phổ biến trong AI team** | Hỏi danh sách vai trò thường có ở AI team giai đoạn pre-pilot | Nhận về khoảng 10 vai trò. Nhóm **giữ 3, chuyển 4 sang mục Extended cố ý chưa lập, loại phần còn lại** vì không gỡ được blocker nào của cổng gác gần nhất. Đây đúng là chỗ dễ sa vào "càng nhiều chức danh càng tốt" mà luật số 5 cấm. |
| **Gợi ý cách chuyển một vấn đề Team Health thành hành động cụ thể** | Đưa câu *"đội tự đặt ngưỡng, tự đo, tự báo cáo"* nhờ chuyển thành hành động kiểm được | Thành hành động **G-3**: review 20 phút mỗi thứ Sáu 20h, mỗi buổi đúng một người ngoài đội dự, biên bản 5 dòng đẩy lên repo. Nhóm tự thêm phần **owner, ngày cụ thể và dấu hiệu hoàn thành**. |

---

## Không được dùng — và nhóm đã không dùng

| Việc đề bài cấm | Nhóm đã làm gì để không vi phạm |
|---|---|
| **Bịa stakeholder không tồn tại trong dự án** | Mọi stakeholder trên bản đồ là **vai trò có thật** trong đường đi của sản phẩm. Nhóm **không đặt tên riêng của bất kỳ bác sĩ, điều dưỡng hay bệnh viện nào** — dùng "Bệnh viện A", "Trưởng khoa Cấp cứu", "điều dưỡng tiếp nhận". Bịa một cái tên nghe thật là cách nhanh nhất để bài đẹp lên mà sai đi. |
| **Bịa số liệu / feedback để Pitch thuyết phục hơn** | Mọi con số trong Pitch **truy ngược được** về workbook Day 25 và dashboard Day 26 (giá 6.000.000 ₫ + 13.000 ₫/ca · GM 71,8% · breakeven containment 55,1% · chi phí AI 2.307 ₫/ca · 22/22 phép kiểm tra của `verify_thresholds.py`). Chỗ chưa có số thì ghi thẳng **"chưa đo"** — containment 78% được gọi đúng tên là **ước tính**, và Pitch có hẳn một khối *"Điều nhóm CHƯA có"*. **Không có một feedback người dùng nào được trích, vì nhóm chưa có người dùng nào.** |
| **Tự quyết định RACI thay team mà không có thảo luận** | AI chỉ được dùng để **soát lỗi hình thức** (thiếu A, thừa A). Việc **ai giữ chữ A** do nhóm tự chốt theo nguyên tắc "A là người chịu hậu quả nếu việc đó hỏng", và lý do của từng hàng được viết ra ở cột ghi chú của Trang 2. |
| **Tạo AI Team "đẹp trên giấy" nhưng không phản ánh nguồn lực thật** | Nhóm có **3 người và không có tiền tuyển ai** — nên Trang 3 kết luận **không gap nào được giải bằng Hire**, và vai trò Domain Expert lâm sàng **để trống, gọi đúng tên là gap** thay vì chia nhau gánh rồi coi như đã có. Hưng đã tự phản đối chính đề nghị giao vai trò đó cho mình. |
| **Viết Growth Plan chung chung mà team không cam kết thực hiện** | Đúng 3 hành động, mỗi hành động có owner là **người đang giữ chữ A trong RACI**, có deadline theo ngày, có dấu hiệu hoàn thành **kiểm được từ bên ngoài** (file, email, lệnh chạy được). Nhóm còn thêm **điểm kiểm giữa kỳ ngày 14** với phản ứng quyết trước, và ghi ra **4 việc đã bị loại khỏi kế hoạch cùng lý do** — trong đó loại thẳng câu "team cần giao tiếp tốt hơn". |

---

## Một chỗ nhóm đã suýt vi phạm

Bản nháp đầu của Trang 1 có một stakeholder ghi là *"đối tác dữ liệu y tế đã ký MOU"*. Không có MOU nào cả —
câu đó xuất hiện vì nó làm bản đồ trông trưởng thành hơn. Linh phát hiện khi soát chéo và nhóm **xóa hẳn**,
không đổi thành "đối tác dữ liệu tiềm năng" cho đỡ tiếc, vì như vậy vẫn là giữ lại một ô trống được sơn màu.

Cách nhóm chốt để tránh lặp lại: **mỗi dòng trên bản đồ phải trả lời được câu "ai trong nhóm đã nói chuyện với
người này, ngày nào?"** — chưa ai nói chuyện thì stance ghi **Trung lập** hoặc **Chưa ủng hộ**, và đó chính là
lý do 8 trong 10 stakeholder của bài này không mang nhãn "Ủng hộ".
