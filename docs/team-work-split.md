# Phân công cá nhân và phần việc nhóm — Day 27 · AI Team Lab

Nhóm **JCungDuoc** · Track 1 · Dự án **MedTriage AI** · ngày làm Lab **29/08/2026**

Tài liệu này là **tài liệu của nhóm**. Nó tồn tại để giảng viên đối chiếu được: chỗ nào là **bài làm cá nhân**
(mỗi người tự làm trước, chưa thảo luận), chỗ nào là **kết quả nhóm đã chốt chung**, và ai chịu trách nhiệm
cho phần nào của file PDF 4 trang.

---

## 1. Thành viên, vai trò dự án và vai trò trong Lab

| Họ và tên | MHV | Vai trò trong dự án MedTriage AI | Vai trò trong Lab Day 27 | Sở hữu trang nào của PDF |
|---|---|---|---|---|
| **Lê Hoàng Việt** | `2A202601543` | **AI Product Owner / Founder** — sở hữu mô hình kinh tế, 3 cổng gác, quan hệ stakeholder, quyết định release | **Trưởng nhóm & người tổng hợp** — tạo repo, chốt Phase 0, chủ trì Phase 1 và Phase 2 | **Trang 1** và **Trang 2** |
| **Hồ Phạm Đức Linh** | `2A202601533` | **Clinical Safety & Evals Lead** — định nghĩa red flag, bộ golden cases, ngưỡng under-triage, quyền bấm luật dừng R-03 | **Chủ trì Phase 4** — Team Health, Competency L1/L2/L3, Growth Plan; phản biện an toàn lâm sàng cho Pitch | **Trang 4** |
| **Trần Vương Hưng** | `2A202601789` | **AI / Platform Engineer** — kiosk, VPC, khử PII, pipeline dữ liệu, eval harness, uptime pilot | **Chủ trì Phase 3** — AI Team Architecture, Core Roles, Priority Resourcing; giữ nhịp Phase 5 | **Trang 3** |

### Vì sao chia vai đúng như vậy — căn cứ từ bài làm trước của chính nhóm

Không phải chia ngẫu nhiên hay chia theo chức danh nghe hay. Mỗi người nhận đúng phần mình đã có bằng chứng năng lực:

- **Việt → Product Owner, Trang 1 + Trang 2.** Là người dựng **mô hình kinh tế Day 25** (giá, gross margin 71,8%,
  breakeven containment 55,1%) và **dashboard vận hành Day 26** (8 đèn, 4 phép tính `[MH]`, 5 luật quyết định,
  3 cổng gác). Pitch ở Trang 2 phải đứng trên đúng những con số đó, và người bảo vệ được chúng trước Trưởng khoa
  Cấp cứu là người đã tính ra chúng. Quan hệ với mentor (S5) và cố vấn tài chính (S6) cũng đang nằm ở người này.
- **Linh → Clinical Safety & Evals, Trang 4.** Ở **Day 22**, Linh làm hồ sơ ngành `healthcare-assistant` cho
  ClinIQ Diagnostic Copilot: **harm map 10 dòng đủ 7 failure layer**, **8 compliance gap**, **5 release blocker**,
  kết luận `conditional-go` cho pilot một khoa. Đây là người duy nhất trong nhóm đã từng ngồi với rủi ro lâm sàng
  ở mức chi tiết — nên Trang 4 (Team Health + competency cần nâng) do Linh chủ trì, và **role được chọn để nâng
  competency ở Trang 4 chính là role của Linh**, không phải chọn hộ người khác.
- **Hưng → Platform, Trang 3.** Ở **Day 22**, Hưng làm ngành `mobility-autonomous-driving` cho SafeLane Highway
  Assist — ngành mà chính nhóm chốt là **stakes cao nhất** vì harm không đảo ngược được, và là người phải định
  nghĩa **system boundary** cho một hệ `semi-automated`. Trang 3 hỏi đúng câu đó ở cấp tổ chức: năng lực nào
  nằm trong đội, năng lực nào mua ngoài, ranh giới ở đâu.

---

## 2. Artefact nào là cá nhân, artefact nào là nhóm

| Artefact | Cá nhân hay nhóm | Ghi chú |
|---|---|---|
| Danh sách stakeholder tự liệt kê (Phase 1.1) | **Cá nhân** | Mỗi người tự liệt kê **≥6 stakeholder** trong 5 phút, **không nhìn bài nhau**. Nằm ở `docs/individual/<MHV>-<Tên>.md`. |
| Bản pitch tự viết lại (Phase 2.3) | **Cá nhân** | Mỗi người tự viết lại pitch theo cấu trúc Conclusion First bằng chữ của mình, để kiểm tra là **hiểu thông điệp** chứ không phải đang gật đầu với bản nháp chung. |
| Điểm Team Health 1–5 (Phase 4.1) | **Cá nhân** | Chấm riêng **trước khi thảo luận**. Chính vì chấm riêng mới lộ ra chênh lệch 2 điểm ở "Chất lượng AI". |
| **Stakeholder Map + 4 chiến lược** (Trang 1) | **NHÓM** | Gộp 3 danh sách cá nhân, loại trùng, đặt lên ma trận, chấm stance, chọn 4 stakeholder ưu tiên. |
| **Pitch bản cuối + phản biện + RACI** (Trang 2) | **NHÓM** | Bản cuối là **tổng hợp câu rõ nhất từ 3 bản cá nhân** — xem mục 4 để biết câu nào lấy của ai. |
| **AI Team Design** (Trang 3) | **NHÓM** | Architecture, Core Roles, 3 capability gap, Priority Resourcing, Squad Goal. |
| **Team Health & Growth Plan** (Trang 4) | **NHÓM** | So điểm cá nhân → chọn vấn đề ưu tiên → chọn competency → chốt 3 hành động. |
| `docs/phase-gates.md`, `docs/ai-usage.md`, file này | **NHÓM** | Tài liệu quá trình, không thuộc 4 trang bài nộp. |

