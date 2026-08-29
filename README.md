# Track 1 - Day 27 — AI Team Lab

- **Team:** Nhóm JCungDuoc — **JCungDuoc**
- **Thành viên (3 người):**

| Họ và tên | MHV | Vai trò trong dự án | Vai trò trong Lab hôm nay |
|---|---|---|---|
| **Lê Hoàng Việt** | `2A202601543` | AI Product Owner / Founder | **Trưởng nhóm** — tạo & tổng hợp repository, chốt Phase 0, chủ trì Phase 1 và Phase 2 |
| **Hồ Phạm Đức Linh** | `2A202601533` | Clinical Safety & Evals Lead | Chủ trì Phase 4 (Team Health & Competency), phản biện an toàn lâm sàng cho Pitch |
| **Trần Vương Hưng** | `2A202601789` | AI / Platform Engineer | Chủ trì Phase 3 (AI Team Design & Priority Resourcing), giữ nhịp Phase 5 |

- **Tên dự án:** **MedTriage AI** — trợ lý tiếp nhận & phân loại cấp cứu cho khoa cấp cứu bệnh viện Việt Nam.
  AI trò chuyện với bệnh nhân ở hàng chờ, thu thập triệu chứng, phát hiện red flag và sinh phiếu bàn giao **SBAR** cho điều dưỡng.
  Nguyên tắc bất biến của sản phẩm: **AI đề xuất — điều dưỡng ký và quyết định.**
- **Link sản phẩm/demo (nếu có):** _chưa có bản demo công khai_ — sản phẩm đang ở **giai đoạn tiền pilot, chưa chạy ca thật nào**.
  Các artefact tiền thân của dự án (mô hình kinh tế và dashboard vận hành) nằm ở bài nộp Day 24 · Day 25 · Day 26 của nhóm.
- **Ngày làm Lab:** 29/08/2026 · **Thời lượng:** 120 phút
- **Format làm bài:** Markdown + HTML → PDF (in từ trình duyệt), tổng hợp trên chính repository này.

> **Về `TeamXX` trong tên repo:** nhóm dùng **`JCungDuoc`** theo số nhóm hiện tại.
> Nếu lớp gán số khác, đổi tên repo và đổi tên file PDF cho khớp — cấu trúc và nội dung không đổi.

---

## File nộp

| File | Nội dung |
|---|---|
| **[`Day27_AI-Team-Lab_JCungDuoc.pdf`](Day27_AI-Team-Lab_JCungDuoc.pdf)** | **Bài nộp chính — đúng 4 trang A4**, chứa đủ 4 artefact của Lab. Đây là **file PDF duy nhất** trong repo. |
| [`README.md`](README.md) | File này. |

Toàn bộ file trong `docs/` là **bằng chứng quá trình**, không phải bài nộp: nó cho phép giảng viên đối chiếu
phần **cá nhân** với phần **nhóm**, và mở lại nguồn HTML đã sinh ra file PDF.

| File phụ trợ | Vai trò |
|---|---|
| [`docs/team-work-split.md`](docs/team-work-split.md) | **Phân công cá nhân ↔ phần việc nhóm** theo từng Phase, kèm timeline 120 phút. |
| [`docs/individual/2A202601543-LeHoangViet.md`](docs/individual/2A202601543-LeHoangViet.md) | Bài làm **cá nhân** của Việt: danh sách stakeholder tự liệt kê, bản pitch tự viết lại, điểm Team Health tự chấm. |
| [`docs/individual/2A202601533-HoPhamDucLinh.md`](docs/individual/2A202601533-HoPhamDucLinh.md) | Bài làm **cá nhân** của Linh. |
| [`docs/individual/2A202601789-TranVuongHung.md`](docs/individual/2A202601789-TranVuongHung.md) | Bài làm **cá nhân** của Hưng. |
| [`docs/phase-gates.md`](docs/phase-gates.md) | Tự soi lỗi Phase 5: đối chiếu từng ô của **GATE 0 → GATE 5** và bảng consistency giữa 4 trang. |
| [`docs/ai-usage.md`](docs/ai-usage.md) | Nhóm đã dùng AI vào việc gì và **cố ý không dùng vào việc gì** (mục 9 của đề bài). |
| [`docs/source/day27-lab.html`](docs/source/day27-lab.html) | Mã nguồn HTML sinh ra file PDF. Mở bằng trình duyệt là xem được, không cần mạng. |

