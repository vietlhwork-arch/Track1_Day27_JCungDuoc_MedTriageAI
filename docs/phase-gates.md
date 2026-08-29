# Phase 5 — Tự soi lỗi & đối chiếu 6 gate

**Nhóm JCungDuoc** · **MedTriage AI** · 29/08/2026
Người đọc checklist: **Hưng** · Người kiểm consistency: **Linh** · Người kiểm repo & export: **Việt**

---

## GATE 0 — Scope đã rõ

> *Qua gate khi cả team đang nói về cùng một dự án, cùng một mục tiêu hiện tại và có một người tổng hợp bài.*

| Ô kiểm | Kết quả |
|---|---|
| Team có 3–5 thành viên, ghi đủ họ tên | ✅ 3 người, đủ họ tên + MHV ở README và ở header cả 4 trang PDF |
| Cùng một dự án | ✅ MedTriage AI — dự án nhóm đã build từ Day 24 đến Day 26, không tạo case mới |
| Cùng một mục tiêu hiện tại | ✅ Qua cổng gác ngày 30 (27/09/2026): containment ≥70% trên ≥800 ca hoàn tất thật |
| Có một người tổng hợp | ✅ Lê Hoàng Việt — tạo repo ở phút thứ 5 của Lab và dùng xuyên suốt |
| Format làm bài đã chốt | ✅ Markdown + HTML → PDF, tổng hợp trên repo |

**→ QUA GATE 0.**

---

## GATE 1 — Stakeholder Map có thể hành động

> *Qua gate khi: có ít nhất 6 stakeholder cụ thể, đã map theo Influence × Interest, có stance rõ ràng và có 4 hành động cụ thể cho 4 stakeholder ưu tiên.*

| Ô kiểm | Yêu cầu | Bài này |
|---|---|---|
| Số stakeholder cụ thể | ≥ 6 | ✅ **10** (S1–S10), mỗi người ghi rõ vai trò thật, không có mục nào chỉ ghi "khách hàng" hay "người dùng" |
| Map theo Influence × Interest | Bắt buộc | ✅ Ma trận 2×2 đầy đủ, cả 4 vùng đều có người |
| Dùng đúng nhãn Champion / Blocker / Supporter / Bystander | Bắt buộc | ✅ Đủ 4 nhãn: 2 Champion · 4 Blocker · 3 Supporter · 1 Bystander |
| Stance riêng cho từng stakeholder | Bắt buộc | ✅ **2** Ủng hộ (S5, S6) · **5** Trung lập (S1, S7, S8, S9, S10) · **3** Chưa ủng hộ (S2, S3, S4) |
| **Kiểm stance thực tế, không mặc định theo quadrant** | Bắt buộc | ✅ Nêu rõ **2 chỗ lệch** — S1 (ô Champion nhưng stance Trung lập) và S3 (ô Supporter nhưng stance Chưa ủng hộ), kèm lý do |
| 2 stakeholder ủng hộ mạnh để tận dụng | 2 | ✅ S5 (mentor) · S6 (cố vấn tài chính) |
| 2 stakeholder ưu tiên thuyết phục | 2 | ✅ S1 (trưởng khoa) · S3 (điều dưỡng tiếp nhận) |
| 4 hành động cụ thể, không chung chung | Bắt buộc | ✅ Cả 4 đều có **owner + deadline có ngày** (01/09 · 08/09 · 03/09–12/09 · 12/09), và đều nói rõ **gửi gì / xin gì** |

**Tự bắt lỗi của chính nhóm:** bản nháp đầu của chiến lược S5 viết *"giữ liên hệ tốt với mentor"* — đúng câu
đề bài lấy làm ví dụ phản diện. Đã sửa thành: gửi bản đề nghị 1 trang + dashboard Day 26, xin 20 phút review,
xin giới thiệu 1 khoa cấp cứu, hạn 01/09 và 05/09.

**→ QUA GATE 1.**

---

## GATE 2 — Pitch rõ, RACI không mơ hồ

> *Qua gate khi: Pitch có kết luận trước + bằng chứng + small ask, có 1 phản biện và cách xử lý, RACI có 4–6 việc quan trọng và mỗi việc có 1 Accountable rõ ràng.*