---

## 3. Timeline 120 phút — ai làm gì, lúc nào

### Phase 0 · 5 phút · **Team** — Chốt phạm vi
Cả ba cùng xác nhận đang nói về **cùng một dự án** (MedTriage AI), **cùng một mục tiêu hiện tại**
(qua cổng gác ngày 30 — 27/09/2026), và **một người tổng hợp** (Việt). Việt tạo repository ngay ở phút thứ 5
và dùng xuyên suốt đến lúc nộp.

### Phase 1 · 20 phút · **Cá nhân → Team** — Stakeholder Map

| Phút | Việc | Hình thức | Việt | Linh | Hưng |
|---:|---|---|---|---|---|
| 0–5 | Liệt kê ≥6 stakeholder | **Cá nhân** | 8 stakeholder, nghiêng về phía **thương mại và học thuật**: mentor, cố vấn tài chính, ban giám đốc, quỹ ươm tạo | 7 stakeholder, nghiêng về phía **lâm sàng và người bị ảnh hưởng**: trưởng khoa, điều dưỡng tiếp nhận, bệnh nhân & người nhà, hội đồng QLCL | 7 stakeholder, nghiêng về phía **hạ tầng và dữ liệu**: phòng CNTT/HIS, nhà cung cấp HIS đương nhiệm, đơn vị pháp lý dữ liệu |
| 5–12 | Gộp, loại trùng, đặt lên ma trận, chấm stance | **Team** | Chốt trục Influence | Chốt stance thực tế từng người | Chốt vị trí S4, S7 |
| 12–20 | Chọn 4 stakeholder ưu tiên + hành động | **Team** | Viết chiến lược cho S5, S6, S1 | Viết chiến lược cho S3 | Kiểm tra "hành động này có kiểm được không?" |

**Kết quả gộp:** 22 mục thô → loại trùng và gộp còn **10 stakeholder** trên bản đồ.
**Phát hiện chỉ có được nhờ làm cá nhân trước:** không ai trong ba người tự mình liệt kê đủ cả ba nhóm.
Danh sách của Việt **không có S3 (điều dưỡng tiếp nhận)** — đúng người có quyền phủ quyết thực địa;
danh sách của Linh **không có S4 (phòng CNTT)** — đúng người giữ cửa dữ liệu.
Nếu Phase 1 làm theo kiểu cả nhóm cùng brainstorm ngay từ đầu, bản đồ sẽ nghiêng theo người nói to nhất.

### Phase 2 · 30 phút · **Team → Cá nhân → Team** — Pitch & RACI

| Phút | Việc | Hình thức | Ai làm gì |
|---:|---|---|---|
| 0–10 | Chọn stakeholder & viết pitch nháp | **Team** | Chọn **S1 — Trưởng khoa Cấp cứu** vì đây là nút thắt duy nhất của cổng ngày 30. Việt viết nháp, cả nhóm cắt bớt phần hứa. |
| 10–15 | Chuẩn bị phản biện | **Team** | **Linh** đề xuất phản biện *"AI chưa đủ đáng tin… ai chịu trách nhiệm?"* và viết 3/5 ý trả lời — đây là địa hạt của Linh. |
| 15–20 | **Mỗi người tự viết lại pitch** | **Cá nhân** | 3 bản trong `docs/individual/`. Không nhìn bản của nhau. |
| 20–30 | Chốt RACI 6 việc | **Team** | Hưng đề xuất tách R khỏi A ở T3/T4/T5; cả nhóm kiểm lại "mỗi hàng đúng 1 A". |

### Phase 3 · 25 phút · **Team** — AI Team Design
**Hưng chủ trì.** Việt phản biện phần chi phí (mỗi lựa chọn Hire/Outsource/Partner phải chịu được ngưỡng
**MH-03: chi phí triển khai ÷ ACV ≤24,4%**). Linh phản biện phần gap chuyên môn lâm sàng và **bác bỏ phương án
Outsource cho gap G-3 (evals)** với lý do: thuê ngoài phần eval là tự bịt mắt đội. Ý này được giữ nguyên vào PDF.

### Phase 4 · 25 phút · **Cá nhân → Team** — Team Health & Growth Plan