### Tái tạo lại file PDF

```bash
chrome --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf="Day27_AI-Team-Lab_JCungDuoc.pdf" \
  "docs/source/day27-lab.html"
```

---

### File PDF tối đa 4 trang

#### Trang 1 — Stakeholder Map & Strategy
- **Stakeholder Map** — 10 stakeholder cụ thể, đặt theo trục **Influence × Interest**, gọi tên đủ 4 vùng
  Champion / Blocker / Supporter / Bystander.
- **Stance (mức độ ủng hộ)** — chấm riêng cho từng người: Ủng hộ / Trung lập / Chưa ủng hộ.
  Nhóm ghi rõ **2 chỗ stance thực tế không khớp nhãn quadrant** (S1 và S3) và giải thích vì sao ưu tiên thực tế.
- **2 stakeholder cần tận dụng sự ủng hộ** — S5 Giảng viên/mentor Track 1 · S6 Cố vấn tài chính ngoài công ty.
- **2 stakeholder cần ưu tiên thuyết phục** — S1 Trưởng khoa Cấp cứu BV A · S3 Điều dưỡng tiếp nhận.
- **Hành động cụ thể** — 4 hành động, mỗi hành động có **owner + deadline** trong 1–2 tuần tới,
  kèm giải thích vì sao **không** chọn S2 và S4 dù cả hai là Blocker ảnh hưởng cao.

#### Trang 2 — Pitch & RACI
- **Pitch "Conclusion First"** gửi S1 — Trưởng khoa Cấp cứu: kết luận → 3 lý do → bằng chứng → small ask.
  Phần bằng chứng nói **cả thứ nhóm có lẫn thứ nhóm chưa có** (containment 78% mới là ước tính, 4/8 đèn dashboard ghi "chưa đo").
- **Phản biện chính + cách xử lý** — *"AI chưa đủ đáng tin để đụng vào bệnh nhân cấp cứu"*, trả lời bằng
  thiết kế shadow mode, ranh giới trách nhiệm pháp lý và **luật dừng R-02 / R-03 viết trước khi chạy**.
- **RACI Matrix** — 6 công việc của 1–2 tháng tới × 6 cột (3 thành viên + 3 stakeholder).
  **6/6 hàng có đúng 1 Accountable**; tách được R khỏi A ở 3/6 hàng; A chia đều **2–2–2** cho ba thành viên.

#### Trang 3 — AI Team Design
- **Team Architecture** — chọn **Embedded**, có lý do và có **điều kiện chuyển sang Hybrid** (≥3 bệnh viện và ≥6 người).
- **Core Roles** — 3 vai trò cần ngay đã có người, vai trò thứ tư (**Domain Expert lâm sàng**) **để trống và gọi đúng tên là gap**.
  Kèm danh sách Extended cố ý chưa lập, theo nguyên tắc "mỗi chức danh thêm vào phải gỡ được một blocker của cổng gác gần nhất".
- **Capability Gap** — 3 gap: chuyên môn lâm sàng · tích hợp HL7/HIS · evals có kỷ luật.
- **Priority Resourcing** — **Partner / Outsource / Partner**, mỗi lựa chọn có lý do và mốc *khi nào cần*.
  **Không gap nào được giải bằng Hire** ở giai đoạn này, và có nói rõ vì sao.
- **Squad Goal** — một câu, gắn thẳng vào cổng gác ngày 30.