| Ô kiểm | Bài này |
|---|---|
| Pitch nói kết luận trước | ✅ Dòng đầu là đề nghị, chưa có một câu kể lể nào trước đó |
| Có 2–3 lý do chính | ✅ Đúng 3 lý do |
| Có bằng chứng hỗ trợ kết luận | ✅ Số liệu Day 25/26 truy ngược được tới ô Excel và tới script `verify_thresholds.py` (22/22 phép kiểm tra) |
| **Không hứa vượt bằng chứng** (luật số 3) | ✅ Có hẳn một khối **"Điều nhóm CHƯA có"**: containment 78% là ước tính, 4/8 đèn "chưa đo", chưa chạy ca thật nào |
| Có small ask cụ thể | ✅ 45 phút + chữ ký cho 2 tuần shadow, bắt đầu 15/09/2026 — **không** xin hợp đồng, HIS hay ngân sách |
| Có 1 phản biện có khả năng xảy ra nhất | ✅ *"AI chưa đủ đáng tin… ai chịu trách nhiệm?"* |
| Cách xử lý dựa trên **bằng chứng hoặc hành động giảm rủi ro**, không dựa trên ý kiến | ✅ 5 ý: thiết kế shadow, ranh giới pháp lý, luật dừng R-02/R-03 viết trước, bàn giao dữ liệu khi dừng, và "không xin niềm tin — xin 200 ca" |
| Bước cá nhân viết lại pitch có thật | ✅ 3 bản trong `docs/individual/`, và `docs/team-work-split.md` §4 ghi rõ **câu nào của ai** được giữ lại |
| RACI có 4–6 công việc quan trọng | ✅ **6** công việc, đúng khoảng 1–2 tháng tới |
| **Mỗi hàng đúng 1 Accountable** | ✅ **6/6** — không hàng nào hai A, không hàng nào thiếu A |
| Tách R và A khi đủ người | ✅ Tách ở **3/6** hàng (T3, T4, T5). Ba hàng còn lại R ≡ A, có ghi lý do và bù bằng **C bắt buộc là người ngoài đội** ở T1 và T6 |
| Stakeholder Trang 1 xuất hiện hợp lý trong RACI | ✅ S5, S1, S4 là ba cột thật trong ma trận |

### 6 việc của nhóm phủ đúng danh sách việc mà đề bài gợi ý

Đề bài (Phase 2.4) nêu 6 loại công việc mẫu. Nhóm **không copy nguyên danh sách đó** mà dịch từng loại sang
đúng việc thật của MedTriage AI trong 1–2 tháng tới — bảng dưới cho thấy độ phủ:

| Việc mẫu của đề bài | Việc tương ứng của nhóm | A |
|---|---|---|
| Xác định use case | **T1** — chốt phạm vi shadow pilot & thuyết phục BV A (chính là chốt use case *nào* được chạy, ở ca trực nào) | Việt |
| Xây MVP | **T2** — dựng kiosk nhập liệu tay + pipeline khử PII trong VPC bệnh viện | Hưng |
| Chuẩn bị dữ liệu | **T3** — 30 golden cases có nhãn do người hành nghề y chốt + bộ nhãn 420 ca | Linh |
| Kiểm thử | **T4** — đo under-triage & containment, chạy eval trước mỗi lần release | Linh |
| Demo / Pilot | **T5** — vận hành shadow pilot 2 tuần tại khoa (uptime, thu ca, trực tại chỗ) | Hưng |
| Quyết định release | **T6** — quyết định GO / FIX tại cổng gác ngày 30 và kích hoạt R-02 / R-03 | Việt |

**Phủ 6/6 loại việc**, và mỗi loại chỉ có **một** việc — không tách nhỏ để bảng trông nhiều hơn.

**→ QUA GATE 2.**

---

## GATE 3 — Team Design phù hợp thực tế

> *Qua gate khi: có 1 architecture được giải thích, có Core Roles, xác định capability gap và Priority Resourcing bằng Hire / Outsource / Partner thay vì chỉ liệt kê chức danh.*