| Phút | Việc | Hình thức | Ghi chú |
|---:|---|---|---|
| 0–5 | Chấm 4 khía cạnh 1–5 | **Cá nhân** | Không ai nói điểm của mình trước khi cả ba chấm xong. |
| 5–12 | So điểm & chọn vấn đề | **Team** | Lộ ra **chênh 2 điểm ở "Chất lượng AI" (Việt 4 — Linh 2)**. Truy ra nguyên nhân: hai người đang chấm hai thứ khác nhau. |
| 12–17 | Chọn competency cần nâng | **Team** | Chọn role **Clinical Safety & Evals Lead**, mức **gần L2**, năng lực cần nâng là **Evals**. |
| 17–25 | Chốt Growth Plan 30 ngày | **Team** | 3 hành động, owner khớp đúng người giữ chữ **A** trong RACI. |

**Quy tắc nhóm tự đặt cho Phase 4:** owner của mỗi hành động Growth Plan **phải là người đang giữ chữ A** cho
phần việc tương ứng trong RACI. Nếu không tìm được người như vậy thì hoặc RACI sai, hoặc hành động đó không
thuộc về nhóm này — hai trường hợp đều phải sửa chứ không được giao đại.

### Phase 5 · 15 phút · **Team, trưởng nhóm phụ trách repo**
Cả ba mở 4 trang và tick từng ô GATE (`docs/phase-gates.md`). **Hưng** giữ nhịp đọc checklist, **Linh** kiểm
consistency giữa Trang 3 và Trang 4, **Việt** kiểm cấu trúc repo, export PDF và kiểm số trang.

---

## 4. Câu nào trong bản Pitch cuối là của ai

Bước cá nhân ở Phase 2.3 chỉ có giá trị nếu bản cuối **thật sự lấy chữ của từng người**, chứ không phải viết
riêng cho vui rồi vẫn dùng bản nháp của trưởng nhóm. Bản cuối ở Trang 2 lấy như sau:

| Phần của Pitch | Lấy từ bản của | Lý do chọn câu đó |
|---|---|---|
| **Kết luận** — "shadow mode 2 tuần, ca trực ngày, mục tiêu 200 ca" | **Việt** | Bản duy nhất nêu small ask ngay trong câu kết luận, nên người nghe biết mình được xin gì trước khi nghe lý do. |
| **Lý do 2** — "shadow mode làm rủi ro lâm sàng bằng 0 **theo thiết kế**, chứ không bằng lời hứa" | **Linh** | Hai bản kia viết "rủi ro thấp". "Bằng 0 theo thiết kế" là câu kiểm được, "thấp" thì không. |
| **Lý do 3** — "khoa giữ được số đo **kể cả khi khoa quyết định dừng**" | **Hưng** | Câu duy nhất đưa ra thứ stakeholder được giữ trong **kịch bản xấu nhất** — đây là thứ hạ rào cản đồng ý xuống thấp nhất. |
| **Bằng chứng — phần "Điều nhóm CHƯA có"** | **Linh** | Việt viết phần số liệu; Linh là người đòi phải nói trước cả phần chưa đo, nếu không thì Pitch đang hứa vượt bằng chứng. |
| **Small ask** — "45 phút + chữ ký cho 2 tuần, không hợp đồng, không HIS" | **Việt**, sửa theo góp ý của **Hưng** | Bản gốc xin cả quyền truy cập HIS. Hưng chỉ ra: xin HIS là kéo S4 vào từ tuần đầu và biến một small ask thành một dự án. Đã cắt. |

---

## 5. Ranh giới trách nhiệm khi bảo vệ bài

- **Việt** bảo vệ: Stakeholder Map, lựa chọn 4 stakeholder ưu tiên, toàn bộ Pitch và phản biện,
  cấu trúc RACI, và mọi con số kinh tế được trích (giá, gross margin, breakeven, các cổng gác).
- **Linh** bảo vệ: stance thực tế của S1/S3, phần trả lời phản biện về an toàn lâm sàng, capability gap G-1 và G-3,
  toàn bộ Trang 4 — điểm Team Health, vấn đề ưu tiên, khung competency L1/L2/L3 và hành động G-2 của Growth Plan.
- **Hưng** bảo vệ: lựa chọn architecture Embedded và điều kiện chuyển Hybrid, capability gap G-2 (HL7/HIS),
  lý do Outsource theo gói thay vì Hire, cách tách R khỏi A trong RACI, và hành động G-3 của Growth Plan.
- **Cả ba cùng bảo vệ:** Squad Goal ở Trang 3 và bảng consistency ở Trang 4 — vì đó là hai chỗ duy nhất
  ràng 4 trang lại với nhau.

Điểm nhóm biết là yếu nhất và sẽ **không** giấu khi bảo vệ: **toàn bộ phía bệnh viện (S1–S4, S7–S9) hiện là
stakeholder đã xác định được vai trò nhưng nhóm chưa tiếp cận ai.** Đó chính là lý do stance của họ được ghi
Trung lập / Chưa ủng hộ, và là lý do hành động G-1 của Growth Plan đứng đầu danh sách với deadline sớm nhất.