#### Trang 4 — Team Health & Growth Plan
- **Team Health Score** — 3 thành viên chấm riêng 4 khía cạnh trước khi so điểm.
  Thấp nhất: **Tốc độ ra sản phẩm 2,3/5**. Chênh lệch lớn nhất: **Chất lượng AI — Việt 4 vs Linh 2**, và lý do thật của chênh lệch đó.
- **Vấn đề ưu tiên** — đội không có đường đo chất lượng đầu ra, nên còn **29 ngày** tới cổng gác ngày 30 mà chưa có ca thật nào.
- **Competency cần nâng** — Clinical Safety & Evals Lead, **gần L2 — AI Practitioner** → nâng **Evals / quality evaluation**.
- **Growth Plan 30 ngày** — đúng 3 hành động (29/08 → 28/09/2026), mỗi hành động đủ
  **owner + deadline + dấu hiệu hoàn thành kiểm được**; owner khớp đúng người giữ chữ **A** trong RACI.
- Kèm **điểm kiểm giữa kỳ ngày 14** và **4 việc đã bị loại khỏi kế hoạch cùng lý do** — để kế hoạch không thành danh sách mong muốn.

---

### Trước khi gửi link repo

- [x] Repo đúng tên theo format — `Track1_Day27_JCungDuoc_MedTriageAI`.
- [x] Repo có `README.md`.
- [x] Repo có **đúng 01** file PDF bài làm — `Day27_AI-Team-Lab_JCungDuoc.pdf`.
- [x] PDF không quá 4 trang — **đúng 4 trang**, khổ A4 (210 × 297 mm), đã kiểm bằng `pypdf`.
- [x] README ghi đủ tên team, thành viên và tên dự án.
- [x] Repo mở quyền truy cập để giảng viên có thể xem.
- [x] **Trưởng nhóm** (Lê Hoàng Việt) gửi **link GitHub repository của team** để nộp bài; các thành viên không tạo hoặc nộp repo riêng.

---

## Vì sao dự án là MedTriage AI chứ không phải một case mới

Luật số 1 của Lab: *"Dùng chính dự án hiện tại của team. Không tạo case giả chỉ để làm Lab."*

MedTriage AI là dự án nhóm đã build liên tục qua các buổi trước, nên mọi con số trong bài hôm nay đều **truy ngược được**
chứ không phải bịa để cho Pitch thuyết phục hơn:

| Nguồn | Thứ được dùng lại ở Day 27 |
|---|---|
| **Day 22** — Responsible AI in Production | Ranh giới *AI đề xuất — người quyết định*; kết luận release `conditional-go` và **5 blocker** chưa gỡ; harm map và vai trò của điều dưỡng. Đây là bằng chứng cho phần trả lời phản biện ở Trang 2 và cho mức năng lực hiện tại ở Trang 4. |
| **Day 24** — Financial Model | Mô hình B2B Hybrid (phí nền + phí theo ca); AI Hidden Costs ≥30% API cost. |
| **Day 25** — Monetization & GTM | Giá **6.000.000 ₫/tháng + 13.000 ₫/ca**; gross margin **71,8%**; breakeven containment **55,1%**; CAC payback **11,9 tháng**. |
| **Day 26** — Operating Dashboard | North Star **Time-to-first-value**; **cổng gác ngày 30 / 60 / 90** (27/09 · 27/10 · 26/11); luật dừng **R-02 / R-03**; ngưỡng **MH-03** chi phí triển khai ÷ ACV ≤24,4%; và lời tự phê *"dashboard của một sản phẩm chưa chạy ca thật nào"* — chính là vấn đề ưu tiên của Trang 4. |

**Điều nhóm cố ý không làm:** không nâng containment 78% thành "đã đo", không bịa tên bệnh viện hay tên bác sĩ,
không ghi stakeholder nào mà nhóm chưa xác định được vai trò thật. Stakeholder nào chưa tiếp cận thì stance ghi
**Trung lập** hoặc **Chưa ủng hộ** đúng như hiện trạng — kể cả khi việc đó làm bức tranh xấu đi.