| Ô kiểm | Bài này |
|---|---|
| Chọn 1 architecture | ✅ **Embedded** |
| Architecture có lý do | ✅ Có, kèm **so sánh cả 3 mô hình** và **điều kiện chuyển sang Hybrid** (≥3 bệnh viện, ≥6 người) |
| Core Roles phù hợp giai đoạn hiện tại | ✅ 3 vai trò cần ngay đã có người; vai trò thứ tư để trống và gọi đúng tên là gap |
| **Không liệt kê chức danh cho đẹp** (luật số 5) | ✅ Extended có 4 vai trò nhưng **cố ý chưa lập**, kèm nguyên tắc "mỗi chức danh thêm vào phải gỡ được một blocker của cổng gác gần nhất" |
| Có capability gap | ✅ **3 gap:** chuyên môn lâm sàng · HL7/HIS · evals |
| Priority Resourcing nói rõ Hire / Outsource / Partner | ✅ **Partner · Outsource · Partner** |
| **Giải thích vì sao chọn cách đó** (luật số 6) | ✅ Mỗi gap có đoạn lý do riêng, gồm cả lý do **bác bỏ phương án khác** (vì sao không Hire, vì sao không Outsource phần eval) |
| Có mốc "khi nào cần" | ✅ 12/09/2026 · trước cổng ngày 60 (27/10) · 19/09 và trước cổng ngày 90 (26/11) |
| Squad Goal một câu | ✅ Có, và gắn thẳng vào cổng gác ngày 30 |

**→ QUA GATE 3.**

---

## GATE 4 — Growth Plan có thể thực thi

> *Qua gate khi: team đã chấm đủ 4 khía cạnh, chọn vấn đề ưu tiên, xác định 1 năng lực cần nâng và có tối đa 3 hành động với owner + deadline + dấu hiệu hoàn thành.*

| Ô kiểm | Bài này |
|---|---|
| Chấm đủ 4 khía cạnh Team Health | ✅ Chất lượng AI · Tiến độ · Tinh thần team · Tốc độ ra sản phẩm |
| Có điểm **riêng của từng thành viên** (bước cá nhân) | ✅ 3 cột điểm riêng + trung bình + độ chênh; điểm gốc nằm trong `docs/individual/` |
| Trả lời "khía cạnh nào thấp nhất" | ✅ Tốc độ ra sản phẩm — **2,3/5** |
| Trả lời "chênh lệch lớn nhất và vì sao" | ✅ Chất lượng AI, Việt 4 vs Linh 2 — **hai người đang chấm hai thứ khác nhau** (bản thiết kế vs đầu ra lâm sàng) |
| Có vấn đề ưu tiên ảnh hưởng trực tiếp milestone tiếp theo | ✅ Không có đường đo chất lượng đầu ra → 29 ngày tới cổng ngày 30 mà chưa có ca thật nào |
| Chọn 1 role + level hiện tại + 1 competency + 1 action 30 ngày | ✅ Clinical Safety & Evals Lead · **gần L2 — AI Practitioner** · **Evals / quality evaluation** · 30 golden cases + eval mỗi release |
| Tối đa 3 hành động | ✅ Đúng **3** |
| Mỗi hành động có **owner** | ✅ Việt · Linh · Hưng — và cả ba đều là **người đang giữ chữ A** cho phần việc tương ứng trong RACI |
| Mỗi hành động có **deadline** | ✅ 03/09 & 12/09 · 19/09 · 05/09 & 28/09 |
| Mỗi hành động có **dấu hiệu hoàn thành kiểm được** | ✅ Email/biên bản ghi rõ ngày bắt đầu · `make eval` chạy trên máy cả 3 người + ≥25/30 nhãn có chữ ký người hành nghề · 4 file biên bản trong `docs/weekly/` |
| **Không phải danh sách mong muốn** | ✅ Bổ sung mục "4 việc đã bị loại khỏi Growth Plan và vì sao", trong đó có loại thẳng câu *"team cần giao tiếp tốt hơn"* vì không kiểm được |

**→ QUA GATE 4.**

---

## Kiểm tra consistency giữa 4 trang

| Câu hỏi của đề bài | Đối chiếu |
|---|---|
| **Stakeholder quan trọng ở Trang 1 có xuất hiện hợp lý trong Pitch/RACI không?** | ✅ **S1** là stakeholder ưu tiên số 1 của Trang 1, là **đối tượng của Pitch**, là **cột C trong 5/6 hàng RACI**, và là bên phải đồng ý cho hành động **G-1** của Growth Plan. **S5** là Champion ở Trang 1, là **C bắt buộc ở T1 và T6**, và là người ngoài đội dự buổi review tuần lẻ ở **G-3**. **S4** là Blocker ở Trang 1, là cột trong RACI, và là lý do tồn tại của capability gap **G-2** ở Trang 3. |
| **Capability gap ở Trang 3 có liên quan đến vấn đề Team Health ở Trang 4 không?** | ✅ Gap **G-1** (thiếu chuyên môn lâm sàng → Partner) là **nguyên nhân** của chênh lệch 2 điểm ở "Chất lượng AI", vì không ai trong đội chốt được nhãn đúng. Gap **G-3** (evals) nói thẳng phần lõi phải nâng nội bộ và **trỏ tên sang hành động G-2 của Growth Plan**. Đây không phải hai danh sách rời nhau. |
| **Growth Plan có người chịu trách nhiệm phù hợp với RACI không?** | ✅ **G-1 → Việt** (A của T1) · **G-2 → Linh** (A của T3 và T4) · **G-3 → Hưng** (A của T2 và T5). Quy tắc nhóm tự đặt: owner của một hành động Growth Plan **phải** đang giữ chữ A cho phần việc tương ứng; nếu không tìm được người như vậy thì hoặc RACI sai, hoặc hành động đó không thuộc về nhóm này. |
| **Chiều ngược lại — Trang 4 có nuôi lại Trang 1 không?** | ✅ Hành động **G-2** (mời điều dưỡng trưởng chốt nhãn, trả công theo buổi, tên ghi trong tài liệu eval) **chính là** chiến lược thuyết phục **S3** ở Trang 1 — một hành động phục vụ hai mục tiêu: lấp gap năng lực và đổi stance của một stakeholder. |

---

## GATE 5 — Repository sẵn sàng nộp

| Ô kiểm | Kết quả |
|---|---|
| Repo đúng tên theo format `Track1_Day27_TeamXX_TenDuAn` | ✅ `Track1_Day27_JCungDuoc_MedTriageAI` |
| Repo có `README.md` | ✅ |
| Repo có **đúng 01** file PDF bài làm | ✅ `Day27_AI-Team-Lab_JCungDuoc.pdf` — file PDF duy nhất trong toàn repo |
| PDF không quá 4 trang | ✅ **Đúng 4 trang**, A4 210 × 297 mm — kiểm bằng `pypdf`, không phải ước lượng |
| README ghi đủ tên team, thành viên, tên dự án | ✅ |
| Repo mở quyền truy cập cho giảng viên | ✅ (public) |
| Trưởng nhóm nộp bằng link repository | ✅ Lê Hoàng Việt gửi link; thành viên không tạo repo riêng |

**→ QUA GATE 5. Sẵn sàng nộp.**

---

## Ba điều nhóm biết là yếu và không giấu

1. **Toàn bộ phía bệnh viện (S1–S4, S7–S9) là stakeholder đã xác định được vai trò nhưng nhóm chưa tiếp cận ai.**
   Đó là lý do stance của họ ghi Trung lập / Chưa ủng hộ, và là lý do hành động G-1 đứng đầu Growth Plan với
   deadline sớm nhất. Nhóm không ghi khống một cuộc gặp nào chưa xảy ra.
2. **Cổng gác ngày 30 nhiều khả năng không đủ mẫu.** Nếu shadow bắt đầu 15/09 thì chỉ còn 12 ngày thu ca, tức
   cần ~67 ca/ngày để đạt 800. Nhóm ghi thẳng rủi ro này lên Trang 4 và chốt trước cách xử lý: **báo cáo lại quy
   mô mẫu thật tại cổng và chấp nhận kết luận FIX**, không nới định nghĩa "ca hoàn tất" cho số đẹp hơn.
3. **Ba trong sáu hàng RACI có R ≡ A.** Với 3 người thì đây là điều khó tránh, nhưng nhóm không coi đó là chuyện
   bình thường: đã bù bằng cách bắt buộc có **C là người ngoài đội** ở đúng hai hàng nguy hiểm nhất — T1 (đối
   ngoại) và T6 (quyết định release).
